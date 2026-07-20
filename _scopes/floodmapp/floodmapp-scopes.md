---
authorization_urls:
- https://login.floodmapp.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Floodmapp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FloodMapp publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FloodMapp API on a user''s behalf.


  Tokens are issued from https://login.floodmapp.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FloodMapp
provider_slug: floodmapp
schemes:
- flows:
  - authorizationUrl: https://login.floodmapp.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.floodmapp.com/oauth2/token
  name: cognitoOAuth2
  provider: AWS Cognito
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the authenticated principal.
  flows:
  - authorizationCode
  scope: openid
slug: floodmapp-scopes
source_filename: floodmapp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Observed OAuth2 authorization request from api.floodmapp.com to AWS Cognito\n  (login.floodmapp.com/oauth2/authorize).\nschemes:\n  - name: cognitoOAuth2\n    provider: AWS Cognito\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.floodmapp.com/oauth2/authorize\n        tokenUrl: https://login.floodmapp.com/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; returns an ID token identifying the authenticated principal.\n    flows: [authorizationCode]\n    sources: [observed authorization request]\nnotes: >-\n  Only the standard OIDC 'openid' scope was observed in the public authorization\n  redirect. FloodMapp does not publish a scopes/permissions reference; any\n  resource-server scopes are provisioned privately per customer. Not fabricated\n  beyond the single observed scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/floodmapp/refs/heads/main/scopes/floodmapp-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Flood Intelligence
- Flood Forecasting
- Geospatial
- GIS
- Emergency Management
- Climate Risk
- Machine Learning
- Hydrology
token_urls:
- https://login.floodmapp.com/oauth2/token
---
