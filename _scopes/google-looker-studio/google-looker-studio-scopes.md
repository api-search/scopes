---
api_specs:
- filename: google-looker-studio-assets-search-api-openapi.yml
  format: yaml
  label: Google Looker Studio Assets:search API
  slug: google-looker-studio-assets-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/openapi/google-looker-studio-assets-search-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: https://developers.google.com/looker-studio/api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Google Looker Studio Scopes
name_suffix: OAuth Scopes
note: The provider documents the fully-qualified scope URIs; the OpenAPI declares only the short suffixes. Both forms are recorded below so a client generated from either source resolves. Scopes are attached to the OAuth client by a Workspace admin during domain-wide delegation, not declared by the app.
overview: 'Google Looker Studio publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Looker Studio API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Looker Studio
provider_slug: google-looker-studio
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-looker-studio-assets-search-api-openapi.yml
scope_count: 3
scope_names:
- datastudio
- datastudio.readonly
- userinfo.profile
scopes:
- description: View and manage Looker Studio assets.
  flows:
  - authorizationCode
  scope: datastudio
- description: View Looker Studio assets.
  flows:
  - authorizationCode
  scope: datastudio.readonly
- description: View profile information.
  flows:
  - authorizationCode
  scope: userinfo.profile
slug: google-looker-studio-scopes
source_filename: google-looker-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: openapi/google-looker-studio-assets-search-api-openapi.yml\ndocs: https://developers.google.com/looker-studio/api\nevidence:\n- url: https://developers.google.com/looker-studio/api\n  status: 200\n  kind: provider scope list and least-privilege guidance\n- url: https://developers.google.com/looker-studio/integrate/api/reference/assets/search\n  status: 200\n  kind: per-operation scope requirement\nnote: >-\n  The provider documents the fully-qualified scope URIs; the OpenAPI declares only the short\n  suffixes. Both forms are recorded below so a client generated from either source resolves.\n  Scopes are attached to the OAuth client by a Workspace admin during domain-wide delegation, not\n  declared by the app.\nschemes:\n- name: OAuth2\n  source: openapi/google-looker-studio-assets-search-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl:\
  \ https://oauth2.googleapis.com/token\nscopes:\n- scope: datastudio\n  uri: https://www.googleapis.com/auth/datastudio\n  description: View and manage Looker Studio assets.\n  level: read-write\n  required_for:\n  - PATCH /v1/assets/{assetName}/permissions\n  - POST /v1/assets/{assetName}/permissions:addMembers\n  - POST /v1/assets/{assetName}/permissions:revokeAllPermissions\n  also_accepted_for:\n  - GET /v1/assets:search\n  - GET /v1/assets/{assetName}/permissions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-assets-search-api-openapi.yml\n  - https://developers.google.com/looker-studio/api\n- scope: datastudio.readonly\n  uri: https://www.googleapis.com/auth/datastudio.readonly\n  description: View Looker Studio assets.\n  level: read-only\n  required_for: []\n  also_accepted_for:\n  - GET /v1/assets:search\n  - GET /v1/assets/{assetName}/permissions\n  provider_guidance: >-\n    \"If your app doesn't need to manage Data Studio assets, consider using\
  \ the more restrictive\n    https://www.googleapis.com/auth/datastudio.readonly scope instead of\n    https://www.googleapis.com/auth/datastudio.\"\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-assets-search-api-openapi.yml\n  - https://developers.google.com/looker-studio/api\n- scope: userinfo.profile\n  uri: https://www.googleapis.com/auth/userinfo.profile\n  description: View profile information.\n  level: read-only\n  note: >-\n    Listed by the provider among the scopes \"commonly requested if using the Data Studio API to\n    manage assets\", alongside the datastudio scope. Not required by any documented operation.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-assets-search-api-openapi.yml\n  - https://developers.google.com/looker-studio/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker-studio/refs/heads/main/scopes/google-looker-studio-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Looker
- Reporting
token_urls:
- https://oauth2.googleapis.com/token
---
