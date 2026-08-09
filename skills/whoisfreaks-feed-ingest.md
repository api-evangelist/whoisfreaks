---
name: Bulk feed and database ingest
description: Check what data is ready, download the newly-registered-domain and threat feeds, and watch credit burn.
api: openapi/whoisfreaks-openapi-original.yml
operations: [databaseFileStatus, dbNewlyGtldJson, dbNewlyCctldJson, dbNewlyGtld, dbNewlyCctld, dbDroppedJson, downloadThreatFeedPhishing, downloadThreatFeedPhishingSample, downloadThreatFeedMalware, downloadThreatFeedSpam, accountUsage]
generated: '2026-08-09'
method: generated
source: openapi/whoisfreaks-openapi-original.yml + conventions/whoisfreaks-conventions.yml
---

# Bulk feed and database ingest

Use this for the file side of WhoisFreaks — daily newly-registered domains,
dropped domains, and the phishing/malware/spam threat feeds.

## Hosts

Live lookups are on `https://api.whoisfreaks.com`. **Bulk downloads are served
from `https://files.whoisfreaks.com`** — the OpenAPI declares both servers, and
using the wrong one is the most common failure on this surface.

Auth is the same `apiKey` query parameter.

## Steps

1. **`databaseFileStatus`** — `GET /v3.4/status`
   Documented as public. Call it **first, every run**: it reports which daily,
   weekly and monthly files have actually been produced and for which date
   ranges. Downloading before the file exists is the usual cause of an empty or
   failed pull.
2. Pull the feed you need:
   - Newly registered, JSON: **`dbNewlyGtldJson`** `GET /v3.1/domains/newly/gtld`,
     **`dbNewlyCctldJson`** `GET /v3.1/domains/newly/cctld`
   - Newly registered, CSV: **`dbNewlyGtld`**, **`dbNewlyCctld`**
     (`/v3.1/download/domainer/gtld|cctld`), with `…/cleaned` variants that
     include parsed WHOIS
   - Dropped, JSON: **`dbDroppedJson`** `GET /v3.1/domains/dropped`
   - Threat feeds: **`downloadThreatFeedPhishing`**, **`downloadThreatFeedMalware`**,
     **`downloadThreatFeedSpam`** under `/v3.4/download/threat-feed/…` (CSV, daily)
3. **Try the sample first.** `downloadThreatFeedPhishingSample` (and the malware
   and spam equivalents) return a sample of the same shape — use them to build
   and test the parser before spending on a full pull.
4. **`accountUsage`** — `GET /v1.0/whoisapi/usage`
   Check remaining credits and subscription state after the run. Bulk pulls are
   where credit burn actually happens.

## Rules

- **Cadence.** Newly-registered feeds are produced twice daily; dropped and
  threat feeds daily. Polling more often than that returns the same file and
  wastes credits — there is no `If-Modified-Since` or ETag contract documented.
- **`412` = plan limit reached.** Stop; do not retry in a loop.
- **`408`/`499`**: these are large files. Raise the client timeout rather than
  retrying — `499` specifically means *your* timeout was too short.
- No idempotency key exists, and a re-download is billed again. Persist what you
  fetched and check the file status before re-pulling.
- Free, no-key alternatives exist for evaluation: the public GitHub datasets
  `WhoisFreaks/daily-newly-registered-domains` and
  `WhoisFreaks/daily-expired-and-dropped-domains`.

## Output

Which files were available per `databaseFileStatus`, what you pulled (feed,
date, row count), what you skipped and why, and the remaining credit balance.
