---
api_specs:
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Contacts API
  slug: propertyme-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Properties API
  slug: propertyme-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Tenancies API
  slug: propertyme-tenancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Inspections API
  slug: propertyme-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Job Tasks API
  slug: propertyme-job-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Tasks API
  slug: propertyme-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Bills API
  slug: propertyme-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Dashboards API
  slug: propertyme-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Documents and Images API
  slug: propertyme-documents-and-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Members API
  slug: propertyme-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Portfolio Connection API
  slug: propertyme-portfolio-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
authorization_urls:
- https://login.propertyme.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- ciba
kind: oauth-scopes
layout: scope
method: searched
name: Propertyme Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PropertyMe publishes 20 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and ciba flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PropertyMe API on a user''s behalf.


  Tokens are issued from https://login.propertyme.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PropertyMe
provider_slug: propertyme
schemes:
- flows:
  - authorizationUrl: https://login.propertyme.com/connect/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://login.propertyme.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://login.propertyme.com/connect/token
  - deviceAuthorizationUrl: https://login.propertyme.com/connect/deviceauthorization
    flow: deviceCode
  - backchannelAuthenticationUrl: https://login.propertyme.com/connect/ciba
    flow: ciba
  name: OIDC
  source: https://login.propertyme.com/.well-known/openid-configuration
scope_count: 20
scope_names:
- openid
- profile
- email
- offline_access
- property:read
- property:write
- contact:read
- contact:write
- activity:read
- activity:write
- transaction:read
- transaction:write
- communication:read
- communication:write
- tenancy:write
- customer:read
- customer:write
- form:write
- ids:admin
- org-portal:api
scopes:
- description: Standard OIDC scope — issue an id_token identifying the signed-in PropertyMe user.
  flows: []
  scope: openid
- description: Standard OIDC scope — name, preferred_username, picture, locale and related profile claims.
  flows: []
  scope: profile
- description: Standard OIDC scope — email and email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh_token so an integration can keep polling a portfolio without re-consent.
  flows: []
  scope: offline_access
- description: Read lots (properties), tenancies and tenancy balances in the connected portfolio — including the rentals, active sales, vacancy and archived filters and the lot detail record.
  flows: []
  scope: property:read
- description: Attach comments and documents to a lot, an owner folio or a tenant folio.
  flows: []
  scope: property:write
- description: Read owners, tenants, suppliers, ownerships, the agency contact, contact alerts, contact images and the agency member directory.
  flows: []
  scope: contact:read
- description: Attach comments and documents to a contact.
  flows: []
  scope: contact:write
- description: Read inspections, job tasks (maintenance work orders, v1 and v2), general tasks, their quotations, documents, images and assigned managers, plus the activity dashboards.
  flows: []
  scope: activity:read
- description: Create and update inspections, job tasks and tasks, and drive their state machines — schedule, reschedule, inspect, close, reopen for inspections; approve, assign, complete, reject, reopen for jobs — plus quotations and attachments. The largest write surface in the contract.
  flows: []
  scope: activity:write
- description: Read the transaction dashboard aggregate over the trust ledger.
  flows: []
  scope: transaction:read
- description: Create a bill against the trust accounting ledger (POST /v1/bills). The only transaction-writing operation in the published contract.
  flows: []
  scope: transaction:write
- description: Read the communications dashboard aggregate.
  flows: []
  scope: communication:read
- description: Advertised by the identity provider; no published operation requires it.
  flows: []
  scope: communication:write
- description: Advertised by the identity provider; no published operation requires it. Tenancies are read-only in the public contract.
  flows: []
  scope: tenancy:write
- description: Advertised by the identity provider; no published operation requires it.
  flows: []
  scope: customer:read
- description: Advertised by the identity provider; no published operation requires it.
  flows: []
  scope: customer:write
- description: Advertised by the identity provider; no published operation requires it.
  flows: []
  scope: form:write
- description: Identity-server administration scope. Advertised by the identity provider; not part of the public integration surface.
  flows: []
  scope: ids:admin
- description: Organisation portal API scope. Advertised by the identity provider; no published operation requires it.
  flows: []
  scope: org-portal:api
