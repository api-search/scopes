---
authorization_urls:
- https://vault12.com/core/users/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
- password
- refresh_token
kind: oauth-scopes
layout: scope
method: searched
name: Vault12 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vault12 publishes 4 OAuth 2.0 scopes via the authorizationCode, implicit, password, and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Vault12 API on a user''s behalf.


  Tokens are issued from https://vault12.com/core/users/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vault12
provider_slug: vault12
schemes:
- flows:
  - authorizationUrl: https://vault12.com/core/users/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://vault12.com/core/users/oauth2/token
  - authorizationUrl: https://vault12.com/core/users/oauth2/authorize
    flow: implicit
  - flow: password
    tokenUrl: https://vault12.com/core/users/oauth2/token
  - flow: refresh_token
    tokenUrl: https://vault12.com/core/users/oauth2/token
  issuer: https://vault12.com
  name: Vault12 OAuth 2.0 authorization server
  source: well-known/vault12-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication (id_token issuance, RS256 signed)
  flows: []
  scope: openid
- description: Access to the user's profile claims via the userinfo endpoint
  flows: []
  scope: profile
- description: Access to the user's email claims via the userinfo endpoint
  flows: []
  scope: email
- description: Long-lived access via refresh tokens
  flows: []
  scope: offline_access
slug: vault12-scopes
source_filename: vault12-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://vault12.com/.well-known/oauth-authorization-server\ndocs: null\nnotes: >-\n  Vault12 publishes RFC 8414 OAuth 2.0 authorization-server metadata on\n  vault12.com. The scopes_supported list is the standard OpenID Connect set;\n  no product-specific scopes are published. No public scopes/permissions\n  reference page was found on vault12.com.\nschemes:\n  - name: Vault12 OAuth 2.0 authorization server\n    source: well-known/vault12-oauth-authorization-server.json\n    issuer: https://vault12.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://vault12.com/core/users/oauth2/authorize\n        tokenUrl: https://vault12.com/core/users/oauth2/token\n      - flow: implicit\n        authorizationUrl: https://vault12.com/core/users/oauth2/authorize\n      - flow: password\n        tokenUrl: https://vault12.com/core/users/oauth2/token\n      - flow: refresh_token\n        tokenUrl: https://vault12.com/core/users/oauth2/token\n\
  scopes:\n  - scope: openid\n    description: OpenID Connect authentication (id_token issuance, RS256 signed)\n    sources: [well-known/vault12-oauth-authorization-server.json]\n  - scope: profile\n    description: Access to the user's profile claims via the userinfo endpoint\n    sources: [well-known/vault12-oauth-authorization-server.json]\n  - scope: email\n    description: Access to the user's email claims via the userinfo endpoint\n    sources: [well-known/vault12-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Long-lived access via refresh tokens\n    sources: [well-known/vault12-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vault12/refs/heads/main/scopes/vault12-scopes.yml
summary_line: 4 scopes · authorizationCode/implicit/password/refresh_token
tags:
- Company
- Cryptocurrency
- Security
- Backup
- Inheritance
- Wallets
- Cryptography
- Secret Sharing
- Key Management
token_urls:
- https://vault12.com/core/users/oauth2/token
---
