---
api_specs:
- filename: ms-products-openapi.yml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ms-products/refs/heads/main/openapi/ms-products-openapi.yml
authorization_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ms Products Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Microsoft Products APIs publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Microsoft Products APIs API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/common/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Microsoft Products APIs
provider_slug: ms-products
schemes:
- description: 'Microsoft identity platform OAuth 2.0. Acquire access tokens from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token and send as `Authorization: Bearer <token>`.'
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: oauth2
  source: openapi/ms-products-openapi.yml
scope_count: 1
scope_names:
- https://graph.microsoft.com/.default
scopes:
- description: Default app permissions
  flows:
  - authorizationCode
  - clientCredentials
  scope: https://graph.microsoft.com/.default
slug: ms-products-scopes
source_filename: ms-products-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ms-products-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/ms-products-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n  description: 'Microsoft identity platform OAuth 2.0. Acquire access tokens from https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    and send as `Authorization: Bearer <token>`.'\nscopes:\n- scope: https://graph.microsoft.com/.default\n  description: Default app permissions\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/ms-products-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ms-products/refs/heads/main/scopes/ms-products-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Azure
- Cloud
- Enterprise
- Microsoft
- Office 365
- Productivity
token_urls:
- https://login.microsoftonline.com/common/oauth2/v2.0/token
---
