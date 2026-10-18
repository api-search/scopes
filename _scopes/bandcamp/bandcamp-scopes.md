---
api_specs:
- filename: bandcamp-account-api-openapi.yml
  format: yaml
  label: Bandcamp Account API
  slug: bandcamp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/openapi/bandcamp-account-api-openapi.yml
- filename: bandcamp-merch-orders-api-openapi.yml
  format: yaml
  label: Bandcamp Merch Orders API
  slug: bandcamp-merch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/openapi/bandcamp-merch-orders-api-openapi.yml
- filename: bandcamp-sales-api-openapi.yml
  format: yaml
  label: Bandcamp Sales API
  slug: bandcamp-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/openapi/bandcamp-sales-api-openapi.yml
- filename: bandcamp-oauth-api-openapi.yml
  format: yaml
  label: Bandcamp O Auth API
  slug: bandcamp-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/openapi/bandcamp-oauth-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Bandcamp Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Bandcamp uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://bandcamp.com/oauth_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bandcamp
provider_slug: bandcamp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  source: openapi/bandcamp-account-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  source: openapi/bandcamp-merch-orders-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  source: openapi/bandcamp-oauth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  source: openapi/bandcamp-sales-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: bandcamp-scopes
source_filename: bandcamp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/bandcamp-account-api-openapi.yml, openapi/bandcamp-merch-orders-api-openapi.yml,\n  openapi/bandcamp-oauth-api-openapi.yml, openapi/bandcamp-sales-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bandcamp-account-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\n- name: oauth2\n  source: openapi/bandcamp-merch-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\n- name: oauth2\n  source: openapi/bandcamp-oauth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\n- name: oauth2\n  source: openapi/bandcamp-sales-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/scopes/bandcamp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Music
- Marketplace
- Indie
- Audio
- Sales
- Merch
token_bound: false
token_urls:
- https://bandcamp.com/oauth_token
---
