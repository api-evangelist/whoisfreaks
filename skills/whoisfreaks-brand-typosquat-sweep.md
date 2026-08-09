---
name: Brand typosquat sweep
description: Enumerate typo variants of a brand, find which are registered, and triage the registered ones for phishing risk.
api: openapi/whoisfreaks-openapi-original.yml
operations: [typosquatting, domainAvailabilityV2, bulkDomainAvailabilityV2, whoisLive, dnsLive, domainReputation]
generated: '2026-08-09'
method: generated
source: openapi/whoisfreaks-openapi-original.yml + conventions/whoisfreaks-conventions.yml
---

# Brand typosquat sweep

Use this when asked "who is squatting on our brand" or "is anyone impersonating this domain".

## Auth

`apiKey` query parameter. Base URL `https://api.whoisfreaks.com`.

## Steps

1. **`typosquatting`** — `GET /v3.0/domain/typos?apiKey=…&keyword=<brand>`
   Generate and look up typo/lookalike variants. Optional `pattern` and
   `labelLength` narrow the generator; `page` pages the results.
   **This endpoint bills 5 credits per page** — decide how deep to go first.
2. **`domainAvailabilityV2`** / **`bulkDomainAvailabilityV2`** —
   `GET` or `POST /v2.0/domain/availability`
   Split the candidate list into registered (the threat) and available (the
   defensive-registration shopping list). Use the bulk POST for the list —
   **100 domains maximum per request**, `413` above that.
3. **`whoisLive`** — for each registered variant, pull registration date and
   registrant. Domains registered in the last 30 days are the priority queue.
4. **`dnsLive`** — `type=all`. A variant with MX records is being prepared for
   email-based phishing even if it has no website yet; a variant with no
   records at all is parked.
5. **`domainReputation`** — `GET /v1/domain/security?apiKey=…`
   Scores the domain, including DGA features and risk categories. Note this
   endpoint sits on the `/v1/` prefix, not `/v1.0/`.

## Rules

- **Do not brute-force the variant space yourself.** `typosquatting` is the
  generator; enumerating candidates client-side and checking each one burns
  credits for a worse result.
- `typosquatting` is in the historical/reverse rate class — **10 rpm**.
- **`403` = unsupported TLD.** Expect it across the long tail of the 1528+ TLDs
  the monitoring products cover; skip and continue rather than aborting.
- For ongoing coverage, stop calling the API on a loop and point the user at
  Brand Monitoring (twice-daily scans, webhook or email alerts) — see
  `asyncapi/whoisfreaks-monitoring-webhooks.yml`.

## Output

A table of registered lookalikes with registration date, registrant (or
redacted), whether MX/A records exist, and the reputation verdict — sorted by
registration recency. Then the available variants worth defensively registering.
