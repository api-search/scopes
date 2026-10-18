---
api_specs:
- filename: arity-activation-api-openapi.yml
  format: yaml
  label: Arity Activation API
  slug: arity-activation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-activation-api-openapi.yml
- filename: arity-authentication-api-openapi.yml
  format: yaml
  label: Arity Authentication API
  slug: arity-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-authentication-api-openapi.yml
- filename: arity-booking-api-documentation-api-openapi.yml
  format: yaml
  label: Arity Booking API Documentation API
  slug: arity-booking-api-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-booking-api-documentation-api-openapi.yml
- filename: arity-prequalcredit-api-openapi.yml
  format: yaml
  label: Arity Pre Qual Credit API
  slug: arity-prequalcredit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-prequalcredit-api-openapi.yml
- filename: arity-registration-api-openapi.yml
  format: yaml
  label: Arity Registration API
  slug: arity-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-registration-api-openapi.yml
- filename: arity-scoring-api-openapi.yml
  format: yaml
  label: Arity Scoring API
  slug: arity-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-scoring-api-openapi.yml
- filename: arity-trip-intelligence-api-openapi.yml
  format: yaml
  label: Arity Trip Intelligence API
  slug: arity-trip-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/openapi/arity-trip-intelligence-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Arity Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Arity uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.arity.com/platform/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arity
provider_slug: arity
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.arity.com/platform/oauth/v1/token
  name: oauth2
  source: openapi/arity-driving-engine-booking-api.yml
scope_count: 0
scope_names: []
scopes: []
slug: arity-scopes
source_filename: arity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/arity-driving-engine-booking-api.yml\nschemes:\n- name: oauth2\n  source: openapi/arity-driving-engine-booking-api.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.arity.com/platform/oauth/v1/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arity/refs/heads/main/scopes/arity-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Telematics
- Mobility Data
- Insurance
- Driving Behavior
- Analytics
- Location Data
token_bound: false
token_urls:
- https://api.arity.com/platform/oauth/v1/token
---
