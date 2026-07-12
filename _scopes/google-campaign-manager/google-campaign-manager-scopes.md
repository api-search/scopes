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
name: Google Campaign Manager Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Campaign Manager publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Campaign Manager API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schemes:
- description: OAuth 2.0 authentication for accessing Campaign Manager 360 resources. Requires appropriate scopes for trafficking or reporting operations.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/google-campaign-manager-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/dfareporting
- https://www.googleapis.com/auth/dfatrafficking
scopes:
- description: View and manage DoubleClick for Advertisers reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dfareporting
- description: View and manage your DoubleClick Campaign Manager's (DCM) display ad campaigns
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dfatrafficking
slug: google-campaign-manager-scopes
source_filename: google-campaign-manager-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-campaign-manager-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/google-campaign-manager-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication for accessing Campaign Manager 360 resources. Requires\n    appropriate scopes for trafficking or reporting operations.\nscopes:\n- scope: https://www.googleapis.com/auth/dfareporting\n  description: View and manage DoubleClick for Advertisers reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-campaign-manager-openapi.yml\n- scope: https://www.googleapis.com/auth/dfatrafficking\n  description: View and manage your DoubleClick Campaign Manager's (DCM) display ad campaigns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-campaign-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/scopes/google-campaign-manager-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
token_urls:
- https://oauth2.googleapis.com/token
---
