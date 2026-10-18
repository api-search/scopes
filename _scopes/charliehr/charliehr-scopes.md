---
api_specs:
- filename: charliehr-company-api-openapi.yml
  format: yaml
  label: CharlieHR Company API
  slug: charliehr-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-company-api-openapi.yml
- filename: charliehr-leave-absences-api-openapi.yml
  format: yaml
  label: CharlieHR Leave / Absences API
  slug: charliehr-leave-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-leave-absences-api-openapi.yml
- filename: charliehr-leave-allowances-api-openapi.yml
  format: yaml
  label: CharlieHR Leave Allowances API
  slug: charliehr-leave-allowances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-leave-allowances-api-openapi.yml
- filename: charliehr-team-members-api-openapi.yml
  format: yaml
  label: CharlieHR Team Members API
  slug: charliehr-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/openapi/charliehr-team-members-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Charliehr Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'CharlieHR uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://charliehr.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CharlieHR
provider_slug: charliehr
schemes:
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  source: openapi/charliehr-company-api-openapi.yml
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  source: openapi/charliehr-leave-absences-api-openapi.yml
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  source: openapi/charliehr-leave-allowances-api-openapi.yml
- description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged for an access token, which is sent in the Authorization header of each request.
  flows:
  - flow: clientCredentials
    tokenUrl: https://charliehr.com/oauth/token
  name: oauth2
  source: openapi/charliehr-team-members-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: charliehr-scopes
source_filename: charliehr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/charliehr-company-api-openapi.yml, openapi/charliehr-leave-absences-api-openapi.yml,\n  openapi/charliehr-leave-allowances-api-openapi.yml, openapi/charliehr-team-members-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/charliehr-company-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\n- name: oauth2\n  source: openapi/charliehr-leave-absences-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\n- name: oauth2\n  source: openapi/charliehr-leave-allowances-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\n- name: oauth2\n  source: openapi/charliehr-team-members-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://charliehr.com/oauth/token\n  description: OAuth 2.0. A Client ID and Client Secret issued in the CharlieHR app are exchanged\n    for an access token, which is sent in the Authorization header of each request.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charliehr/refs/heads/main/scopes/charliehr-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Human Resources
- HRIS
- People
- Leave
- Time Off
token_bound: false
token_urls:
- https://charliehr.com/oauth/token
---
