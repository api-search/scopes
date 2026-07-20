---
authorization_urls:
- https://auth.carto.com/authorize
description: ''
docs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Cartodb Scopes
name_suffix: OAuth Scopes
note: CARTO authenticates the Cloud-Native API with OAuth 2.0 bearer tokens issued by the Auth0-backed identity provider (auth.carto.com) for the `carto-cloud-native-api` audience. API-resource permissions are carried on the token as the user's/M2M-client's granted access rather than a fixed public scope registry; the OIDC identity scopes below come verbatim from the auth server's discovery document.
overview: 'CARTO publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CARTO API on a user''s behalf.


  Tokens are issued from https://auth.carto.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CARTO
provider_slug: cartodb
schemes:
- audience: carto-cloud-native-api
  flows:
  - authorizationUrl: https://auth.carto.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.carto.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.carto.com/oauth/token
  name: OAuth2
  source: well-known/cartodb-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access the user's basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email and email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: cartodb-scopes
source_filename: cartodb-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods/oauth-access-tokens\ndocs: https://docs.carto.com/carto-for-developers/key-concepts/authentication-methods\nnote: >-\n  CARTO authenticates the Cloud-Native API with OAuth 2.0 bearer tokens issued by\n  the Auth0-backed identity provider (auth.carto.com) for the\n  `carto-cloud-native-api` audience. API-resource permissions are carried on the\n  token as the user's/M2M-client's granted access rather than a fixed public scope\n  registry; the OIDC identity scopes below come verbatim from the auth server's\n  discovery document.\nschemes:\n- name: OAuth2\n  source: well-known/cartodb-oauth-authorization-server.json\n  audience: carto-cloud-native-api\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.carto.com/authorize\n    tokenUrl: https://auth.carto.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.carto.com/oauth/token\n\
  scopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token.\n  sources: [well-known/cartodb-openid-configuration.json]\n- scope: profile\n  description: Access the user's basic profile claims.\n  sources: [well-known/cartodb-openid-configuration.json]\n- scope: email\n  description: Access the user's email and email_verified claims.\n  sources: [well-known/cartodb-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  sources: [well-known/cartodb-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cartodb/refs/heads/main/scopes/cartodb-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Developer Tools
- Location Intelligence
- Geospatial
- Maps
- Spatial Analytics
- Data Warehouse
- GIS
- Agents
token_urls:
- https://auth.carto.com/oauth/token
---
