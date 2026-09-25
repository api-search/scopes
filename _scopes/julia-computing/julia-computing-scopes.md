---
authorization_urls:
- https://auth.juliahub.com/dex/auth
description: ''
docs: https://help.juliahub.com/juliahub-jl/stable/getting-started/
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Julia Computing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Julia Computing publishes 5 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Julia Computing API on a user''s behalf.


  Tokens are issued from https://auth.juliahub.com/dex/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Julia Computing
provider_slug: julia-computing
schemes:
- flows:
  - authorizationUrl: https://auth.juliahub.com/dex/auth
    flow: authorizationCode
    tokenUrl: https://auth.juliahub.com/dex/token
  - deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code
    flow: deviceCode
    tokenUrl: https://auth.juliahub.com/dex/token
  issuer: https://auth.juliahub.com/dex
  name: OpenIDConnect
  source: well-known/julia-computing-openid-configuration.json
scope_count: 5
scope_names:
- openid
- email
- profile
- groups
- offline_access
scopes:
- description: Required OpenID Connect scope; requests an ID token identifying the authenticated JuliaHub user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access to the user's email address and email_verified claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Access to the user's basic profile claims (name, preferred_username, locale).
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access to the user's group memberships used for JuliaHub organization/authorization.
  flows:
  - authorizationCode
  - deviceCode
  scope: groups
- description: Requests a refresh token so the client can obtain new access tokens without re-authentication.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: julia-computing-scopes
source_filename: julia-computing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://juliahub.com/.well-known/openid-configuration\ndocs: https://help.juliahub.com/juliahub-jl/stable/getting-started/\nschemes:\n  - name: OpenIDConnect\n    source: well-known/julia-computing-openid-configuration.json\n    issuer: https://auth.juliahub.com/dex\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.juliahub.com/dex/auth\n        tokenUrl: https://auth.juliahub.com/dex/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://auth.juliahub.com/dex/device/code\n        tokenUrl: https://auth.juliahub.com/dex/token\nscopes:\n  - scope: openid\n    description: Required OpenID Connect scope; requests an ID token identifying the authenticated JuliaHub user.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/julia-computing-openid-configuration.json]\n  - scope: email\n    description: Access to the user's email address and email_verified claim.\n\
  \    flows: [authorizationCode, deviceCode]\n    sources: [well-known/julia-computing-openid-configuration.json]\n  - scope: profile\n    description: Access to the user's basic profile claims (name, preferred_username, locale).\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/julia-computing-openid-configuration.json]\n  - scope: groups\n    description: Access to the user's group memberships used for JuliaHub organization/authorization.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/julia-computing-openid-configuration.json]\n  - scope: offline_access\n    description: Requests a refresh token so the client can obtain new access tokens without re-authentication.\n    flows: [authorizationCode, deviceCode]\n    sources: [well-known/julia-computing-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/julia-computing/refs/heads/main/scopes/julia-computing-scopes.yml
summary_line: 5 scopes · authorizationCode/deviceCode
tags:
- Company
- Julia
- Scientific Computing
- Modeling and Simulation
- High Performance Computing
- Cloud Computing
- Data Science
- Programming Language
- Package Registry
- Machine Learning
- Pharma
token_urls:
- https://auth.juliahub.com/dex/token
---
