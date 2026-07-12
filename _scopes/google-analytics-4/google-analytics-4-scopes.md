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
name: Google Analytics 4 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Analytics 4 publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Analytics 4 API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Analytics 4
provider_slug: google-analytics-4
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-analytics-4-openapi.yml
scope_count: 2
scope_names:
- analytics
- analytics.readonly
scopes:
- description: View and manage Google Analytics data
  flows:
  - authorizationCode
  scope: analytics
- description: View Google Analytics data
  flows:
  - authorizationCode
  scope: analytics.readonly
slug: google-analytics-4-scopes
source_filename: google-analytics-4-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-analytics-4-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-analytics-4-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: analytics\n  description: View and manage Google Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-openapi.yml\n- scope: analytics.readonly\n  description: View Google Analytics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-analytics-4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics-4/refs/heads/main/scopes/google-analytics-4-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Analytics
- Data Collection
- Marketing
- Measurement
- Mobile Analytics
- Reporting
- Web Analytics
token_urls:
- https://oauth2.googleapis.com/token
---
