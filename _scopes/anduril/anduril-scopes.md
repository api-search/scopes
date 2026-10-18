---
api_specs:
- filename: anduril-entities-api-openapi.yml
  format: yaml
  label: Anduril Industries Entities API
  slug: anduril-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-entities-api-openapi.yml
- filename: anduril-objects-api-openapi.yml
  format: yaml
  label: Anduril Industries Objects API
  slug: anduril-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-objects-api-openapi.yml
- filename: anduril-tasks-api-openapi.yml
  format: yaml
  label: Anduril Industries Tasks API
  slug: anduril-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-tasks-api-openapi.yml
- filename: anduril-oauth-api-openapi.yml
  format: yaml
  label: Anduril Industries O Auth API
  slug: anduril-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-oauth-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Anduril Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Anduril Industries uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.developer.anduril.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anduril Industries
provider_slug: anduril
schemes:
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/anduril-entities-api-openapi.yml
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/anduril-oauth-api-openapi.yml
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/anduril-objects-api-openapi.yml
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/anduril-tasks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: anduril-scopes
source_filename: anduril-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/anduril-entities-api-openapi.yml, openapi/anduril-oauth-api-openapi.yml, openapi/anduril-objects-api-openapi.yml,\n  openapi/anduril-tasks-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/anduril-entities-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n  description: OAuth 2.0 client credentials flow for service-to-service access.\n- name: oauth2ClientCredentials\n  source: openapi/anduril-oauth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n  description: OAuth 2.0 client credentials flow for service-to-service access.\n- name: oauth2ClientCredentials\n  source: openapi/anduril-objects-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n  description: OAuth 2.0 client credentials flow for service-to-service\
  \ access.\n- name: oauth2ClientCredentials\n  source: openapi/anduril-tasks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n  description: OAuth 2.0 client credentials flow for service-to-service access.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/scopes/anduril-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Defense
- Autonomy
- Lattice
- Command and Control
- C2
- Sensors
- Effectors
- Counter-UAS
- Unmanned Systems
- Mission Software
- Edge AI
- ITAR
token_bound: false
token_urls:
- https://api.developer.anduril.com/oauth/token
---
