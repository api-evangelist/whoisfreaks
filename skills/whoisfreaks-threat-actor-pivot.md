---
name: Threat actor infrastructure pivot
description: Start from one bad domain and enumerate the rest of the actor's infrastructure via reverse WHOIS and reverse DNS.
api: openapi/whoisfreaks-openapi-original.yml
operations: [whoisLive, whoisHistory, whoisReverse, dnsLive, dnsReverse]
generated: '2026-08-09'
method: generated
source: openapi/whoisfreaks-openapi-original.yml + conventions/whoisfreaks-conventions.yml
---

# Threat actor infrastructure pivot

Use this when given one suspicious domain and asked "what else does this actor own".

## Auth

`apiKey` query parameter on every call. Base URL `https://api.whoisfreaks.com`.

## Steps

1. **`whoisLive`** — `GET /v2.0/whois/live?apiKey=…&domainName=<domain>`
   Pull the registrant email, owner name and organization. If the record is
   privacy-redacted, go to step 2 before giving up.
2. **`whoisHistory`** — `GET /v2.0/whois/history?apiKey=…&domainName=<domain>`
   Historical records frequently expose a registrant identity that the current
   record redacts. Take the pre-redaction email/owner/company.
3. **`whoisReverse`** — `GET /v2.0/whois/reverse?apiKey=…&email=<email>`
   (or `&owner=`, `&company=`, `&keyword=`). This searches 4.1B+ current and
   historical records. Regex is supported on `email`; `owner`, `company` and
   `keyword` are exact-match. `keyword` accepts 3–63 characters.
   Paginate with `page` — 50 records per page, 100 in mini mode.
4. **`dnsLive`** — resolve the seed domain, keep the A-record IP and the NS
   hostnames.
5. **`dnsReverse`** — `GET /v2.1/dns/reverse?apiKey=…&value=<ip-or-nameserver>&type=a`
   Enumerate every other domain pointing at the same IP or nameserver. This is
   the hosting-side pivot that catches infrastructure the registrant-side pivot
   misses.

## Rules

- **Slowest rate class.** `whoisHistory`, `whoisReverse` and `dnsReverse` are
  the historical/reverse class — **10 requests per minute**. Budget for it:
  serialize, do not fan out.
- **Pagination bills per page.** Reverse DNS is 5 credits per page. Stop at the
  page count you actually need and report the total rather than pulling
  everything.
- **`412` means the plan is exhausted**, not that the query is wrong.
- Two-hop pivots explode fast. Cap the expansion (e.g. top 25 domains by
  registration recency) and say what you capped.
- Redaction is normal for ccTLDs and post-GDPR gTLDs — absence of a registrant
  is not evidence of anything.

## Output

The pivot key you used, the number of domains it returned, the most recent
registrations, and which of them share the seed's IP or nameserver. Distinguish
registrant-side matches from hosting-side matches — they are different strengths
of evidence.
