---
api_specs:
- filename: spiko-public-openapi.json
  format: json
  label: Spiko Public API
  slug: spiko-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-public-openapi.json
- filename: spiko-investor-openapi.json
  format: json
  label: Spiko Investor API
  slug: spiko-investor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-investor-openapi.json
- filename: spiko-distributor-openapi.json
  format: json
  label: Spiko Distributor API
  slug: spiko-distributor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/openapi/spiko-distributor-openapi.json
authorization_urls:
- https://investor-auth.spiko.io/oauth2/auth
description: ''
docs: https://docs.spiko.io/developers/investor_api/getting_started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Spiko Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spiko publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spiko API on a user''s behalf.


  Tokens are issued from https://investor-auth.spiko.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spiko
provider_slug: spiko
schemes:
- flows:
  - authorizationUrl: https://investor-auth.spiko.io/oauth2/auth
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    tokenUrl: https://investor-auth.spiko.io/oauth2/token
  name: oauth2
  source: openapi/spiko-investor-openapi.json
scope_count: 3
scope_names:
- openid
- offline
- offline_access
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Required for obtaining a refresh token.
  flows:
  - authorizationCode
  scope: offline
- description: Standard OIDC offline access scope for issuing refresh tokens.
  flows:
  - authorizationCode
  scope: offline_access
slug: spiko-scopes
source_filename: spiko-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/spiko-investor-openapi.json\ndocs: https://docs.spiko.io/developers/investor_api/getting_started\nauthorization_server: https://investor-auth.spiko.io\nwell_known: https://investor-auth.spiko.io/.well-known/openid-configuration\nnotes: >-\n  OAuth 2.0 (authorization code + PKCE S256) protects the Investor API. Scopes\n  advertised by the authorization server's OpenID discovery document are openid,\n  offline, and offline_access. The OpenAPI oauth2 flow only enumerates the\n  `offline` scope (used to request a refresh token); the remaining scopes come\n  from the live /.well-known/openid-configuration. The Distributor API does not\n  use OAuth (HTTP Basic only) and therefore has no scope surface.\nschemes:\n- name: oauth2\n  source: openapi/spiko-investor-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://investor-auth.spiko.io/oauth2/auth\n    tokenUrl: https://investor-auth.spiko.io/oauth2/token\n\
  \    code_challenge_methods:\n    - S256\n    - plain\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows:\n  - authorizationCode\n  sources:\n  - https://investor-auth.spiko.io/.well-known/openid-configuration\n- scope: offline\n  description: Required for obtaining a refresh token.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spiko-investor-openapi.json\n- scope: offline_access\n  description: Standard OIDC offline access scope for issuing refresh tokens.\n  flows:\n  - authorizationCode\n  sources:\n  - https://investor-auth.spiko.io/.well-known/openid-configuration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiko/refs/heads/main/scopes/spiko-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Fintech
- Money Market Funds
- Treasury Management
- Tokenization
- Cash Management
- Payments
- Webhooks
token_urls:
- https://investor-auth.spiko.io/oauth2/token
---
