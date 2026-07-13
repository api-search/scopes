---
api_specs:
- filename: cognite-data-fusion-api.yaml
  format: yaml
  label: Cognite Data Fusion API
  slug: cognite-data-fusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/openapi/cognite-data-fusion-api.yaml
authorization_urls:
- https://your-idps.authorization.url/
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cognite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cognite publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cognite API on a user''s behalf.


  Tokens are issued from https://your-idps.token.url/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cognite
provider_slug: cognite
schemes:
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://your-idps.token.url/
  name: oauth2-client-credentials
  source: openapi/cognite-data-fusion-api.json
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - authorizationUrl: https://your-idps.authorization.url/
    flow: authorizationCode
    tokenUrl: https://your-idps.token.url/
  name: oauth2-auth-code
  source: openapi/cognite-data-fusion-api.json
- description: Auth flow for Open Industrial Data. Get your client secret from https://hub.cognite.com/open-industrial-data-211.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/48d5043c-cf70-4c49-881c-c638f5796997/oauth2/v2.0/token
  name: oauth2-open-industrial-data
  source: openapi/cognite-data-fusion-api.json
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - flow: clientCredentials
    tokenUrl: https://your-idps.token.url/
  name: oauth2-client-credentials
  source: openapi/cognite-data-fusion-api.yaml
- description: Access token issued by the CDF project's configured identity provider. Access token must be an OpenID Connect token, and the project must be configured to accept OpenID Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'. The token can be obtained through any flow supported by the identity provider.
  flows:
  - authorizationUrl: https://your-idps.authorization.url/
    flow: authorizationCode
    tokenUrl: https://your-idps.token.url/
  name: oauth2-auth-code
  source: openapi/cognite-data-fusion-api.yaml
- description: Auth flow for Open Industrial Data. Get your client secret from https://hub.cognite.com/open-industrial-data-211.
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/48d5043c-cf70-4c49-881c-c638f5796997/oauth2/v2.0/token
  name: oauth2-open-industrial-data
  source: openapi/cognite-data-fusion-api.yaml
scope_count: 3
scope_names:
- default
- https://api.cognitedata.com/.default
- https://{cluster}.cognitedata.com/.default
scopes:
- description: https://{cluster}.cognitedata.com/.default
  flows:
  - authorizationCode
  - clientCredentials
  scope: default
- description: ''
  flows: []
  scope: https://api.cognitedata.com/.default
- description: ''
  flows: []
  scope: https://{cluster}.cognitedata.com/.default
slug: cognite-scopes
source_filename: cognite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cognite-data-fusion-api.json, openapi/cognite-data-fusion-api.yaml\nschemes:\n- name: oauth2-client-credentials\n  source: openapi/cognite-data-fusion-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-idps.token.url/\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n- name: oauth2-auth-code\n  source: openapi/cognite-data-fusion-api.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-idps.authorization.url/\n    tokenUrl: https://your-idps.token.url/\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token\
  \ must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n- name: oauth2-open-industrial-data\n  source: openapi/cognite-data-fusion-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/48d5043c-cf70-4c49-881c-c638f5796997/oauth2/v2.0/token\n  description: Auth flow for Open Industrial Data. Get your client secret from https://hub.cognite.com/open-industrial-data-211.\n- name: oauth2-client-credentials\n  source: openapi/cognite-data-fusion-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://your-idps.token.url/\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens.\
  \ Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n- name: oauth2-auth-code\n  source: openapi/cognite-data-fusion-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://your-idps.authorization.url/\n    tokenUrl: https://your-idps.token.url/\n  description: Access token issued by the CDF project's configured identity provider. Access\n    token must be an OpenID Connect token, and the project must be configured to accept OpenID\n    Connect tokens. Use a header key of 'Authorization' with a value of 'Bearer $accesstoken'.\n    The token can be obtained through any flow supported by the identity provider.\n- name: oauth2-open-industrial-data\n  source: openapi/cognite-data-fusion-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/48d5043c-cf70-4c49-881c-c638f5796997/oauth2/v2.0/token\n  description: Auth flow\
  \ for Open Industrial Data. Get your client secret from https://hub.cognite.com/open-industrial-data-211.\nscopes:\n- scope: default\n  description: https://{cluster}.cognitedata.com/.default\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n- scope: https://api.cognitedata.com/.default\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n- scope: https://{cluster}.cognitedata.com/.default\n  sources:\n  - openapi/cognite-data-fusion-api.json\n  - openapi/cognite-data-fusion-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognite/refs/heads/main/scopes/cognite-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Industrial IoT
- Manufacturing
- Industrial Data
- Digital Twin
- Asset Management
- Time Series
- Industrial AI
token_urls:
- https://your-idps.token.url/
- https://login.microsoftonline.com/48d5043c-cf70-4c49-881c-c638f5796997/oauth2/v2.0/token
---
