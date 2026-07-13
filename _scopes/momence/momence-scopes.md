---
api_specs:
- filename: momence-openapi.yml
  format: yaml
  label: Momence Authentication API
  slug: momence-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Members API
  slug: momence-host-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Sessions & Bookings API
  slug: momence-host-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Memberships API
  slug: momence-host-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Host Checkout & Sales API
  slug: momence-host-checkout-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Account API
  slug: momence-member-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
- filename: momence-openapi.yml
  format: yaml
  label: Momence Member Booking API
  slug: momence-member-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/openapi/momence-openapi.yml
authorization_urls:
- /api/v2/auth/authorize
description: ''
docs: https://api.docs.momence.com/docs/getting-started
flows:
- password
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Momence Scopes
name_suffix: OAuth Scopes
note: Momence OAuth2 does not define scopes - the API is always used as a specific user and all permissions are inferred from that user's Momence account role, per https://api.docs.momence.com/docs/getting-started and https://api.docs.momence.com/docs/authorization.
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
  source: openapi/momence-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: momence-scopes
source_filename: momence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/momence-openapi.yml\ndocs: https://api.docs.momence.com/docs/getting-started\nnote: Momence OAuth2 does not define scopes - the API is always used as a specific\n  user and all permissions are inferred from that user's Momence account role, per\n  https://api.docs.momence.com/docs/getting-started and\n  https://api.docs.momence.com/docs/authorization.\nschemes:\n- name: OAuth2\n  source: openapi/momence-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /api/v2/auth/token\n  - flow: authorizationCode\n    authorizationUrl: /api/v2/auth/authorize\n    tokenUrl: /api/v2/auth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/momence/refs/heads/main/scopes/momence-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fitness
- Wellness
- Studio Management
- Booking
- Scheduling
- Memberships
- Payments
- Class Management
token_urls:
- /api/v2/auth/token
---
