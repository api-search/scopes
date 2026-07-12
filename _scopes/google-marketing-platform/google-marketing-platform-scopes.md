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
name: Google Marketing Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Marketing Platform Admin publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Marketing Platform Admin API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Marketing Platform Admin
provider_slug: google-marketing-platform
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/marketingplatformadmin.analytics.read
- https://www.googleapis.com/auth/marketingplatformadmin.analytics.update
scopes:
- description: View Analytics links
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.read
- description: Manage Analytics links
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.update
slug: google-marketing-platform-scopes
source_filename: google-marketing-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.read\n  description: View Analytics links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n- scope: https://www.googleapis.com/auth/marketingplatformadmin.analytics.update\n  description: Manage Analytics links\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-marketing-platform/refs/heads/main/scopes/google-marketing-platform-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Google Marketing Platform
- Marketing
- Organization Management
- Platform Administration
token_urls:
- https://oauth2.googleapis.com/token
---
