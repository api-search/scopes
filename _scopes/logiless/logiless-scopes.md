---
api_specs:
- filename: logiless-articles-api-openapi.yml
  format: yaml
  label: Logiless Articles API
  slug: logiless-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-articles-api-openapi.yml
- filename: logiless-inbound-deliveries-api-openapi.yml
  format: yaml
  label: Logiless Inbound Deliveries API
  slug: logiless-inbound-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inbound-deliveries-api-openapi.yml
- filename: logiless-inter-warehouse-transfers-api-openapi.yml
  format: yaml
  label: Logiless Inter-Warehouse Transfers API
  slug: logiless-inter-warehouse-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inter-warehouse-transfers-api-openapi.yml
- filename: logiless-inventory-api-openapi.yml
  format: yaml
  label: Logiless Inventory API
  slug: logiless-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-inventory-api-openapi.yml
- filename: logiless-locations-api-openapi.yml
  format: yaml
  label: Logiless Locations API
  slug: logiless-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-locations-api-openapi.yml
- filename: logiless-outbound-deliveries-api-openapi.yml
  format: yaml
  label: Logiless Outbound Deliveries API
  slug: logiless-outbound-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-outbound-deliveries-api-openapi.yml
- filename: logiless-sales-orders-api-openapi.yml
  format: yaml
  label: Logiless Sales Orders API
  slug: logiless-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-sales-orders-api-openapi.yml
- filename: logiless-sales-returns-api-openapi.yml
  format: yaml
  label: Logiless Sales Returns API
  slug: logiless-sales-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-sales-returns-api-openapi.yml
- filename: logiless-suppliers-api-openapi.yml
  format: yaml
  label: Logiless Suppliers API
  slug: logiless-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/openapi/logiless-suppliers-api-openapi.yml
authorization_urls:
- https://app2.logiless.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Logiless Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Logiless uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app2.logiless.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Logiless
provider_slug: logiless
schemes:
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-articles-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-inbound-deliveries-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-inter-warehouse-transfers-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-inventory-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-locations-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-outbound-deliveries-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-sales-orders-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-sales-returns-api-openapi.yml
- description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.
  flows:
  - authorizationUrl: https://app2.logiless.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://app2.logiless.com/oauth2/token
  name: oauth2
  source: openapi/logiless-suppliers-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: logiless-scopes
source_filename: logiless-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/logiless-articles-api-openapi.yml, openapi/logiless-inbound-deliveries-api-openapi.yml,\n  openapi/logiless-inter-warehouse-transfers-api-openapi.yml, openapi/logiless-inventory-api-openapi.yml,\n  openapi/logiless-locations-api-openapi.yml, openapi/logiless-outbound-deliveries-api-openapi.yml,\n  openapi/logiless-sales-orders-api-openapi.yml, openapi/logiless-sales-returns-api-openapi.yml,\n  openapi/logiless-suppliers-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/logiless-articles-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped\
  \ to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-inbound-deliveries-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-inter-warehouse-transfers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30\
  \ days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-inventory-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-locations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh\
  \ tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-outbound-deliveries-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-sales-orders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS\
  \ Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-sales-returns-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5 business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\n- name: oauth2\n  source: openapi/logiless-suppliers-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app2.logiless.com/oauth/v2/auth\n    tokenUrl: https://app2.logiless.com/oauth2/token\n  description: OAuth 2.0 authorization-code flow. Applications must be registered and reviewed\n    (3–5\
  \ business days) in the LOGILESS Developers console. Access and refresh tokens are valid\n    for 30 days. Tokens are issued per LOGILESS user and scoped to that user's merchant data.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiless/refs/heads/main/scopes/logiless-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Logistics
- E-Commerce
- Order Management
- Warehouse Management
- Inventory
- Fulfillment
- Shipping
- OMS
- WMS
- Japan
token_bound: false
token_urls:
- https://app2.logiless.com/oauth2/token
---
