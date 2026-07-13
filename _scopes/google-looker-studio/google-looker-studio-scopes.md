---
api_specs:
- filename: rest
  format: yaml
  label: Google Looker Studio API
  slug: google-looker-studio-api
  spec_type: OpenAPI
  url: https://lookerstudio.googleapis.com/$discovery/rest
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Looker Studio Scopes
name_suffix: OAuth Scopes
note: ''
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
  source: openapi/google-looker-studio-openapi.yml
scope_count: 3
scope_names:
- datastudio
- datastudio.readonly
- userinfo.profile
scopes:
- description: View and manage Looker Studio assets
  flows:
  - authorizationCode
  scope: datastudio
- description: View Looker Studio assets
  flows:
  - authorizationCode
  scope: datastudio.readonly
- description: View profile information
  flows:
  - authorizationCode
  scope: userinfo.profile
slug: google-looker-studio-scopes
source_filename: google-looker-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-looker-studio-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-looker-studio-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: datastudio\n  description: View and manage Looker Studio assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-openapi.yml\n- scope: datastudio.readonly\n  description: View Looker Studio assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-openapi.yml\n- scope: userinfo.profile\n  description: View profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-looker-studio-openapi.yml\n"
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
