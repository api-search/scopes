---
authorization_urls:
- https://auth.numeric.io/oauth2/authorize
description: ''
docs: https://api.numeric.io/.well-known/oauth-authorization-server
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Numeric Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Numeric publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Numeric API on a user''s behalf.


  Tokens are issued from https://auth.numeric.io/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Numeric
provider_slug: numeric
schemes:
- flows:
  - authorizationUrl: https://auth.numeric.io/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.numeric.io/oauth2/token
  - deviceAuthorizationUrl: https://auth.numeric.io/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://auth.numeric.io/oauth2/token
  issuer: https://auth.numeric.io
  name: OAuth2
  source: well-known/numeric-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email address claim.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
slug: numeric-scopes
source_filename: numeric-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://auth.numeric.io/.well-known/oauth-authorization-server\ndocs: https://api.numeric.io/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/numeric-oauth-authorization-server.json\n  issuer: https://auth.numeric.io\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.numeric.io/oauth2/authorize\n    tokenUrl: https://auth.numeric.io/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.numeric.io/oauth2/device_authorization\n    tokenUrl: https://auth.numeric.io/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  sources: [well-known/numeric-oauth-authorization-server.json]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  sources: [well-known/numeric-oauth-authorization-server.json]\n- scope: email\n  description: Access to the user's email address claim.\n\
  \  sources: [well-known/numeric-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n  sources: [well-known/numeric-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numeric/refs/heads/main/scopes/numeric-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Fintech
- Accounting
- Financial Close
- Reconciliation
- MCP
- Agent Skills
- OAuth
token_urls:
- https://auth.numeric.io/oauth2/token
---
