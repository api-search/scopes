---
authorization_urls:
- https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth
description: ''
docs: https://docs.picogrid.com/reference/start
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Picogrid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Picogrid publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Picogrid API on a user''s behalf.


  Tokens are issued from https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Picogrid
provider_slug: picogrid
schemes:
- flows:
  - authorizationUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token
  name: OAuth2
  provider: Keycloak (realm "legion")
  source: well-known/picogrid-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- profile
- email
- offline_access
- global:::basic
- global:::profile
- global:::email
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived, offline access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legion global basic access scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: global:::basic
- description: Legion global profile scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: global:::profile
- description: Legion global email scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: global:::email
slug: picogrid-scopes
source_filename: picogrid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://legion-prod.picogrid.com/v3/.well-known/oauth-authorization-server\ndocs: https://docs.picogrid.com/reference/start\nschemes:\n- name: OAuth2\n  source: well-known/picogrid-oauth-authorization-server.json\n  provider: Keycloak (realm \"legion\")\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/auth\n    tokenUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email claim.\n  flows: [authorizationCode]\n\
  - scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n  flows: [authorizationCode]\n- scope: 'global:::basic'\n  description: Legion global basic access scope.\n  flows: [authorizationCode, clientCredentials]\n- scope: 'global:::profile'\n  description: Legion global profile scope.\n  flows: [authorizationCode, clientCredentials]\n- scope: 'global:::email'\n  description: Legion global email scope.\n  flows: [authorizationCode, clientCredentials]\nnotes: >-\n  These are the OAuth scopes advertised by the Keycloak realm's authorization\n  server metadata (scopes_supported). Legion layers a separate fine-grained,\n  resource-level authorization model on top of scopes (organization roles such\n  as org:viewer / org:operator / org:admin / system-admin, plus permission\n  templates and grant/revoke/check operations under /v3/authorization/*), so\n  effective access is governed by permissions in addition to token scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picogrid/refs/heads/main/scopes/picogrid-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Company
- Data
- Defense
- Public Safety
- Systems Integration
- Sensors
- Unmanned Systems
- Command and Control
- Geospatial
- Situational Awareness
- OAuth
- Video Streaming
token_urls:
- https://auth.legion-prod.picogrid.com/realms/legion/protocol/openid-connect/token
---
