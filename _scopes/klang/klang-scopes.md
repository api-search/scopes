---
authorization_urls:
- https://login.seed.game/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Klang Scopes
name_suffix: OAuth Scopes
note: Klang publishes no scopes or permissions reference page. These are the scopes advertised verbatim in the SEED OpenID Connect discovery document — the standard OIDC set with no product-specific scopes exposed.
overview: 'Klang Games publishes 5 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Klang Games API on a user''s behalf.


  Tokens are issued from https://login.seed.game/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Klang Games
provider_slug: klang
schemes:
- flows:
  - authorizationUrl: https://login.seed.game/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.seed.game/oauth2/token
  - deviceAuthorizationUrl: https://login.seed.game/oauth2/device_authorize
    flow: deviceCode
    tokenUrl: https://login.seed.game/oauth2/token
  name: SEEDOAuth2
  source: well-known/klang-openid-configuration.json
scope_count: 5
scope_names:
- openid
- offline_access
- email
- phone
- profile
scopes:
- description: Request an ID token and identify the end user (OIDC Core).
  flows:
  - authorizationCode
  scope: openid
- description: Request a refresh token for long-lived access (OIDC Core).
  flows:
  - authorizationCode
  scope: offline_access
- description: Access the email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Access the phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Access the basic profile claims (name, family_name, given_name, middle_name, preferred_username, picture, birthdate).
  flows:
  - authorizationCode
  scope: profile
slug: klang-scopes
source_filename: klang-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://seed.game/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Klang publishes no scopes or permissions reference page. These are the scopes\n  advertised verbatim in the SEED OpenID Connect discovery document — the\n  standard OIDC set with no product-specific scopes exposed.\nschemes:\n- name: SEEDOAuth2\n  source: well-known/klang-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.seed.game/oauth2/authorize\n    tokenUrl: https://login.seed.game/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.seed.game/oauth2/device_authorize\n    tokenUrl: https://login.seed.game/oauth2/token\nscopes:\n- scope: openid\n  description: Request an ID token and identify the end user (OIDC Core).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/klang-openid-configuration.json\n- scope: offline_access\n  description: Request a refresh token\
  \ for long-lived access (OIDC Core).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/klang-openid-configuration.json\n- scope: email\n  description: Access the email and email_verified claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/klang-openid-configuration.json\n- scope: phone\n  description: Access the phone_number and phone_number_verified claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/klang-openid-configuration.json\n- scope: profile\n  description: >-\n    Access the basic profile claims (name, family_name, given_name,\n    middle_name, preferred_username, picture, birthdate).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/klang-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klang/refs/heads/main/scopes/klang-scopes.yml
summary_line: 5 scopes · authorizationCode/deviceCode
tags:
- Company
- Consumer
- Gaming
- Game Development
- MMO
- Simulation
- Entertainment
- Identity
- OpenID Connect
- Berlin
token_urls:
- https://login.seed.game/oauth2/token
---
