# Tropic

Tropic is an intelligent procurement platform that combines AI-powered spend management, supplier management, and benchmark data to help organizations find and capture savings opportunities. Tropic's AI agents track renewals, spot shadow spend, flag compliance issues, and automate manual procurement tasks with SKU-level price benchmarks from thousands of actual deals.

**URL:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/tropic/refs/heads/main/apis.yml)

## APIs

### Tropic API

The Tropic public REST API enables organizations to connect Tropic with other software in their stack, managing contracts, suppliers, procurement requests, webhooks, and users programmatically.

- **Base URL:** `https://api.tropicapp.io/v1`
- **Authentication:** Bearer token (API key from Tropic settings)
- **Documentation:** [API and Webhooks](https://help.tropicapp.io/hc/en-us/sections/31190632406171-API-and-Webhooks)

**Key Endpoints:**
- `GET/POST /contracts` — List and create contracts
- `GET/PUT/DELETE /contracts/{id}` — Manage individual contracts
- `GET/POST /suppliers` — List and create supplier profiles
- `GET/PUT /suppliers/{id}` — Manage individual suppliers
- `GET/POST /requests` — List and submit procurement requests
- `POST /requests/{id}/approve` — Approve a request
- `POST /requests/{id}/reject` — Reject a request
- `GET/POST /webhooks` — Manage webhook subscriptions
- `GET /users` — List organization users

## Artifacts

| Type | File |
|---|---|
| OpenAPI Spec | [openapi/tropic-openapi.yml](openapi/tropic-openapi.yml) |
| Spectral Rules | [rules/tropic-rules.yml](rules/tropic-rules.yml) |
| Naftiko Capabilities | [capabilities/procurement-management.yaml](capabilities/procurement-management.yaml) |
| Shared Capability | [capabilities/shared/tropic-api.yaml](capabilities/shared/tropic-api.yaml) |
| Contract JSON Schema | [json-schema/tropic-contract-schema.json](json-schema/tropic-contract-schema.json) |
| Supplier JSON Schema | [json-schema/tropic-supplier-schema.json](json-schema/tropic-supplier-schema.json) |
| Contract Structure | [json-structure/tropic-contract-structure.json](json-structure/tropic-contract-structure.json) |
| Supplier Structure | [json-structure/tropic-supplier-structure.json](json-structure/tropic-supplier-structure.json) |
| JSON-LD Context | [json-ld/tropic-context.jsonld](json-ld/tropic-context.jsonld) |
| Examples | [examples/](examples/) |
| Vocabulary | [vocabulary/tropic-vocabulary.yml](vocabulary/tropic-vocabulary.yml) |

## Capabilities

### Procurement Management (`capabilities/procurement-management.yaml`)

Workflow capability for managing the full procurement lifecycle — from intake and request approval through contract execution and supplier management. Used by procurement teams, finance managers, and operations leads.

- **REST port:** 8080
- **MCP port:** 9090
- **Tools:** 14 tools covering contracts, suppliers, requests, approvals, and webhooks

## Tags

- Benchmarking
- Contract Management
- Cost Optimization
- Procurement
- Renewals
- SaaS Management
- Spend Management
- Supplier Management

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-03

## Maintainers

**FN:** Kin Lane  
**Email:** kin@apievangelist.com
