---
api_specs:
- filename: debank-pro-openapi.yml
  format: yaml
  label: DeBank OpenAPI
  slug: debank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/openapi/debank-pro-openapi.yml
authorization_urls:
- https://debank.com/connect
description: ''
docs: https://docs.cloud.debank.com/en/debank-connect/integration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Debank Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 lives in DeBank Connect, not in the published Swagger — derive-oauth-scopes.py found zero oauth2 securitySchemes in openapi/, so this file is searched from the Connect integration guide. The DeBank Cloud Pro API (pro-openapi.debank.com) is api-key only and has no scope surface.
overview: 'DeBank publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DeBank API on a user''s behalf.


  Tokens are issued from https://api.connect.debank.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DeBank
provider_slug: debank
schemes:
- client_authentication: client_secret_basic (HTTP Basic with client_id/client_secret)
  flows:
  - authorizationUrl: https://debank.com/connect
    flow: authorizationCode
    pkce: false
    refreshUrl: https://api.connect.debank.com/oauth/token
    refresh_token: true
    response_type: code
    state_supported: true
    tokenUrl: https://api.connect.debank.com/oauth/token
    token_type: Bearer
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: DeBank Connect
  source: https://docs.cloud.debank.com/en/debank-connect/integration
  token_endpoint_auth_note: Documented as HTTPBasicAuth(client_id, client_secret) on a form-data POST.
scope_count: 3
scope_names:
- user:base:read
- user:chain:read
- user:social:read
scopes:
- description: Read the authorizing user's base profile — address, web3_id, name, avatar, on-chain birth time and follower value.
  flows:
  - authorizationCode
  scope: user:base:read
- description: Read the authorizing user's on-chain portfolio data.
  flows:
  - authorizationCode
  scope: user:chain:read
- description: Read the authorizing user's social following data.
  flows:
  - authorizationCode
  scope: user:social:read
slug: debank-scopes
source_filename: debank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.cloud.debank.com/en/debank-connect/integration\ndocs: https://docs.cloud.debank.com/en/debank-connect/integration\nnote: OAuth 2.0 lives in DeBank Connect, not in the published Swagger — derive-oauth-scopes.py found zero oauth2\n  securitySchemes in openapi/, so this file is searched from the Connect integration guide. The DeBank Cloud Pro\n  API (pro-openapi.debank.com) is api-key only and has no scope surface.\nschemes:\n- name: DeBank Connect\n  source: https://docs.cloud.debank.com/en/debank-connect/integration\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  client_authentication: client_secret_basic (HTTP Basic with client_id/client_secret)\n  token_endpoint_auth_note: Documented as HTTPBasicAuth(client_id, client_secret) on a form-data POST.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://debank.com/connect\n    tokenUrl: https://api.connect.debank.com/oauth/token\n\
  \    refreshUrl: https://api.connect.debank.com/oauth/token\n    response_type: code\n    state_supported: true\n    pkce: false\n    token_type: Bearer\n    refresh_token: true\nscopes:\n- scope: user:base:read\n  description: Read the authorizing user's base profile — address, web3_id, name, avatar, on-chain birth time and\n    follower value.\n  flows:\n  - authorizationCode\n  api: GET https://api.connect.debank.com/v1/user\n  docs: https://docs.cloud.debank.com/en/debank-connect/api/user-base-data\n  sources:\n  - https://docs.cloud.debank.com/en/debank-connect/integration\n- scope: user:chain:read\n  description: Read the authorizing user's on-chain portfolio data.\n  flows:\n  - authorizationCode\n  docs: https://docs.cloud.debank.com/en/debank-connect/api/user-chain-data\n  sources:\n  - https://docs.cloud.debank.com/en/debank-connect/integration\n- scope: user:social:read\n  description: Read the authorizing user's social following data.\n  flows:\n  - authorizationCode\n  docs:\
  \ https://docs.cloud.debank.com/en/debank-connect/api/user-social-data\n  sources:\n  - https://docs.cloud.debank.com/en/debank-connect/integration\nscope_count: 3\ndiscovery:\n  oauth_authorization_server: null\n  openid_configuration: null\n  note: Neither /.well-known/oauth-authorization-server nor /.well-known/openid-configuration is served on api.connect.debank.com\n    (both 404, probed 2026-08-12), so the endpoints above are documented only in prose. Not OpenID Connect — no\n    id_token, no userinfo discovery.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debank/refs/heads/main/scopes/debank-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- web3
- defi
- blockchain
- crypto
- portfolio-tracking
- on-chain-data
- wallet
- token-data
- nft
- ethereum
- oauth
- market-data
token_urls:
- https://api.connect.debank.com/oauth/token
---
