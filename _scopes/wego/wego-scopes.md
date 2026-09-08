---
api_specs:
- filename: wego-api-openapi.json
  format: json
  label: Wego API
  slug: wego-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/openapi/wego-api-openapi.json
authorization_urls:
- https://auth.wego.com/user-auth/v2/users/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wego Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wego publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wego API on a user''s behalf.


  Tokens are issued from https://auth.wego.com/user-auth/v2/users/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wego
provider_slug: wego
schemes:
- description: OAuth2 authorization-code flow (PKCE supported) against the Wego auth server.
  flows:
  - authorizationUrl: https://auth.wego.com/user-auth/v2/users/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.wego.com/user-auth/v2/users/oauth/token
  name: oauth2
  source: openapi/wego-api-openapi.json
scope_count: 3
scope_names:
- openid
- profile
- users
scopes:
- description: OpenID Connect sign-in.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: User identity for the API.
  flows:
  - authorizationCode
  scope: users
slug: wego-scopes
source_filename: wego-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/wego-api-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/wego-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.wego.com/user-auth/v2/users/oauth/authorize\n    tokenUrl: https://auth.wego.com/user-auth/v2/users/oauth/token\n  description: OAuth2 authorization-code flow (PKCE supported) against the Wego auth server.\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wego-api-openapi.json\n- scope: profile\n  description: Basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wego-api-openapi.json\n- scope: users\n  description: User identity for the API.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wego-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wego/refs/heads/main/scopes/wego-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Travel
- Flights
- Hotels
- Metasearch
- Booking
- Agent Native
- Tourism
- Search
token_urls:
- https://auth.wego.com/user-auth/v2/users/oauth/token
---
