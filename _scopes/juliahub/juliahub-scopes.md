---
authorization_urls:
- https://auth.juliahub.com/dex/auth
description: ''
docs: https://help.juliahub.com/julia-api/stable/guides/authentication/
flows:
- deviceCode
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Juliahub Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Juliahub publishes 5 OAuth 2.0 scopes via the deviceCode and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Juliahub API on a user''s behalf.


  Tokens are issued from https://auth.juliahub.com/dex/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Juliahub
provider_slug: juliahub
schemes:
- flows:
  - deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code
    flow: deviceCode
    tokenUrl: https://auth.juliahub.com/dex/token
  - authorizationUrl: https://auth.juliahub.com/dex/auth
    flow: authorizationCode
    tokenUrl: https://auth.juliahub.com/dex/token
  issuer: https://auth.juliahub.com/dex
  name: OAuth2
  source: well-known/juliahub-openid-configuration.json
scope_count: 5
scope_names:
- openid
- email
- profile
- groups
- offline_access
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - deviceCode
  - authorizationCode
  scope: openid
- description: Access the user's email address and email_verified claim.
  flows:
  - deviceCode
  - authorizationCode
  scope: email
- description: Access the user's profile claims (name, preferred_username, locale).
  flows:
  - deviceCode
  - authorizationCode
  scope: profile
- description: Access the user's group memberships on JuliaHub.
  flows:
  - deviceCode
  - authorizationCode
  scope: groups
- description: Issue a refresh token so the client can renew access without re-authenticating.
  flows:
  - deviceCode
  - authorizationCode
  scope: offline_access
slug: juliahub-scopes
source_filename: juliahub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://juliahub.com/.well-known/openid-configuration\ndocs: https://help.juliahub.com/julia-api/stable/guides/authentication/\nschemes:\n- name: OAuth2\n  source: well-known/juliahub-openid-configuration.json\n  issuer: https://auth.juliahub.com/dex\n  flows:\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code\n    tokenUrl: https://auth.juliahub.com/dex/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.juliahub.com/dex/auth\n    tokenUrl: https://auth.juliahub.com/dex/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows: [deviceCode, authorizationCode]\n- scope: email\n  description: Access the user's email address and email_verified claim.\n  flows: [deviceCode, authorizationCode]\n- scope: profile\n  description: Access the user's profile claims (name, preferred_username, locale).\n  flows: [deviceCode,\
  \ authorizationCode]\n- scope: groups\n  description: Access the user's group memberships on JuliaHub.\n  flows: [deviceCode, authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without re-authenticating.\n  flows: [deviceCode, authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juliahub/refs/heads/main/scopes/juliahub-scopes.yml
summary_line: 5 scopes · deviceCode/authorizationCode
tags:
- Julia
- Scientific Computing
- Cloud Computing
- Modeling and Simulation
- High Performance Computing
- Data Science
- Developer Tools
- Package Registry
- Company
token_urls:
- https://auth.juliahub.com/dex/token
---
