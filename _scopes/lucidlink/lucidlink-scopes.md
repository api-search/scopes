---
api_specs:
- filename: lucidlink-service-api.json
  format: json
  label: LucidLink Service API
  slug: lucidlink-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidlink/refs/heads/main/openapi/lucidlink-service-api.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Lucidlink Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LucidLink uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.lucidlink.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LucidLink
provider_slug: lucidlink
schemes:
- api: LucidLink Service API v1
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.lucidlink.com/oauth2/token
  name: standard
  source: openapi/lucidlink-service-api.json
  type: oauth2
scope_count: 0
scope_names: []
scopes: []
slug: lucidlink-scopes
source_filename: lucidlink-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  openapi/lucidlink-service-api.json securityDefinitions, plus a documentation search for a\n  scopes or permissions reference across support.lucidlink.com and www.lucidlink.com\ndocs: null\ndocs_note: >-\n  No scopes or permissions reference page exists. LucidLink's Help Center has no article on\n  API scopes, and the Service Accounts article states the opposite — that for the initial\n  release a service account \"inherits the full permissions/scope of a workspace\n  administrator, granting access to all available API functionalities\".\nschemes:\n- name: standard\n  api: LucidLink Service API v1\n  source: openapi/lucidlink-service-api.json\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.lucidlink.com/oauth2/token\nscopes: []\nscope_count: 0\nfinding: >-\n  LucidLink declares an OAuth2 client-credentials flow with an EMPTY scopes map and applies\n  it globally. There is no way for a\
  \ client to request less than everything: one credential\n  reaches domain creation and deletion, filespace creation and deletion, and billing —\n  including PATCH /billing/payment, which overwrites the payment instrument on the account.\n  For an agent-mediated integration that is the sharpest edge on this API.\npartial_mitigation:\n  name: Collaborator Service Accounts (beta)\n  since: build 3.7.8584 (2026-08-08)\n  detail: >-\n    Scopes automation to specific folders and filespaces rather than to full admin. It\n    applies to the service-account bearer model on the Management API, not to the OAuth2\n    credentials on the public Service API, and it is API-only with no UI in beta.\n  docs: https://support.lucidlink.com/hc/en-us/articles/48014583746573-Collaborator-Service-Accounts-Beta\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidlink/refs/heads/main/scopes/lucidlink-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud Storage
- File Streaming
- File Collaboration
- Media and Entertainment
- Object Storage
- Developer Platform
- MCP
- Agentic AI
- Zero-Knowledge Encryption
- Identity and Access Management
token_urls:
- https://auth.lucidlink.com/oauth2/token
---
