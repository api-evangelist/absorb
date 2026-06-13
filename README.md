# Absorb LMS

Absorb LMS is a cloud-based learning management system with a REST API for managing learners, courses, certificates, departments, enrollments, and tracking e-learning completion data.

## APIs

- **Integration API** - REST-based interface for integrating external systems with Absorb LMS. Covers users, enrollments, courses, certificates, departments, learning paths, and more.
- **SCIM API** - SCIM 2.0 standard implementation for automated user and group provisioning.
- **Infuse API** - Headless LMS embedding for integrating Absorb learning experiences into external applications (paid add-on).

## Documentation

- [API Documentation](https://docs.myabsorb.com/)
- [Integration API v2 Reference](https://docs.myabsorb.com/integration-api/v2/docs)
- [Getting Started Guide](https://support.absorblms.com/hc/en-us/articles/222482188-Getting-Started-with-the-Absorb-Integration-API)
- [API Changelog](https://support.absorblms.com/hc/en-us/articles/22151754631955-Integration-API-Change-Log)
- [API Glossary](https://support.absorblms.com/hc/en-us/articles/26898046456467-Integration-API-Glossary)
- [Help Center](https://support.absorblms.com/hc/en-us)
- [Blog](https://www.absorblms.com/blog)

## Authentication

The Integration API supports:

- **OAuth 2.0** (recommended) - Supports on-behalf-of flows for requesting tokens on behalf of other users.
- **Private API Key** - Required `X-API-Key` header obtained from portal settings.
- **Basic Method** - `/authenticate` endpoint returning a Bearer token valid for four hours.

## Base URLs

| Region | Production | Sandbox |
|--------|-----------|---------|
| US | `https://rest.myabsorb.com` | `https://rest.sandbox.myabsorb.com` |
| EU | `https://rest.myabsorb.eu` | `https://rest.sandbox.myabsorb.eu` |
| AU | `https://rest.myabsorb.com.au` | `https://rest.sandbox.myabsorb.com.au` |
| CA | `https://rest.myabsorb.ca` | `https://rest.sandbox.myabsorb.ca` |

## Rate Limits

- 200 requests per second standard limit
- 100 additional burst requests above the standard limit
- HTTP 429 returned when exceeded; implement exponential backoff

## Pricing

Absorb LMS uses a per-active-learner pricing model with custom quotes. No public list pricing is available. Contact [sales](https://www.absorblms.com/contact) for a quote.

## Maintainer

**Kin Lane** - kin@apievangelist.com
