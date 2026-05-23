# cdk-global

API Evangelist profile for **CDK Global** — the dominant U.S. dealer management system (DMS)
provider, serving roughly 15,000 automotive dealerships across the U.S. and Canada with sales,
F&I, fixed operations, parts, CRM, and digital-retail software. CDK was spun out of ADP in 2014
and acquired by **Brookfield Business Partners in July 2022 for $8.3B**, taking the company
private. The real developer surface lives on **Fortellis** — CDK's API gateway, app marketplace,
and developer community for the automotive ecosystem.

On **June 19, 2024**, CDK was hit by a **BlackSuit ransomware attack** that took most of its
services offline. Roughly **15,000 dealerships were disrupted**, CDK paid an estimated **$25M
ransom in bitcoin**, and the outage caused approximately **$605M in dealer losses** in the first
two weeks. Most dealers were restored by July 4, 2024. The incident is the largest disruption to
U.S. automotive retail technology in recent memory and reframes any FinOps or vendor-risk view
of CDK.

## Fortellis at a glance

- **135+** published APIs
- **425+** apps in the Fortellis Marketplace
- **82,000+** dealer integrations
- **6.7B+** API transactions per year
- Ecosystem covers Dealers, ISVs, OEMs, Heavy Truck, and Powersports

## What this repo contains

This is a full pipeline run — the canonical API Evangelist profile of CDK Global / Fortellis,
covering the published API surface, integration patterns (synchronous APIs, AsyncAPI, Event Relay
webhooks), Naftiko capabilities, schemas, examples, plans, rate limits, and FinOps.

### Folders

