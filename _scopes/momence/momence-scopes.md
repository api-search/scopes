---
api_specs:
- filename: momence-auth-api-openapi.yml
  format: yaml
  label: Momence Auth API
  slug: momence-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-auth-api-openapi.yml
- filename: momence-host-api-openapi.yml
  format: yaml
  label: Momence Host API
  slug: momence-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-host-api-openapi.yml
- filename: momence-host-checkout-api-openapi.yml
  format: yaml
  label: Momence Host Checkout API
  slug: momence-host-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-host-checkout-api-openapi.yml
- filename: momence-member-addresses-api-openapi.yml
  format: yaml
  label: Momence Member Addresses API
  slug: momence-member-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-addresses-api-openapi.yml
- filename: momence-member-api-openapi.yml
  format: yaml
  label: Momence Member API
  slug: momence-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-api-openapi.yml
- filename: momence-member-checkout-api-openapi.yml
  format: yaml
  label: Momence Member Checkout API
  slug: momence-member-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-checkout-api-openapi.yml
- filename: momence-member-host-api-openapi.yml
  format: yaml
  label: Momence Member Host API
  slug: momence-member-host-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-host-api-openapi.yml
- filename: momence-member-sessions-api-openapi.yml
  format: yaml
  label: Momence Member Sessions API
  slug: momence-member-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-member-sessions-api-openapi.yml
authorization_urls:
- /api/v2/auth/authorize
description: ''
docs: ''
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Momence Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Momence uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/v2/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Momence
provider_slug: momence
schemes:
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-auth-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-host-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-host-checkout-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-member-addresses-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-member-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-member-checkout-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-member-host-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /api/v2/auth/token
  - authorizationUrl: /api/v2/auth/authorize
    flow: authorizationCode
    tokenUrl: /api/v2/auth/token
  name: OAuth2
  source: openapi/momence-member-sessions-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: momence-scopes
source_filename: momence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/momence-auth-api-openapi.yml, openapi/momence-host-api-openapi.yml, openapi/momence-host-checkout-api-openapi.yml,\n  openapi/momence-member-addresses-api-openapi.yml, openapi/momence-member-api-openapi.yml,\n  openapi/momence-member-checkout-api-openapi.yml, openapi/momence-member-host-api-openapi.yml,\n  openapi/momence-member-sessions-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/momence-auth-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-host-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-host-checkout-api-openapi.yml\n  flows:\n  - flow:\
  \ password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-member-addresses-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-member-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-member-checkout-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-member-host-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl:\
  \ /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\n- name: OAuth2\n  source: openapi/momence-member-sessions-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/scopes/momence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fitness
- Wellness
- Studio Management
- Booking
- Scheduling
- Membership
- Payments
- Class Management
token_bound: false
token_urls:
- /api/v2/auth/token
---
