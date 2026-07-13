---
api_specs:
- filename: warner-music-group-licensing-openapi.yml
  format: yaml
  label: Warner Music Group Licensing API
  slug: wmg-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/openapi/warner-music-group-licensing-openapi.yml
authorization_urls:
- https://auth.wmg.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Warner Music Group Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Warner Music Group publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Warner Music Group API on a user''s behalf.


  Tokens are issued from https://auth.wmg.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Warner Music Group
provider_slug: warner-music-group
schemes:
- description: OAuth 2.0 for WMG partner authentication
  flows:
  - authorizationUrl: https://auth.wmg.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.wmg.com/oauth/token
  name: OAuth2
  source: openapi/warner-music-group-licensing-openapi.yml
scope_count: 3
scope_names:
- catalog:read
- licenses:read
- licenses:write
scopes:
- description: Read catalog information
  flows:
  - authorizationCode
  scope: catalog:read
- description: Read license requests
  flows:
  - authorizationCode
  scope: licenses:read
- description: Submit license requests
  flows:
  - authorizationCode
  scope: licenses:write
slug: warner-music-group-scopes
source_filename: warner-music-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warner-music-group-licensing-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/warner-music-group-licensing-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wmg.com/oauth/authorize\n    tokenUrl: https://auth.wmg.com/oauth/token\n  description: OAuth 2.0 for WMG partner authentication\nscopes:\n- scope: catalog:read\n  description: Read catalog information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/warner-music-group-licensing-openapi.yml\n- scope: licenses:read\n  description: Read license requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/warner-music-group-licensing-openapi.yml\n- scope: licenses:write\n  description: Submit license requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/warner-music-group-licensing-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/scopes/warner-music-group-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Music
- Entertainment
- Streaming
- Licensing
- Publishing
token_urls:
- https://auth.wmg.com/oauth/token
---