| Folder | Purpose |
|---|---|
| `openapi/` | OpenAPI 2.0 / 3.0 specs from the Fortellis [`example-spec`](https://github.com/Fortellis/example-spec) and [`Fortellis-Event-Relay-Webhook`](https://github.com/Fortellis/Fortellis-Event-Relay-Webhook) reference repos |
| `asyncapi/` | AsyncAPI specs from [`AsyncAPIHelloWorld`](https://github.com/Fortellis/AsyncAPIHelloWorld) and [`Event-Relay-Specs`](https://github.com/Fortellis/Event-Relay-Specs) |
| `capabilities/` | Naftiko capability definitions, one per Fortellis API surface |
| `rules/` | Spectral ruleset enforcing Fortellis OpenAPI conventions (versioned basePath, OAuth on identity.fortellis.io, camelCase operationIds, Event-Relay header requirements) |
| `json-schema/` | JSON Schemas for Fortellis entities (Service Appointment, Booking Session, Part, Event, Marketplace App) |
| `json-structure/` | Field-level structure docs for the Service Appointment and Event payloads |
| `json-ld/` | JSON-LD context mapping Fortellis terms to schema.org |
| `examples/` | Request/response examples for the principal Fortellis operations + an Event Relay webhook delivery |
| `vocabulary/` | Term vocabulary spanning CDK DMS and the Fortellis platform |
| `plans/` | API Commons Plans 0.1 view of CDK DMS suites + Fortellis ISV / Dealer / OEM tiers |
| `rate-limits/` | API Commons Rate Limits 0.1 view (per-subscription gateway limits + Event Relay retry semantics) |
| `finops/` | FinOps Framework / FOCUS view (with explicit ransomware business-continuity risk line item) |

## APIs documented

| # | API | Folder |
|---|---|---|
| 1 | Fortellis Platform | meta |
| 2 | Fortellis Service Appointments | `openapi/fortellis-appointments-openapi.yml` |
| 3 | Fortellis Booking Sessions (User / Service) | `openapi/fortellis-user-service-openapi.yml` |
| 4 | Fortellis Parts Store | `openapi/fortellis-parts-store-openapi.yml` |
| 5 | Fortellis Pet Adoption (reference) | `openapi/fortellis-pet-adoption-openapi.yml` |
| 6 | Fortellis Event Relay Webhook | `openapi/fortellis-event-relay-webhook-openapi.yml` |
| 7 | Fortellis Event Relay Data Plane Proxy | `asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml` |
| 8 | Fortellis AsyncAPI Hello World | `asyncapi/fortellis-hello-world-asyncapi.yml` |

The full machine-readable inventory lives in `apis.yml`.

## Fortellis developer tooling (from the GitHub org)

The [`Fortellis`](https://github.com/Fortellis) GitHub org carries 50+ repos covering CLI,
spec linter, VS Code extension, GitHub Actions, and OAuth / Admin-API / webhook reference
implementations in **JavaScript, Python, Java, and .NET**:

- **CLI**: [`fortellis-cli`](https://github.com/Fortellis/fortellis-cli) — `npm install -g @fortellis/fortellis-cli` (init, configure, add, api-template, api-lint, status, push)
- **Linter**: [`fortellis-spec-linter`](https://github.com/Fortellis/fortellis-spec-linter)
- **VS Code**: [`vscode-fortellis-spec-tools`](https://github.com/Fortellis/vscode-fortellis-spec-tools)
- **GitHub Actions**: [`api-spec-lint-action`](https://github.com/Fortellis/api-spec-lint-action), [`api-spec-push-action`](https://github.com/Fortellis/api-spec-push-action)
- **Admin API reference**: [`admin-api-example`](https://github.com/Fortellis/admin-api-example) (.NET), [`python-admin-api`](https://github.com/Fortellis/python-admin-api), [`Admin-API-Implementation-Java`](https://github.com/Fortellis/Admin-API-Implementation-Java)
- **OAuth reference apps**: Authorization Code, Implicit, and Client Credentials flows in JS, Python, Java, and .NET
- **Event Relay**: [`Java-Public-Webhook-Example`](https://github.com/Fortellis/Java-Public-Webhook-Example), [`Fortellis-Event-Relay-Webhook`](https://github.com/Fortellis/Fortellis-Event-Relay-Webhook), [`Event-Relay-Specs`](https://github.com/Fortellis/Event-Relay-Specs)

## Notable absences

- Fortellis does **not** publish a public per-call rate card or per-tier rate-limit table — pricing and limits are negotiated per ISV / dealer / OEM subscription.
- `docs.fortellis.io`, `status.fortellis.io`, and `apidocs.fortellis.io` are client-side React apps that don't render content to plain HTML fetches — the OpenAPI surface had to be reconstructed from the GitHub `example-spec` and `Event-Relay-Specs` repos.
- No public StatusPage RSS / JSON feed was discoverable; uptime monitoring must be done externally.
- CDK Global itself (cdkglobal.com) is a marketing site — the API surface is all under Fortellis.
- Last activity on most Fortellis GitHub repos is 2022 — the platform is operational but the public developer-tooling repos appear relatively stable rather than active.

## Major event — June 2024 ransomware attack

| Field | Value |
|---|---|
| Date | June 19, 2024 |
| Recovery date | ~July 4, 2024 |
| Attributed to | BlackSuit (Eastern European / Russian operator) |
| Ransom paid | ~$25M USD (bitcoin) — paid June 21, 2024 |
| Dealers affected | ~15,000 across U.S. and Canada |
| Estimated dealer losses | ~$605M (first two weeks) |
| Outcome | Multiple negligence lawsuits filed against CDK |

The incident is captured as a first-class `x-incidents` entry in `apis.yml` and called out
explicitly in `finops/cdk-global-finops.yml` as a business-continuity FinOps risk.

## Pipeline

Run via the API Evangelist `run-pipeline` skill. To re-run:

```
cd /Users/kinlane/GitHub/all/cdk-global
# use Claude Code: /run-pipeline cdk-global
```

## License

Profile content is published under the same terms as the rest of the API Evangelist network.
Underlying Fortellis spec files come from the public [`Fortellis`](https://github.com/Fortellis)
GitHub organization and retain their original repository licenses.
