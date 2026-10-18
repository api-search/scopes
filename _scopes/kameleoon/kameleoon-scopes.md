---
api_specs:
- filename: kameleoon-experiments-api-openapi.yml
  format: yaml
  label: Kameleoon Experiments API
  slug: kameleoon-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/openapi/kameleoon-experiments-api-openapi.yml
- filename: kameleoon-personalizations-api-openapi.yml
  format: yaml
  label: Kameleoon Personalizations API
  slug: kameleoon-personalizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/openapi/kameleoon-personalizations-api-openapi.yml
- filename: kameleoon-oauth-api-openapi.yml
  format: yaml
  label: Kameleoon O Auth API
  slug: kameleoon-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/openapi/kameleoon-oauth-api-openapi.yml
authorization_urls:
- https://api.kameleoon.com/oauth/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Kameleoon Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Kameleoon uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.kameleoon.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kameleoon
provider_slug: kameleoon
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.kameleoon.com/oauth/token
  - authorizationUrl: https://api.kameleoon.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kameleoon.com/oauth/token
  name: oauth2
  source: openapi/kameleoon-experiments-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.kameleoon.com/oauth/token
  - authorizationUrl: https://api.kameleoon.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kameleoon.com/oauth/token
  name: oauth2
  source: openapi/kameleoon-oauth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.kameleoon.com/oauth/token
  - authorizationUrl: https://api.kameleoon.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.kameleoon.com/oauth/token
  name: oauth2
  source: openapi/kameleoon-personalizations-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: kameleoon-scopes
source_filename: kameleoon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/kameleoon-experiments-api-openapi.yml, openapi/kameleoon-oauth-api-openapi.yml,\n  openapi/kameleoon-personalizations-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/kameleoon-experiments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.kameleoon.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.kameleoon.com/oauth/authorize\n    tokenUrl: https://api.kameleoon.com/oauth/token\n- name: oauth2\n  source: openapi/kameleoon-oauth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.kameleoon.com/oauth/token\n  - flow: authorizationCode\n    authorizationUrl: https://api.kameleoon.com/oauth/authorize\n    tokenUrl: https://api.kameleoon.com/oauth/token\n- name: oauth2\n  source: openapi/kameleoon-personalizations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.kameleoon.com/oauth/token\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://api.kameleoon.com/oauth/authorize\n    tokenUrl: https://api.kameleoon.com/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kameleoon/refs/heads/main/scopes/kameleoon-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Experimentation
- A/B Testing
- Personalization
- Feature Flags
- Artificial Intelligence
token_bound: false
token_urls:
- https://api.kameleoon.com/oauth/token
---
