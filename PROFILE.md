# WhoisFreaks

Domain and IP intelligence provider offering WHOIS, DNS, IP geolocation/security, SSL, subdomain, and domain availability REST APIs, downloadable databases, monitoring services, and an official MCP server.

- **Provider:** https://whoisfreaks.com
- **Documentation:** https://whoisfreaks.com/documentation
- **Base URL:** https://api.whoisfreaks.com/ (bulk downloads: https://files.whoisfreaks.com/)
- **Tags:** WHOIS, DNS, Domain Intelligence, IP Intelligence / Geolocation, Cybersecurity / Threat Intelligence, OSINT, Reverse Lookup, SSL/Certificate, Domain Monitoring, Brand Protection
- **Public API:** yes
- **OpenAPI:** yes — 3.0.3, 57 paths / 60 operations / 78 schemas
- **Agent-native (MCP / llms.txt / skills):** yes

## APIs

- **WhoisFreaks API** — REST (JSON/XML) for Live WHOIS, WHOIS History, Bulk/Reverse WHOIS, IP/ASN WHOIS, live/historical/reverse DNS, Domain Availability, Typosquatting, IP Geolocation, IP Reputation, Domain Reputation, SSL, Subdomains, account utilities, and bulk database/threat-feed downloads. (`https://api.whoisfreaks.com`)
- **WhoisFreaks MCP Server** — official open-source Java MCP server exposing 14 domain-intelligence tools. (`https://github.com/WhoisFreaks/whoisfreaks-mcp-server`)

## Contract discovery — 2026-08-09

The earlier note on this profile said "no OpenAPI/AsyncAPI/GraphQL spec was found". That was wrong, and it is corrected here. A real OpenAPI **3.0.3** document — 57 paths, 60 operations, 78 component schemas — is published at
`https://raw.githubusercontent.com/WhoisFreaks/wf-sdks-docs/main/spec/whoisfreaks-openapi.yaml`
and is the source all ten official SDKs are generated from. It is not linked from the docs site and does not sit at any conventional spec path: `api.whoisfreaks.com/openapi.json|swagger.json|api-docs|docs|redoc` all return 404, and `whoisfreaks.com/openapi.json` returns the Next.js HTML 404 shell. It was found by inspecting the SDK repositories, which carry `.openapi-generator/` markers. The spec is saved verbatim to `openapi/whoisfreaks-openapi-original.yml`.

## What is published

- **OpenAPI 3.0.3**, 60 operations, apiKey-in-query auth (`openapi/`)
- **Ten official SDKs** — Python, JavaScript, TypeScript, Java, Kotlin, C#, Go, Ruby, Swift, PHP, all generated from one spec and released in lockstep at 0.21.0 (`packages/`)
- **610 runnable code examples** — one per endpoint per language (`examples/`)
- **Go CLI** with flag-based WHOIS/DNS/SSL/availability modes (`cli/`)
- **MCP server** — 14 tools, stdio + HTTP/SSE, Docker image `whoisfreaks/mcp-server` (`mcp/`), fully crosswalked to REST operationIds (`mcp/whoisfreaks-tool-crosswalk.yml`)
- **llms.txt** — 173 lines, regenerated 2026-08-07 (`llms/`)
- **Public Postman collection** — 48 requests across 23 folders
- **Error reference**, **rate-limiting reference** with three `x-ratelimit-*` headers, **status page**, **99.99% uptime commitment** in the Terms
- **n8n node**, Splunk/Pi-hole/BIND9/Zeek/Suricata/AdGuard/Rspamd/SpamAssassin integrations, MS Security Copilot plugin

## What is missing

- No `/.well-known/` documents at all — no `security.txt`, no `api-catalog`, no agent card (all 404 on both hosts)
- No RFC 9457 problem+json; 44 of 60 operations declare only a bodyless `4XX`
- No idempotency contract, no request-id header, no cursor pagination
- No API changelog, no deprecation/sunset policy, no roadmap
- No vulnerability-disclosure program, no bug bounty, no trust center, no third-party certifications (GDPR is self-asserted)
- API key travels as a URL query parameter with no header alternative and no scoping
- No AsyncAPI; webhook alerts are advertised on the Brand Monitoring page with no payload schema
- MCP covers only 14 of 60 operations — no bulk, database, threat-feed or account tools

_Enriched by the API Evangelist enrichment pipeline, 2026-08-09._
