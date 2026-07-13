---
api_specs:
- filename: google-chrome-management-api-openapi.json
  format: json
  label: Chrome Management API
  slug: chrome-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/openapi/google-chrome-management-api-openapi.json
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Chrome Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Chrome publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Chrome API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Chrome
provider_slug: google-chrome
schemes:
- description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-chrome-management-api-openapi.json
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/chrome.management.appdetails.readonly
- https://www.googleapis.com/auth/chrome.management.reports.readonly
- https://www.googleapis.com/auth/chrome.management.telemetry.readonly
scopes:
- description: View Chrome app details
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chrome.management.appdetails.readonly
- description: View Chrome browser and device reports
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chrome.management.reports.readonly
- description: View Chrome telemetry data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/chrome.management.telemetry.readonly
slug: google-chrome-scopes
source_filename: google-chrome-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-chrome-management-api-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/google-chrome-management-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: Google OAuth 2.0 authentication. Requires appropriate Chrome Management API scopes.\nscopes:\n- scope: https://www.googleapis.com/auth/chrome.management.appdetails.readonly\n  description: View Chrome app details\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chrome-management-api-openapi.json\n- scope: https://www.googleapis.com/auth/chrome.management.reports.readonly\n  description: View Chrome browser and device reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chrome-management-api-openapi.json\n- scope: https://www.googleapis.com/auth/chrome.management.telemetry.readonly\n \
  \ description: View Chrome telemetry data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-chrome-management-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-chrome/refs/heads/main/scopes/google-chrome-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Browser
- Chrome Extensions
- Developer Tools
- Web Platform
token_urls:
- https://oauth2.googleapis.com/token
---
