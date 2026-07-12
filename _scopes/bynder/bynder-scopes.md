---
authorization_urls:
- https://yourportal.bynder.com/v6/authentication/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bynder Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bynder publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bynder API on a user''s behalf.


  Tokens are issued from https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bynder
provider_slug: bynder
schemes:
- description: OAuth 2.0 with JWT bearer access tokens
  flows:
  - authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
  - flow: clientCredentials
    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
  name: oauth2
  source: openapi/bynder-openapi.yml
scope_count: 7
scope_names:
- asset:read
- asset:write
- collection:read
- collection:write
- meta.assetbank:read
- meta.assetbank:write
- offline
scopes:
- description: Read assets
  flows:
  - authorizationCode
  - clientCredentials
  scope: asset:read
- description: Write assets
  flows:
  - authorizationCode
  - clientCredentials
  scope: asset:write
- description: Read collections
  flows:
  - authorizationCode
  scope: collection:read
- description: Write collections
  flows:
  - authorizationCode
  scope: collection:write
- description: Read asset bank metaproperties
  flows:
  - authorizationCode
  scope: meta.assetbank:read
- description: Write asset bank metaproperties
  flows:
  - authorizationCode
  scope: meta.assetbank:write
- description: Refresh token access
  flows:
  - authorizationCode
  scope: offline
slug: bynder-scopes
source_filename: bynder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bynder-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bynder-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourportal.bynder.com/v6/authentication/oauth2/auth\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization\n  - flow: clientCredentials\n    tokenUrl: https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials\n  description: OAuth 2.0 with JWT bearer access tokens\nscopes:\n- scope: asset:read\n  description: Read assets\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: asset:write\n  description: Write assets\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: collection:read\n  description: Read collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope:\
  \ collection:write\n  description: Write collections\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: meta.assetbank:read\n  description: Read asset bank metaproperties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: meta.assetbank:write\n  description: Write asset bank metaproperties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n- scope: offline\n  description: Refresh token access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bynder-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/scopes/bynder-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- Digital Asset Management
- DAM
- Brand Management
- Content Management
- Marketing
token_urls:
- https://yourportal.bynder.com/v6/authentication/oauth2/token/authorization
- https://yourportal.bynder.com/v6/authentication/oauth2/token/client-credentials
---
