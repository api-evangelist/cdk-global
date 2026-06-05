# CDK Global (cdk-global)

CDK Global is the dominant U.S. dealer management system (DMS) provider, serving roughly 15,000 automotive dealerships with software covering sales, F&I, fixed operations, parts, CRM, and digital retail. CDK was spun out of ADP in 2014 and acquired by Brookfield Business Partners in July 2022 for $8.3B (taken private). The company operates the Fortellis platform — a developer marketplace and integration hub with 135+ published APIs, 425+ marketplace apps, 82,000+ dealer integrations, and 6.7B+ API transactions per year — exposing CDK DMS data to ISVs, OEMs, and third-party automotive systems. CDK suffered a major BlackSuit ransomware attack on June 19, 2024, paying ~$25M in bitcoin to restore service over roughly two weeks; the outage caused an estimated $605M in dealer losses and triggered numerous lawsuits.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cdk-global/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cdk-global/main/apis.yml)

## Tags

- Automotive
- Dealer Management
- DMS
- Auto Retail
- F&I
- Fixed Operations
- Parts
- CRM
- Digital Retail
- Marketplace
- Developer Platform
- Events
- Webhooks
- AsyncAPI

## Timestamps

- **Created:** 2026-05-22
- **Modified:** 2026-05-23

## APIs

### Fortellis Platform

Fortellis is CDK Global's open automotive commerce platform — an API gateway, app marketplace, and developer community that brokers data flow between dealerships, ISVs, OEMs, heavy-truck, and powersports systems. Fortellis publishes 135+ APIs, lists 425+ marketplace apps, and processes 6.7B+ API transactions per year across 82K+ dealer integrations.

