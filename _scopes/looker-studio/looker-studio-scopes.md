---
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Looker Studio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Looker Studio publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Looker Studio API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Looker Studio
provider_slug: looker-studio
schemes:
- description: OAuth 2.0 authentication with domain-wide delegation. Requires Google Workspace or Cloud Identity organization.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/looker-studio-api-openapi.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/datastudio
- https://www.googleapis.com/auth/datastudio.readonly
- https://www.googleapis.com/auth/userinfo.profile
scopes:
- description: Full access to manage Looker Studio assets and permissions.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datastudio
- description: Read-only access to Looker Studio assets.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/datastudio.readonly
- description: Access to user profile information.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/userinfo.profile
slug: looker-studio-scopes
source_filename: looker-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/looker-studio-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/looker-studio-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication with domain-wide delegation. Requires Google Workspace\n    or Cloud Identity organization.\nscopes:\n- scope: https://www.googleapis.com/auth/datastudio\n  description: Full access to manage Looker Studio assets and permissions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/looker-studio-api-openapi.yml\n- scope: https://www.googleapis.com/auth/datastudio.readonly\n  description: Read-only access to Looker Studio assets.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/looker-studio-api-openapi.yml\n- scope: https://www.googleapis.com/auth/userinfo.profile\n  description: Access to user profile information.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/looker-studio-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/scopes/looker-studio-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
token_urls:
- https://oauth2.googleapis.com/token
---
