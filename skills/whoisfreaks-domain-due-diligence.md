---
name: Domain due diligence
description: Build a full picture of one domain — registration, hosting, certificate and attack surface — in four calls.
api: openapi/whoisfreaks-openapi-original.yml
operations: [whoisLive, dnsLive, sslLookup, subdomains]
generated: '2026-08-09'
method: generated
source: openapi/whoisfreaks-openapi-original.yml + conventions/whoisfreaks-conventions.yml
---

# Domain due diligence

Use this when asked "who owns this domain / is this domain legitimate / what is it running".

## Auth

Every call takes `apiKey` as a **query parameter** — there is no header option.
Read it from the environment; never echo it back to the user and never put it in
a URL you display, because the key is visible in any logged URL.

Base URL: `https://api.whoisfreaks.com`

## Steps

1. **`whoisLive`** — `GET /v2.0/whois/live?apiKey=…&domainName=<domain>`
   Registration facts: registrar, registrant, create/update/expiry dates,
   nameservers, status codes. A very recent `create_date` is the single strongest
   risk signal on this API.
2. **`dnsLive`** — `GET /v2.0/dns/live?apiKey=…&domainName=<domain>&type=all`
   Resolve A/AAAA/MX/NS/TXT. Keep the A-record IPs — they are the join key into
   the IP triage skill (`whoisfreaks-ip-triage`).
3. **`sslLookup`** — `GET /v1.0/ssl/live?apiKey=…&domainName=<domain>&chain=true`
   Issuer, validity window and SANs. SANs frequently reveal sibling domains the
   operator owns.
4. **`subdomains`** — `GET /v1.0/subdomains?apiKey=…&domain=<domain>`
   Known subdomains. Paginate with `page`; this endpoint is in the historical/
   reverse rate class (10 rpm), so pace it.

## Rules

- **Rate classes differ.** `whoisLive`, `dnsLive`, `sslLookup` are live (80 rpm);
  `subdomains` is slower. Read `x-ratelimit-remaining-requests`; on `429`, take
  `x-ratelimit-remaining-time`, divide by 1e9 for seconds, sleep that plus
  ~200ms. Throttled calls are not billed.
- **`404` is a result, not a failure.** It means no record exists — say so
  rather than retrying.
- **`403` means the TLD is unsupported**, not that the domain is fake. Check
  https://whoisfreaks.com/supported-tlds before concluding anything.
- **`206`/`210` are successes.** `206` is a partial response; `210` means the
  answer came from cache because the upstream WHOIS server did not respond —
  flag the staleness in your answer.
- **Every call costs credits.** Do not loop; four calls is the whole job.
- There is **no idempotency key**. Retrying bills again.

## Output

Registration age and registrar, registrant (or "redacted"), hosting IPs and
provider, certificate issuer/expiry, and the subdomain count — then one
sentence on whether anything looks anomalous, citing the field that says so.
