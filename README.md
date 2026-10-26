# WhoisFreaks (whoisfreaks)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

WhoisFreaks is a domain and IP intelligence provider whose REST API suite covers live WHOIS, historical WHOIS, bulk and reverse WHOIS, IP and ASN WHOIS, live/historical/reverse DNS, domain availability with suggestions, typosquatting discovery, SSL certificate lookup, subdomain enumeration, IP geolocation, IP reputation and domain reputation. Alongside the live lookup APIs it ships bulk downloadable databases (WHOIS, DNS, subdomains, IP geolocation, IP security, ASN, newly registered domains, expiring and dropped domains, and daily phishing/malware/spam threat feeds), brand/domain/registrant monitoring services with email, Telegram and webhook alerts, ten officially maintained OpenAPI-generated SDKs, a Go CLI, an n8n community node, and an open-source MCP server exposing fourteen domain-intelligence tools to AI assistants. Authentication is a single apiKey query parameter across every endpoint.

**APIs.json:** [https://whoisfreaks.apievangelist.com/apis.yml](https://whoisfreaks.apievangelist.com/apis.yml)

## Tags

- WHOIS
- DNS
- Domain Intelligence
- IP Intelligence / Geolocation
- Cybersecurity / Threat Intelligence
- OSINT
- Reverse Lookup
- SSL/Certificate
- Domain Monitoring
- Brand Protection
- Threat Feeds
- Domain Availability

## Timestamps

- **Created:** 2026-07-29
- **Modified:** 2026-08-09

## APIs

### WhoisFreaks MCP Server

Official open-source Model Context Protocol server (Java) exposing 14 WhoisFreaks domain-intelligence tools to MCP-compatible AI clients. Distributed as source and as the whoisfreaks/mcp-server Docker image; runs over stdio locally or HTTP/SSE on port 3100 when self-hosted. No vendor-hosted public MCP endpoint.

- **Human URL:** [https://github.com/WhoisFreaks/whoisfreaks-mcp-server](https://github.com/WhoisFreaks/whoisfreaks-mcp-server)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- MCP
- Domain Intelligence
- WHOIS
- DNS
- Cybersecurity / Threat Intelligence

#### Properties

- [M C P Server](mcp/whoisfreaks-mcp.yml)
- [Tool Crosswalk](mcp/whoisfreaks-tool-crosswalk.yml)
- [Source Code](https://github.com/WhoisFreaks/whoisfreaks-mcp-server)
- [Postman Collection](collections/whoisfreaks-account-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-account-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-asn-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-asn-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-asn-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-asn-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-dns-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-dns-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-expiring-dropped-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-expiring-dropped-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-ip-geolocation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-geolocation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-ip-security-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-security-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-ip-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-newly-registered-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-newly-registered-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-subdomains-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-subdomains-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-threat-feed-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-threat-feed-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-databases-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-dns-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-dns-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-domain-availability-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-domain-availability-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-domain-reputation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-domain-reputation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-geolocation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-geolocation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-ip-reputation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ip-reputation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-ip-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ip-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-ssl-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ssl-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-subdomains-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-subdomains-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-typosquatting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-typosquatting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/whoisfreaks-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### WhoisFreaks Account API

Account, API key, and usage utilities

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Account

#### Properties

- [OpenAPI](openapi/whoisfreaks-account-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-account-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-account-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks ASN WHOIS API

Autonomous System Number WHOIS

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- ASN WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-asn-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-asn-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-asn-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - ASN WHOIS API

ASN WHOIS database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - ASN WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-asn-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-asn-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-asn-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - DNS API

DNS database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - DNS

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-dns-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-dns-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-dns-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - Expiring & Dropped API

Expiring and dropped domain downloads

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - Expiring & Dropped

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-expiring-dropped-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-expiring-dropped-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-expiring-dropped-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - IP Geolocation API

IP geolocation database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - IP Geolocation

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-ip-geolocation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-ip-geolocation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-geolocation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - IP Security API

IP security database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - IP Security

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-ip-security-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-ip-security-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-security-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - IP WHOIS API

IP WHOIS database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - IP WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-ip-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-ip-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-ip-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - Newly Registered API

Newly registered domain downloads

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - Newly Registered

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-newly-registered-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-newly-registered-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-newly-registered-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - Subdomains API

Subdomain database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - Subdomains

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-subdomains-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-subdomains-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-subdomains-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - Threat Feed API

The Databases - Threat Feed API from WhoisFreaks — 6 operation(s) for databases - threat feed.

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - Threat Feed

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-threat-feed-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-threat-feed-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-threat-feed-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Databases - WHOIS API

WHOIS database snapshots

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Databases - WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-databases-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-databases-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-databases-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks DNS API

DNS lookup APIs (live, historical, reverse, bulk)

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- DNS

#### Properties

- [OpenAPI](openapi/whoisfreaks-dns-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-dns-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-dns-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Domain Availability API

Check domain availability

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Domain Availability

#### Properties

- [OpenAPI](openapi/whoisfreaks-domain-availability-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-domain-availability-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-domain-availability-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Domain Reputation API

Real-time domain threat assessment and trust scoring

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Domain Reputation

#### Properties

- [OpenAPI](openapi/whoisfreaks-domain-reputation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-domain-reputation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-domain-reputation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Geolocation API

IP geolocation lookup

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Geolocation

#### Properties

- [OpenAPI](openapi/whoisfreaks-geolocation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-geolocation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-geolocation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks IP Reputation API

IP threat intelligence

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- IP Reputation

#### Properties

- [OpenAPI](openapi/whoisfreaks-ip-reputation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-ip-reputation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ip-reputation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks IP WHOIS API

IP address WHOIS

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- IP WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-ip-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-ip-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ip-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks SSL API

SSL certificate lookup

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- SSL

#### Properties

- [OpenAPI](openapi/whoisfreaks-ssl-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-ssl-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-ssl-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Subdomains API

Subdomain enumeration

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Subdomains

#### Properties

- [OpenAPI](openapi/whoisfreaks-subdomains-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-subdomains-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-subdomains-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks Typosquatting API

Detect typo variants of brand domains

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- Typosquatting

#### Properties

- [OpenAPI](openapi/whoisfreaks-typosquatting-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-typosquatting-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-typosquatting-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

### WhoisFreaks WHOIS API

WHOIS lookup APIs (live, historical, reverse, bulk)

- **Human URL:** [https://whoisfreaks.com/documentation/whois-api](https://whoisfreaks.com/documentation/whois-api)
- **Base URL:** `https://api.whoisfreaks.com`

#### Tags

- WHOIS

#### Properties

- [OpenAPI](openapi/whoisfreaks-whois-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/whoisfreaks-whois-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/whoisfreaks-whois-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Documentation](https://whoisfreaks.com/documentation/whois-api)
- [API Reference](https://whoisfreaks.com/documentation)
- [Postman Collection](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [L L M S Txt](https://whoisfreaks.com/llms.txt)

## Common Properties

- [Overlay](overlays/whoisfreaks-openapi-overlay.yaml)
- [Developer Portal](https://whoisfreaks.com/documentation)
- [Documentation](https://whoisfreaks.com/documentation)
- [API Reference](https://whoisfreaks.com/documentation/whois-api)
- [Getting Started](https://whoisfreaks.com/integrations/sdk/python)
- [Support](https://whoisfreaks.com/contact)
- [Blog](https://whoisfreaks.com/resources/blog)
- [GitHub Organization](https://github.com/WhoisFreaks)
- [Pricing](https://whoisfreaks.com/pricing)
- [Sign Up](https://whoisfreaks.com/signup)
- [Login](https://whoisfreaks.com/login)
- [Terms of Service](https://whoisfreaks.com/terms)
- [Privacy Policy](https://whoisfreaks.com/privacy-policy)
- [Postman](https://www.postman.com/wf-official/api) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Status Page](https://whoisfreaks.com/uptime-status)
- [Lifecycle](lifecycle/whoisfreaks-lifecycle.yml)
- [Authentication](authentication/whoisfreaks-authentication.yml)
- [Conventions](conventions/whoisfreaks-conventions.yml)
- [Rate Limits](rate-limits/whoisfreaks-rate-limits.yml)
- [Plans](plans/whoisfreaks-plans.yml)
- [Error Catalog](errors/whoisfreaks-problem-types.yml)
- [Examples](examples/whoisfreaks-code-examples.yml)
- [Packages](packages/whoisfreaks-packages.yml)
- [S D Ks](packages/whoisfreaks-packages.yml)
- [C L I](cli/whoisfreaks-cli.yml)
- [Console](sandbox/whoisfreaks-sandbox.yml)
- [Webhooks](asyncapi/whoisfreaks-monitoring-webhooks.yml)
- [Agent Skill](skills/_index.yml)
- [L L Ms Txt](llms/whoisfreaks-llms.txt)
- [Well Known](well-known/whoisfreaks-well-known.yml)
- [Conformance](conformance/whoisfreaks-conformance.yml)
- [Data Model](data-model/whoisfreaks-data-model.yml)
- [Domain Security](security/whoisfreaks-domain-security.yml)
- [Compliance](https://whoisfreaks.com/privacy-policy)
- [Changelog](changelog/whoisfreaks-changelog.yml)

## Maintainers

**FN:** WhoisFreaks
**Email:** support@whoisfreaks.com
**URL:** https://whoisfreaks.com
