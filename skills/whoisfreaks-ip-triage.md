---
name: IP address triage
description: Decide whether an IP is worth blocking — geolocation, reputation flags, registration ownership and its ASN.
api: openapi/whoisfreaks-openapi-original.yml
operations: [ipReputation, geolocation, ipWhois, asnWhois, bulkIpReputation, bulkGeolocation]
generated: '2026-08-09'
method: generated
source: openapi/whoisfreaks-openapi-original.yml + conventions/whoisfreaks-conventions.yml
---

# IP address triage

Use this when handed one or many IPs and asked whether to trust, rate-limit or block.

## Auth

`apiKey` query parameter. Base URL `https://api.whoisfreaks.com`.

## Steps

1. **`ipReputation`** — `GET /v1.0/security?apiKey=…&ip=<ip>`
   The decision call: proxy, VPN, Tor exit node, bot and threat flags.
2. **`geolocation`** — `GET /v1.0/geolocation?apiKey=…&ip=<ip>`
   Country, city, ISP, coordinates, plus the network/ASN and company blocks.
3. **`ipWhois`** — `GET /v1.0/ip-whois?apiKey=…&ip=<ip>`
   The registration side: inetnum range, route, abuse/IRT contact, organization.
   Use the IRT contact when you need somewhere to report abuse.
4. **`asnWhois`** — `GET /v2.0/asn-whois?apiKey=…&asn=<ASNxxxx>`
   Take the ASN from step 2 or 3. Peers and org tell you whether the address sits
   in a bulletproof/anonymizing network or a mainstream provider.

## Many IPs at once

Use the bulk POST variants instead of looping:

- **`bulkIpReputation`** — `POST /v1.0/security`
- **`bulkGeolocation`** — `POST /v1.0/geolocation`

**Maximum 100 entries per request** — over that you get `413`. Bulk operations
are the 20 rpm class.

## Rules

- **`423 Locked` means you sent a bogon** (reserved/unroutable) range. Filter
  RFC1918, loopback, link-local and reserved space client-side first.
- **`404` on `ipWhois` means the IP is not in the database** — a legitimate empty
  answer, not an error.
- The bulk POSTs are read-only fan-outs, so a retry is safe **but is billed
  again**; there is no idempotency key. Deduplicate before you send.
- Rate-limit handling: read `x-ratelimit-remaining-requests`; on `429`, convert
  `x-ratelimit-remaining-time` from nanoseconds and sleep.

## Output

A verdict per IP (allow / watch / block), the single flag that drove it, the
network owner and ASN, and the abuse contact if a report is warranted. Say
explicitly when reputation is clean but the ASN is anonymizing — those are
different findings.
