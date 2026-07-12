---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Data Studio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Data Studio publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Data Studio API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Data Studio
provider_slug: google-data-studio
schemes:
- description: OAuth 2.0 authentication. Requires domain-wide delegation configured by a Google Workspace administrator.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-data-studio-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/datastudio
- https://www.googleapis.com/auth/datastudio.readonly
- https://www.googleapis.com/auth/userinfo.profile
scopes:
- description: Full read and write access to Looker Studio assets and permissions.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datastudio
- description: Read-only access to Looker Studio assets and permissions.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datastudio.readonly
- description: Access to user profile information.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/userinfo.profile
slug: google-data-studio-scopes
source_filename: google-data-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-data-studio-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-data-studio-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication. Requires domain-wide delegation configured by a Google\n    Workspace administrator.\nscopes:\n- scope: https://www.googleapis.com/auth/datastudio\n  description: Full read and write access to Looker Studio assets and permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-data-studio-api-openapi.yml\n- scope: https://www.googleapis.com/auth/datastudio.readonly\n  description: Read-only access to Looker Studio assets and permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-data-studio-api-openapi.yml\n- scope: https://www.googleapis.com/auth/userinfo.profile\n  description:\
  \ Access to user profile information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-data-studio-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-data-studio/refs/heads/main/scopes/google-data-studio-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data
- Reporting
- Visualization
token_urls:
- https://oauth2.googleapis.com/token
---
