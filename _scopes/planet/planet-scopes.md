---
authorization_urls:
- https://login.planet.com/authorize
description: ''
docs: https://docs.planet.com/develop/authentication/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Planet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Planet publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Planet API on a user''s behalf.


  Tokens are issued from https://login.planet.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Planet
provider_slug: planet
schemes:
- flows:
  - authorizationUrl: https://login.planet.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.planet.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.planet.com/oauth/token
  name: PlanetOAuth2
  source: https://docs.planet.com/develop/authentication/
scope_count: 5
scope_names:
- planet
- offline_access
- openid
- profile
- email
scopes:
- description: Access to all Planet APIs (the primary API-access scope).
  flows:
  - authorizationCode
  - clientCredentials
  scope: planet
- description: Issue a refresh token so a user session can be renewed without re-login.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect - authenticate the user and return an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims (name, nickname, picture, etc.).
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email address and verification status.
  flows:
  - authorizationCode
  scope: email
slug: planet-scopes
source_filename: planet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://login.planet.com/.well-known/openid-configuration\ndocs: https://docs.planet.com/develop/authentication/\nschemes:\n- name: PlanetOAuth2\n  source: https://docs.planet.com/develop/authentication/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.planet.com/authorize\n    tokenUrl: https://login.planet.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.planet.com/oauth/token\nscopes:\n- scope: planet\n  description: Access to all Planet APIs (the primary API-access scope).\n  flows: [authorizationCode, clientCredentials]\n- scope: offline_access\n  description: Issue a refresh token so a user session can be renewed without re-login.\n  flows: [authorizationCode]\n- scope: openid\n  description: OpenID Connect - authenticate the user and return an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims (name, nickname,\
  \ picture, etc.).\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email address and verification status.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes above marked as OIDC identity scopes (openid/profile/email/offline_access)\n  are advertised in the login.planet.com discovery document; `planet` is the\n  documented scope that grants access to the Planet APIs. The authorization server\n  additionally advertises fine-grained OIDC claim scopes (name, given_name,\n  family_name, nickname, phone, address, picture, created_at, identities).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planet/refs/heads/main/scopes/planet-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Satellite Imagery
- Earth Observation
- Geospatial
- Remote Sensing
- Mapping
- Analytics
- Location
- Data
- GIS
- Company
token_urls:
- https://login.planet.com/oauth/token
---
