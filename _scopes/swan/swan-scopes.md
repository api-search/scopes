---
authorization_urls: []
description: ''
docs: https://docs.swan.io/developers/using-api/authentication
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Swan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Swan publishes 5 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Swan API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Swan
provider_slug: swan
schemes:
- authorizationUrl: https://oauth.swan.io/oauth2/auth
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  name: OAuth2
  tokenUrl: https://oauth.swan.io/oauth2/token
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- offline
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the client can obtain new access tokens without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy alias for offline refresh-token access.
  flows:
  - authorizationCode
  scope: offline
slug: swan-scopes
source_filename: swan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://oauth.swan.io/.well-known/openid-configuration\ndocs: https://docs.swan.io/developers/using-api/authentication\nschemes:\n- name: OAuth2\n  authorizationUrl: https://oauth.swan.io/oauth2/auth\n  tokenUrl: https://oauth.swan.io/oauth2/token\n  flows: [authorizationCode, clientCredentials, refreshToken]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the user.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email address.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token so the client can obtain new access tokens without re-consent.\n  flows: [authorizationCode]\n- scope: offline\n  description: Legacy alias for offline refresh-token access.\n  flows: [authorizationCode]\nnotes: >-\n\
  \  Scopes are the OpenID Connect scopes advertised by Swan's authorization server\n  discovery document (scopes_supported). Project access tokens obtained via the\n  client_credentials grant are issued with project-level access and an empty\n  scope string; fine-grained authorization for those tokens is governed by the\n  project's configured permissions and by consent granted through user tokens,\n  not by OAuth scope values. Sensitive mutations require a user access token (or\n  a project token impersonating a user) plus explicit user consent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swan/refs/heads/main/scopes/swan-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Banking as a Service
- Embedded Finance
- Fintech
- Payments
- Cards
- SEPA
- GraphQL
- Europe
- Accounts
token_urls: []
---
