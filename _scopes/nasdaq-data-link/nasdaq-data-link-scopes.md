---
api_specs:
- filename: postman
  format: yaml
  label: Nasdaq Data Link REST API for Real-Time or Delayed Data
  slug: nasdaq-data-link-rest-api-for-real-time-or-delayed-data
  spec_type: Postman
  url: https://github.com/Nasdaq/NasdaqCloudDataService-REST-API/tree/main/restapi/postman
authorization_urls:
- https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/authorize
description: ''
docs: https://docs.data.nasdaq.com/docs/streaming-api
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nasdaq Data Link Scopes
name_suffix: OAuth Scopes
note: Nasdaq Data Link publishes no user-facing scopes reference; scopes below are the scopes_supported advertised by the live RFC 8414 authorization-server metadata (Okta org signin.nasdaq.com) that data.nasdaq.com's RFC 9728 protected-resource metadata points at. The core Tables REST API uses api_key query-parameter auth (no scopes); OAuth applies to the Nasdaq Cloud Data Service streaming/real-time surface, whose credentials are provisioned by Nasdaq sales.
overview: 'Nasdaq Data Link publishes 9 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nasdaq Data Link API on a user''s behalf.


  Tokens are issued from https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nasdaq Data Link
provider_slug: nasdaq-data-link
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token
  - authorizationUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/authorize
    flow: authorizationCode
    tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token
  issuer: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417
  name: nasdaq-okta
scope_count: 9
scope_names:
- datalink
- interclient_access
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
scopes:
- description: Nasdaq Data Link resource access (custom scope advertised by the authorization server)
  flows: []
  scope: datalink
- description: Inter-client access (custom scope advertised by the authorization server)
  flows: []
  scope: interclient_access
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: OIDC profile claims
  flows: []
  scope: profile
- description: OIDC email claims
  flows: []
  scope: email
- description: OIDC address claims
  flows: []
  scope: address
- description: OIDC phone claims
  flows: []
  scope: phone
- description: Refresh token issuance
  flows: []
  scope: offline_access
- description: Device single sign-on
  flows: []
  scope: device_sso
slug: nasdaq-data-link-scopes
source_filename: nasdaq-data-link-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/.well-known/oauth-authorization-server\ndocs: https://docs.data.nasdaq.com/docs/streaming-api\nnote: >-\n  Nasdaq Data Link publishes no user-facing scopes reference; scopes below are\n  the scopes_supported advertised by the live RFC 8414 authorization-server\n  metadata (Okta org signin.nasdaq.com) that data.nasdaq.com's RFC 9728\n  protected-resource metadata points at. The core Tables REST API uses api_key\n  query-parameter auth (no scopes); OAuth applies to the Nasdaq Cloud Data\n  Service streaming/real-time surface, whose credentials are provisioned by\n  Nasdaq sales.\nschemes:\n  - name: nasdaq-okta\n    issuer: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token\n      - flow: authorizationCode\n        authorizationUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/authorize\n\
  \        tokenUrl: https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token\nscopes:\n  - scope: datalink\n    description: Nasdaq Data Link resource access (custom scope advertised by the authorization server)\n  - scope: interclient_access\n    description: Inter-client access (custom scope advertised by the authorization server)\n  - scope: openid\n    description: OpenID Connect authentication\n  - scope: profile\n    description: OIDC profile claims\n  - scope: email\n    description: OIDC email claims\n  - scope: address\n    description: OIDC address claims\n  - scope: phone\n    description: OIDC phone claims\n  - scope: offline_access\n    description: Refresh token issuance\n  - scope: device_sso\n    description: Device single sign-on\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-data-link/refs/heads/main/scopes/nasdaq-data-link-scopes.yml
summary_line: 9 scopes · clientCredentials/authorizationCode
tags:
- Financial Data
- Stock Market
- Market Data
- Economic Data
- Alternative Data
- Time Series
- Open Data
- Public APIs
token_urls:
- https://signin.nasdaq.com/oauth2/austt9dkdogT6EFRB417/v1/token
---
