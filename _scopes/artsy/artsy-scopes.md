---
api_specs:
- filename: artsy-public-api-openapi.yml
  format: yaml
  label: Artsy Public API
  slug: artsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artsy/refs/heads/main/openapi/artsy-public-api-openapi.yml
authorization_urls:
- https://api.artsy.net/oauth2/authorize
description: ''
docs: https://developers.artsy.net/v2/docs/authentication
flows:
- authorizationCode
- password
- token-exchange
kind: oauth-scopes
layout: scope
method: searched
name: Artsy Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securityScheme because the harvested Swagger 2.0 declares no security at all. Artsy nevertheless runs a real OAuth 2 authorization server (/oauth2/authorize, /oauth2/access_token) and its documentation names exactly ONE scope value. There is no scopes or permissions reference page — the scope surface is genuinely this small, not merely undiscovered.
overview: 'Artsy publishes 1 OAuth 2.0 scope via the authorizationCode, password, and token-exchange flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Artsy API on a user''s behalf.


  Tokens are issued from https://api.artsy.net/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Artsy
provider_slug: artsy
schemes:
- flows:
  - authorizationUrl: https://api.artsy.net/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.artsy.net/oauth2/access_token
  - flow: password
    tokenUrl: https://api.artsy.net/oauth2/access_token
  - flow: token-exchange
    tokenUrl: https://api.artsy.net/oauth2/access_token
  name: OAuth2
  source: https://developers.artsy.net/v2/docs/authentication
scope_count: 1
scope_names:
- offline_access
scopes:
- description: Requests a long-lived token that expires in 25 years instead of the standard 60 days. Passed as the optional "scope" parameter on any of the three /oauth2/access_token grants and echoed back on the token response.
  flows:
  - authorizationCode
  - password
  - token-exchange
  scope: offline_access
slug: artsy-scopes
source_filename: artsy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://developers.artsy.net/v2/docs/authentication\ndocs: https://developers.artsy.net/v2/docs/authentication\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme because the harvested Swagger 2.0 declares no\n  security at all. Artsy nevertheless runs a real OAuth 2 authorization server (/oauth2/authorize,\n  /oauth2/access_token) and its documentation names exactly ONE scope value. There is no scopes or\n  permissions reference page — the scope surface is genuinely this small, not merely undiscovered.\nschemes:\n  - name: OAuth2\n    source: https://developers.artsy.net/v2/docs/authentication\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.artsy.net/oauth2/authorize\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n      - flow: password\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n      - flow: token-exchange\n        tokenUrl: https://api.artsy.net/oauth2/access_token\n\
  scopes:\n  - scope: offline_access\n    description: >-\n      Requests a long-lived token that expires in 25 years instead of the standard 60 days. Passed as\n      the optional \"scope\" parameter on any of the three /oauth2/access_token grants and echoed back\n      on the token response.\n    flows: [authorizationCode, password, token-exchange]\n    sources: [https://developers.artsy.net/v2/docs/authentication]\nscope_count: 1\nmissing:\n  - >-\n    No per-resource scopes are published. Access to write operations (applications, devices, tokens)\n    and to user-bound collections is governed by which token you hold, not by a scope grant.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artsy/refs/heads/main/scopes/artsy-scopes.yml
summary_line: 1 scope · authorizationCode/password/token-exchange
tags:
- Art
- Marketplace
- Artists
- Collectors
- Galleries
- Auctions
- Museums
- Art Market
- Culture
- Images
token_urls:
- https://api.artsy.net/oauth2/access_token
---
