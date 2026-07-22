---
api_specs:
- filename: mason-apps-openapi.json
  format: json
  label: Mason Apps API
  slug: mason-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-apps-openapi.json
- filename: mason-generation-openapi.json
  format: json
  label: Mason Generation API (Genie)
  slug: mason-generation-api-genie
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-generation-openapi.json
- filename: mason-tasks-openapi.json
  format: json
  label: Mason Creative Tasks API
  slug: mason-creative-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-tasks-openapi.json
- filename: mason-search-openapi.json
  format: json
  label: Mason Asset Search API
  slug: mason-asset-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-search-openapi.json
- filename: mason-webhooks-openapi.json
  format: json
  label: Mason Webhooks API
  slug: mason-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-webhooks-openapi.json
- filename: mason-discounts-openapi.json
  format: json
  label: Mason Promotion Engine API (Scrooge)
  slug: mason-promotion-engine-api-scrooge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-discounts-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Mason Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mason uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mason
provider_slug: mason
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/mason-apps-openapi.json
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/mason-generation-openapi.json
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/mason-search-openapi.json
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/mason-webhooks-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: mason-scopes
source_filename: mason-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mason-apps-openapi.json, openapi/mason-generation-openapi.json, openapi/mason-search-openapi.json,\n  openapi/mason-webhooks-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/mason-apps-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/mason-generation-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/mason-search-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\n- name: OAuth2PasswordBearer\n  source: openapi/mason-webhooks-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/scopes/mason-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ecommerce
- Commerce
- AI
- Agents
- Content Generation
- Discounts
- Promotions
- Webhooks
- Shopify
token_urls:
- token
---
