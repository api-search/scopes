---
api_specs:
- filename: fortellis-appointments-openapi.yml
  format: yaml
  label: Fortellis Service Appointments API
  slug: fortellis-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-appointments-openapi.yml
- filename: fortellis-user-service-openapi.yml
  format: yaml
  label: Fortellis User / Booking Sessions API
  slug: fortellis-user-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-user-service-openapi.yml
- filename: fortellis-parts-store-openapi.yml
  format: yaml
  label: Fortellis Parts Store API
  slug: fortellis-parts-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-parts-store-openapi.yml
- filename: fortellis-pet-adoption-openapi.yml
  format: yaml
  label: Fortellis Reference Pet Adoption API
  slug: fortellis-pet-adoption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-pet-adoption-openapi.yml
- filename: fortellis-event-relay-webhook-openapi.yml
  format: yaml
  label: Fortellis Event Relay Webhook
  slug: fortellis-event-relay-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/openapi/fortellis-event-relay-webhook-openapi.yml
- filename: fortellis-event-relay-data-plane-proxy-asyncapi.yml
  format: yaml
  label: Fortellis Event Relay Data Plane Proxy (AsyncAPI)
  slug: fortellis-event-relay-data-plane
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-event-relay-data-plane-proxy-asyncapi.yml
- filename: fortellis-hello-world-asyncapi.yml
  format: yaml
  label: Fortellis AsyncAPI Hello World Reference
  slug: fortellis-async-hello-world
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/asyncapi/fortellis-hello-world-asyncapi.yml
authorization_urls:
- https://identity.fortellis.io/oauth2/
description: ''
docs: ''
flows:
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Cdk Global Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CDK Global publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CDK Global API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CDK Global
provider_slug: cdk-global
schemes:
- flows:
  - authorizationUrl: https://identity.fortellis.io/oauth2/
    flow: implicit
  name: permission-model
  source: openapi/fortellis-appointments-openapi.yml
- flows:
  - authorizationUrl: https://identity.fortellis.io/oauth2/
    flow: implicit
  name: permission-model
  source: openapi/fortellis-parts-store-openapi.yml
- flows:
  - authorizationUrl: https://identity.fortellis.io/oauth2/
    flow: implicit
  name: permission-model
  source: openapi/fortellis-pet-adoption-openapi.yml
- flows:
  - authorizationUrl: https://identity.fortellis.io/oauth2/
    flow: implicit
  name: permission-model
  source: openapi/fortellis-user-service-openapi.yml
scope_count: 3
scope_names:
- anonymous
- pets.adopt
- pets.manage
scopes:
- description: Create, Query, Update, and Delete appointments
  flows:
  - implicit
  scope: anonymous
- description: permission to query, read, and adopt pets
  flows:
  - implicit
  scope: pets.adopt
- description: permission to add, modify, and remove pets
  flows:
  - implicit
  scope: pets.manage
slug: cdk-global-scopes
source_filename: cdk-global-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fortellis-appointments-openapi.yml, openapi/fortellis-parts-store-openapi.yml,\n  openapi/fortellis-pet-adoption-openapi.yml, openapi/fortellis-user-service-openapi.yml\nschemes:\n- name: permission-model\n  source: openapi/fortellis-appointments-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://identity.fortellis.io/oauth2/\n- name: permission-model\n  source: openapi/fortellis-parts-store-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://identity.fortellis.io/oauth2/\n- name: permission-model\n  source: openapi/fortellis-pet-adoption-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://identity.fortellis.io/oauth2/\n- name: permission-model\n  source: openapi/fortellis-user-service-openapi.yml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://identity.fortellis.io/oauth2/\nscopes:\n- scope: anonymous\n  description: Create, Query, Update,\
  \ and Delete appointments\n  flows:\n  - implicit\n  sources:\n  - openapi/fortellis-appointments-openapi.yml\n  - openapi/fortellis-parts-store-openapi.yml\n  - openapi/fortellis-pet-adoption-openapi.yml\n  - openapi/fortellis-user-service-openapi.yml\n- scope: pets.adopt\n  description: permission to query, read, and adopt pets\n  flows:\n  - implicit\n  sources:\n  - openapi/fortellis-pet-adoption-openapi.yml\n- scope: pets.manage\n  description: permission to add, modify, and remove pets\n  flows:\n  - implicit\n  sources:\n  - openapi/fortellis-pet-adoption-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdk-global/refs/heads/main/scopes/cdk-global-scopes.yml
summary_line: 3 scopes · implicit
tags:
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
token_urls: []
---
