---
api_specs:
- filename: advance-auto-parts-catalog-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Catalog API
  slug: advance-auto-parts-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-catalog-api-openapi.yml
- filename: advance-auto-parts-commerce-api-openapi.yml
  format: yaml
  label: Advance Auto Parts Commerce API
  slug: advance-auto-parts-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/openapi/advance-auto-parts-commerce-api-openapi.yml
authorization_urls:
- https://auth.advanceautoparts.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Advance Auto Parts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Advance Auto Parts publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Advance Auto Parts API on a user''s behalf.


  Tokens are issued from https://auth.advanceautoparts.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Advance Auto Parts
provider_slug: advance-auto-parts
schemes:
- flows:
  - authorizationUrl: https://auth.advanceautoparts.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.advanceautoparts.com/oauth/token
  name: oauth2
  source: openapi/advance-auto-parts-commerce-api-openapi.yml
scope_count: 4
scope_names:
- catalog:read
- loyalty:read
- orders:read
- orders:write
scopes:
- description: Read product catalog
  flows:
  - authorizationCode
  scope: catalog:read
- description: Read loyalty account
  flows:
  - authorizationCode
  scope: loyalty:read
- description: Read order history
  flows:
  - authorizationCode
  scope: orders:read
- description: Place and manage orders
  flows:
  - authorizationCode
  scope: orders:write
slug: advance-auto-parts-scopes
source_filename: advance-auto-parts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/advance-auto-parts-commerce-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/advance-auto-parts-commerce-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.advanceautoparts.com/oauth/authorize\n    tokenUrl: https://auth.advanceautoparts.com/oauth/token\nscopes:\n- scope: catalog:read\n  description: Read product catalog\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/advance-auto-parts-commerce-api-openapi.yml\n- scope: loyalty:read\n  description: Read loyalty account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/advance-auto-parts-commerce-api-openapi.yml\n- scope: orders:read\n  description: Read order history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/advance-auto-parts-commerce-api-openapi.yml\n- scope: orders:write\n  description: Place and manage orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/advance-auto-parts-commerce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advance-auto-parts/refs/heads/main/scopes/advance-auto-parts-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Automotive
- E-Commerce
- Parts Catalog
- Retail
- Supply Chain
- Fortune 500
token_urls:
- https://auth.advanceautoparts.com/oauth/token
---
