---
api_specs:
- filename: mason-apps-api-openapi.yml
  format: yaml
  label: Mason Apps API
  slug: mason-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-apps-api-openapi.yml
- filename: mason-create-image-api-openapi.yml
  format: yaml
  label: Mason Create Image API
  slug: mason-create-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-create-image-api-openapi.yml
- filename: mason-images-api-openapi.yml
  format: yaml
  label: Mason Images API
  slug: mason-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-images-api-openapi.yml
- filename: mason-retrieve-an-image-api-openapi.yml
  format: yaml
  label: Mason Retrieve an Image API
  slug: mason-retrieve-an-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-retrieve-an-image-api-openapi.yml
- filename: mason-search-api-openapi.yml
  format: yaml
  label: Mason Search API
  slug: mason-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-search-api-openapi.yml
- filename: mason-template-mappings-api-openapi.yml
  format: yaml
  label: Mason Template Mappings API
  slug: mason-template-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-template-mappings-api-openapi.yml
- filename: mason-tiered-discounts-api-openapi.yml
  format: yaml
  label: Mason Tiered Discounts API
  slug: mason-tiered-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-tiered-discounts-api-openapi.yml
- filename: mason-webhooks-api-openapi.yml
  format: yaml
  label: Mason Webhooks API
  slug: mason-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-webhooks-api-openapi.yml
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
- E-Commerce
- Commerce
- Artificial Intelligence
- Agents
- Content Generation
- Discounts
- Promotions
- Webhook
- Shopify
token_urls:
- token
---