slug: propertyme-scopes
source_filename: propertyme-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://login.propertyme.com/.well-known/openid-configuration\nsupplemental_source: openapi/propertyme-openapi.json\nnotes: >-\n  PropertyMe's Swagger 2.0 document declares only a single apiKey-style `Bearer` security definition,\n  so an OpenAPI-only derivation yields zero scopes — the mechanical derive pass found none. The real\n  scope surface is published anonymously in two places instead: the `scopes_supported` array of the\n  OpenID Connect discovery document at login.propertyme.com, and the prose of every operation\n  description in the contract (\"The auth token must contain a scope of property:read.\"). This file\n  reconciles both: `scopes[]` is the authoritative advertised list, and `operations` counts how many\n  of the 86 published operations actually require each scope. PropertyMe publishes no scope reference\n  page — there is no developer portal — so the discovery document IS the reference. Eight advertised\n\
  \  scopes are never exercised by any published operation; they belong to surfaces PropertyMe has not\n  exposed in the public contract (org portal, forms, customer administration, messaging writes).\nauthorization_endpoint: https://login.propertyme.com/connect/authorize\ntoken_endpoint: https://login.propertyme.com/connect/token\nrevocation_endpoint: https://login.propertyme.com/connect/revocation\nintrospection_endpoint: https://login.propertyme.com/connect/introspect\nregistration_endpoint: https://login.propertyme.com/connect/dcr\nschemes:\n  - name: OIDC\n    source: https://login.propertyme.com/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.propertyme.com/connect/authorize\n        tokenUrl: https://login.propertyme.com/connect/token\n        pkce: [S256, plain]\n      - flow: clientCredentials\n        tokenUrl: https://login.propertyme.com/connect/token\n      - flow: deviceCode\n        deviceAuthorizationUrl:\
  \ https://login.propertyme.com/connect/deviceauthorization\n      - flow: ciba\n        backchannelAuthenticationUrl: https://login.propertyme.com/connect/ciba\nscopes:\n  - scope: openid\n    description: Standard OIDC scope — issue an id_token identifying the signed-in PropertyMe user.\n    category: identity\n    operations: 0\n  - scope: profile\n    description: Standard OIDC scope — name, preferred_username, picture, locale and related profile claims.\n    category: identity\n    operations: 0\n  - scope: email\n    description: Standard OIDC scope — email and email_verified claims.\n    category: identity\n    operations: 0\n  - scope: offline_access\n    description: Issue a refresh_token so an integration can keep polling a portfolio without re-consent.\n    category: identity\n    operations: 0\n  - scope: property:read\n    description: >-\n      Read lots (properties), tenancies and tenancy balances in the connected portfolio — including the\n      rentals, active sales, vacancy\
  \ and archived filters and the lot detail record.\n    category: property\n    operations: 14\n  - scope: property:write\n    description: Attach comments and documents to a lot, an owner folio or a tenant folio.\n    category: property\n    operations: 3\n  - scope: contact:read\n    description: >-\n      Read owners, tenants, suppliers, ownerships, the agency contact, contact alerts, contact images\n      and the agency member directory.\n    category: contact\n    operations: 9\n  - scope: contact:write\n    description: Attach comments and documents to a contact.\n    category: contact\n    operations: 2\n  - scope: activity:read\n    description: >-\n      Read inspections, job tasks (maintenance work orders, v1 and v2), general tasks, their quotations,\n      documents, images and assigned managers, plus the activity dashboards.\n    category: activity\n    operations: 23\n  - scope: activity:write\n    description: >-\n      Create and update inspections, job tasks and tasks, and\
  \ drive their state machines — schedule,\n      reschedule, inspect, close, reopen for inspections; approve, assign, complete, reject, reopen for\n      jobs — plus quotations and attachments. The largest write surface in the contract.\n    category: activity\n    operations: 22\n  - scope: transaction:read\n    description: Read the transaction dashboard aggregate over the trust ledger.\n    category: transaction\n    operations: 1\n  - scope: transaction:write\n    description: >-\n      Create a bill against the trust accounting ledger (POST /v1/bills). The only transaction-writing\n      operation in the published contract.\n    category: transaction\n    operations: 1\n  - scope: communication:read\n    description: Read the communications dashboard aggregate.\n    category: communication\n    operations: 1\n  - scope: communication:write\n    description: Advertised by the identity provider; no published operation requires it.\n    category: communication\n    operations: 0\n  -\
  \ scope: tenancy:write\n    description: >-\n      Advertised by the identity provider; no published operation requires it. Tenancies are read-only\n      in the public contract.\n    category: property\n    operations: 0\n  - scope: customer:read\n    description: Advertised by the identity provider; no published operation requires it.\n    category: customer\n    operations: 0\n  - scope: customer:write\n    description: Advertised by the identity provider; no published operation requires it.\n    category: customer\n    operations: 0\n  - scope: form:write\n    description: Advertised by the identity provider; no published operation requires it.\n    category: forms\n    operations: 0\n  - scope: ids:admin\n    description: >-\n      Identity-server administration scope. Advertised by the identity provider; not part of the public\n      integration surface.\n    category: administration\n    operations: 0\n  - scope: org-portal:api\n    description: >-\n      Organisation portal API\
  \ scope. Advertised by the identity provider; no published operation\n      requires it.\n    category: administration\n    operations: 0\nunscoped_operations:\n  count: 10\n  note: >-\n    Ten published operations carry no scope sentence in their description — DELETE\n    /v1/portfolios/disconnect (the consent seam, which the docs say invalidates the current access\n    token) plus nine job-task and attachment writes that in practice sit under activity:write. Recorded\n    as a documentation gap in the contract, not as unauthenticated access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/scopes/propertyme-scopes.yml
summary_line: 20 scopes · authorizationCode/clientCredentials/deviceCode/ciba
tags:
- Real Estate
- Australia
- Property Management
- Rentals
- PropTech
- Tenancy
- Trust Accounting
- Inspections
- Maintenance
- Documents
- Payments
- New Zealand
token_urls:
- https://login.propertyme.com/connect/token
---