- **Human URL:** [https://fortellis.io](https://fortellis.io)
- **Base URL:** `https://api.fortellis.io`

#### Tags

- Fortellis
- Marketplace
- Developer Platform
- APIs
- Automotive

#### Properties

- [Documentation](https://docs.fortellis.io)
- [API Reference](https://apidocs.fortellis.io)
- [Sign Up](https://sso.fortellis.io)
- [Portal](https://fortellis.io)
- [Community](https://fortellis.io/community)
- [Marketplace](https://fortellis.io/marketplace)
- [GitHub Organization](https://github.com/Fortellis)
- [Postman Collection](collections/fortellis-appointments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-appointments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-event-relay-webhook.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-event-relay-webhook.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-parts-store.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-parts-store.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-pet-adoption.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-pet-adoption.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-user-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-user-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fortellis Service Appointments API

Service-appointments API for booking, querying, updating, and cancelling vehicle service appointments at a dealership service department. Used by scheduling systems integrating with CDK and other DMS providers via Fortellis.

- **Human URL:** [https://apidocs.fortellis.io](https://apidocs.fortellis.io)
- **Base URL:** `https://api.fortellis.io/sales/notification/v3`

#### Tags

- Appointments
- Service
- Fixed Operations
- Scheduling

#### Properties

- [OpenAPI](openapi/fortellis-appointments-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fortellis-appointments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-appointments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://apidocs.fortellis.io)
- [Source Repo](https://github.com/Fortellis/example-spec)

### Fortellis User / Booking Sessions API

Booking-sessions API illustrating Fortellis's REST conventions: session creation, item management, store availability, and slot reservation for service scheduling workflows.

- **Human URL:** [https://apidocs.fortellis.io](https://apidocs.fortellis.io)
- **Base URL:** `https://api.fortellis.io/service/sessions/v4`

#### Tags

- Booking Sessions
- Service
- Scheduling

#### Properties

- [OpenAPI](openapi/fortellis-user-service-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fortellis-user-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-user-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://apidocs.fortellis.io)
- [Source Repo](https://github.com/Fortellis/example-spec)

### Fortellis Parts Store API

Parts-store reference API exposing product info, sizing, and ping/health for dealership parts inventory and procurement integrations.

- **Human URL:** [https://apidocs.fortellis.io](https://apidocs.fortellis.io)
- **Base URL:** `https://api.fortellis.io/sales/parts-store/v47`

#### Tags

- Parts
- Inventory
- Fixed Operations

#### Properties

- [OpenAPI](openapi/fortellis-parts-store-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fortellis-parts-store.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-parts-store.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://apidocs.fortellis.io)
- [Source Repo](https://github.com/Fortellis/example-spec)

### Fortellis Reference Pet Adoption API

Reference / tutorial API distributed by Fortellis for developers learning the platform's OpenAPI conventions, OAuth flows, and admin-API patterns.

- **Human URL:** [https://apidocs.fortellis.io](https://apidocs.fortellis.io)
- **Base URL:** `https://api.fortellis.io/data/v1/example/pet-adoption`

#### Tags

- Reference
- Tutorial
- Developer Education

#### Properties

- [OpenAPI](openapi/fortellis-pet-adoption-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fortellis-pet-adoption.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-pet-adoption.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Source Repo](https://github.com/Fortellis/example-spec)

### Fortellis Event Relay Webhook

Webhook contract that event-sink applications implement to receive asynchronous events from Fortellis Event Relay. Defines payload envelope, required headers (X-Request-Id, Fortellis-Event-Id, Authorization, Data-Owner-Id), and retry semantics for guaranteed delivery.

- **Human URL:** [https://github.com/Fortellis/Fortellis-Event-Relay-Webhook](https://github.com/Fortellis/Fortellis-Event-Relay-Webhook)
- **Base URL:** `https://api.fortellis.io/v1/webhook`

#### Tags

- Events
- Webhooks
- Event Relay
- Asynchronous

#### Properties

- [OpenAPI](openapi/fortellis-event-relay-webhook-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fortellis-event-relay-webhook.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-event-relay-webhook.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Source Repo](https://github.com/Fortellis/Fortellis-Event-Relay-Webhook)

### Fortellis Event Relay Data Plane Proxy (AsyncAPI)

AsyncAPI specification for the Fortellis Event Relay data-plane proxy used by event sources to publish events into Fortellis for fan-out to subscribers.

- **Human URL:** [https://github.com/Fortellis/Event-Relay-Specs](https://github.com/Fortellis/Event-Relay-Specs)

#### Tags

- Events
- AsyncAPI
- Event Relay
- Publish-Subscribe

#### Properties

- [AsyncAPI](asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Source Repo](https://github.com/Fortellis/Event-Relay-Specs)
- [Postman Collection](collections/fortellis-appointments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-appointments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-event-relay-webhook.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-event-relay-webhook.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-parts-store.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-parts-store.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-pet-adoption.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-pet-adoption.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-user-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-user-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Fortellis AsyncAPI Hello World Reference

Hello World AsyncAPI reference distributed by Fortellis to teach the asynchronous API pattern, channel topology, and message envelope conventions used across Fortellis event APIs.

- **Human URL:** [https://github.com/Fortellis/AsyncAPIHelloWorld](https://github.com/Fortellis/AsyncAPIHelloWorld)

#### Tags

- AsyncAPI
- Reference
- Events
- Developer Education

#### Properties

- [AsyncAPI](asyncapi/fortellis-hello-world-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Source Repo](https://github.com/Fortellis/AsyncAPIHelloWorld)
- [Postman Collection](collections/fortellis-appointments.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-appointments.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-event-relay-webhook.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-event-relay-webhook.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-parts-store.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-parts-store.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-pet-adoption.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-pet-adoption.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/fortellis-user-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fortellis-user-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Website](https://www.cdkglobal.com)
- [Portal](https://fortellis.io)
- [Documentation](https://docs.fortellis.io)
- [API Reference](https://apidocs.fortellis.io)
- [Sign Up](https://sso.fortellis.io)
- [Marketplace](https://fortellis.io/marketplace)
- [Community](https://fortellis.io/community)
- [Authentication](https://identity.fortellis.io/oauth2/)
- [GitHub Organization](https://github.com/Fortellis)
- [SDK](https://github.com/Fortellis/fortellis-cli)
- [C L I](https://www.npmjs.com/package/@fortellis/fortellis-cli)
- [V S Code Extension](https://github.com/Fortellis/vscode-fortellis-spec-tools)
- [Git Hub Action](https://github.com/Fortellis/api-spec-lint-action)
- [Git Hub Action](https://github.com/Fortellis/api-spec-push-action)
- [Spec Linter](https://github.com/Fortellis/fortellis-spec-linter)
- [SDK](https://github.com/Fortellis/python-admin-api)
- [SDK](https://github.com/Fortellis/Admin-API-Implementation-Java)
- [SDK](https://github.com/Fortellis/admin-api-implementation)
- [Sample](https://github.com/Fortellis/Java-Public-Webhook-Example)
- [Sample](https://github.com/Fortellis/AuthorizationCodeFlowInDotNet)
- [Sample](https://github.com/Fortellis/ImplicitFlowInDotNet)
- [Sample](https://github.com/Fortellis/ClientCredentialsFlowIn.Net)
- [LinkedIn](https://www.linkedin.com/company/cdk-global)
- [Twitter](https://twitter.com/cdkglobal)
- [Plans](plans/cdk-global-plans-pricing.yml)
- [Rate Limits](rate-limits/cdk-global-rate-limits.yml)
- [Fin Ops](finops/cdk-global-finops.yml)
- [Vocabulary](vocabulary/cdk-global-vocabulary.yml)
- [J S O N L D Context](json-ld/cdk-global-context.jsonld)
- [Spectral Rules](rules/fortellis-rules.yml)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
