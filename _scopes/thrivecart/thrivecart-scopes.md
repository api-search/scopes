---
api_specs:
- filename: thrivecart-account-api-openapi.yml
  format: yaml
  label: ThriveCart Account API
  slug: thrivecart-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-account-api-openapi.yml
- filename: thrivecart-affiliates-api-openapi.yml
  format: yaml
  label: ThriveCart Affiliates API
  slug: thrivecart-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-affiliates-api-openapi.yml
- filename: thrivecart-bumps-api-openapi.yml
  format: yaml
  label: ThriveCart Bumps API
  slug: thrivecart-bumps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-bumps-api-openapi.yml
- filename: thrivecart-customers-api-openapi.yml
  format: yaml
  label: ThriveCart Customers API
  slug: thrivecart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-customers-api-openapi.yml
- filename: thrivecart-downsells-api-openapi.yml
  format: yaml
  label: ThriveCart Downsells API
  slug: thrivecart-downsells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-downsells-api-openapi.yml
- filename: thrivecart-event-subscriptions-api-openapi.yml
  format: yaml
  label: ThriveCart Event subscriptions API
  slug: thrivecart-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-event-subscriptions-api-openapi.yml
- filename: thrivecart-learn-api-openapi.yml
  format: yaml
  label: ThriveCart Learn API
  slug: thrivecart-learn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-learn-api-openapi.yml
- filename: thrivecart-products-api-openapi.yml
  format: yaml
  label: ThriveCart Products API
  slug: thrivecart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-products-api-openapi.yml
- filename: thrivecart-subscriptions-api-openapi.yml
  format: yaml
  label: ThriveCart Subscriptions API
  slug: thrivecart-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-subscriptions-api-openapi.yml
- filename: thrivecart-transactions-api-openapi.yml
  format: yaml
  label: ThriveCart Transactions API
  slug: thrivecart-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-transactions-api-openapi.yml
- filename: thrivecart-upsells-api-openapi.yml
  format: yaml
  label: ThriveCart Upsells API
  slug: thrivecart-upsells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/openapi/thrivecart-upsells-api-openapi.yml
authorization_urls:
- https://thrivecart.com/authorization/new
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Thrivecart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ThriveCart uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://thrivecart.com/authorization/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ThriveCart
provider_slug: thrivecart
schemes:
- description: OAuth 2.0 authorization code grant for applications acting on behalf of another ThriveCart account. ThriveCart does not publish a scope reference; access is granted account-wide on consent.
  flows:
  - authorizationUrl: https://thrivecart.com/authorization/new
    flow: authorizationCode
    tokenUrl: https://thrivecart.com/authorization/token
  name: oauth2
  source: openapi/thrivecart-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: thrivecart-scopes
source_filename: thrivecart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/thrivecart-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/thrivecart-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://thrivecart.com/authorization/new\n    tokenUrl: https://thrivecart.com/authorization/token\n  description: OAuth 2.0 authorization code grant for applications acting on behalf of another\n    ThriveCart account. ThriveCart does not publish a scope reference; access is granted account-wide\n    on consent.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrivecart/refs/heads/main/scopes/thrivecart-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Checkout
- Shopping Cart
- Payments
- E-Commerce
- Subscription
- Affiliate Marketing
- Learning Management
- Creator Economy
- Webhook
token_urls:
- https://thrivecart.com/authorization/token
---
