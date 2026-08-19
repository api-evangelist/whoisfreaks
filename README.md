# WhoisFreaks (whoisfreaks)

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
