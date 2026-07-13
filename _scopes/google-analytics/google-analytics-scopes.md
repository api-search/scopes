---
api_specs:
- filename: google-analytics-data-api.yaml
  format: yaml
  label: Google Analytics Data API (GA4)
  slug: google-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-data-api.yaml
- filename: google-analytics-admin-api.yaml
  format: yaml
  label: Google Analytics Admin API
  slug: google-analytics-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-admin-api.yaml
- filename: google-analytics-measurement-protocol.yaml
  format: yaml
  label: Google Analytics Measurement Protocol (GA4)
  slug: google-analytics-measurement-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-measurement-protocol.yaml
- filename: google-analytics-user-deletion-api.yaml
  format: yaml
  label: Google Analytics User Deletion API
  slug: google-analytics-user-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-user-deletion-api.yaml
- filename: google-analytics-reporting-api-v4.yaml
  format: yaml
  label: Google Analytics Reporting API v4 (Universal Analytics)
  slug: google-analytics-reporting-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-reporting-api-v4.yaml
- filename: google-analytics-management-api-v3.yaml
  format: yaml
  label: Google Analytics Management API v3
  slug: google-analytics-management-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/openapi/google-analytics-management-api-v3.yaml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- implicit
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Analytics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Analytics publishes 7 OAuth 2.0 scopes via the implicit and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Analytics API on a user''s behalf.


  Tokens are issued from https://accounts.google.com/o/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Analytics
provider_slug: google-analytics
schemes:
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-analytics-admin-api.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-analytics-admin-api.yaml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-analytics-data-api.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-analytics-data-api.yaml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-analytics-management-api-v3.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-analytics-management-api-v3.yaml
- description: Oauth 2.0 implicit authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: implicit
  name: Oauth2
  source: openapi/google-analytics-reporting-api-v4.yaml
- description: Oauth 2.0 authorizationCode authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://accounts.google.com/o/oauth2/token
  name: Oauth2c
  source: openapi/google-analytics-reporting-api-v4.yaml
- description: OAuth 2.0 authentication
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-analytics-user-deletion-api.yaml
scope_count: 7
scope_names:
- https://www.googleapis.com/auth/analytics
- https://www.googleapis.com/auth/analytics.edit
- https://www.googleapis.com/auth/analytics.manage.users
- https://www.googleapis.com/auth/analytics.manage.users.readonly
- https://www.googleapis.com/auth/analytics.provision
- https://www.googleapis.com/auth/analytics.readonly
- https://www.googleapis.com/auth/analytics.user.deletion
scopes:
- description: View and manage your Google Analytics data
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics
- description: Edit Google Analytics management entities
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.edit
- description: Manage Google Analytics Account users by email address
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.manage.users
- description: View Google Analytics user permissions
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.manage.users.readonly
- description: Create a new Google Analytics account along with its default property and view
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.provision
- description: See and download your Google Analytics data
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.readonly
- description: Manage Google Analytics user deletion requests
  flows:
  - authorizationCode
  - implicit
  scope: https://www.googleapis.com/auth/analytics.user.deletion
slug: google-analytics-scopes
source_filename: google-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/google-analytics-admin-api.yaml, openapi/google-analytics-data-api.yaml, openapi/google-analytics-management-api-v3.yaml,\n  openapi/google-analytics-reporting-api-v4.yaml, openapi/google-analytics-user-deletion-api.yaml\nschemes:\n- name: Oauth2\n  source: openapi/google-analytics-admin-api.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-analytics-admin-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-analytics-data-api.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n\
  - name: Oauth2c\n  source: openapi/google-analytics-data-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-analytics-management-api-v3.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit authentication\n- name: Oauth2c\n  source: openapi/google-analytics-management-api-v3.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: Oauth2\n  source: openapi/google-analytics-reporting-api-v4.yaml\n  flows:\n  - flow: implicit\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n  description: Oauth 2.0 implicit\
  \ authentication\n- name: Oauth2c\n  source: openapi/google-analytics-reporting-api-v4.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://accounts.google.com/o/oauth2/token\n  description: Oauth 2.0 authorizationCode authentication\n- name: oauth2\n  source: openapi/google-analytics-user-deletion-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 authentication\nscopes:\n- scope: https://www.googleapis.com/auth/analytics\n  description: View and manage your Google Analytics data\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-data-api.yaml\n  - openapi/google-analytics-management-api-v3.yaml\n  - openapi/google-analytics-reporting-api-v4.yaml\n- scope: https://www.googleapis.com/auth/analytics.edit\n  description: Edit Google Analytics\
  \ management entities\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-admin-api.yaml\n  - openapi/google-analytics-management-api-v3.yaml\n- scope: https://www.googleapis.com/auth/analytics.manage.users\n  description: Manage Google Analytics Account users by email address\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-management-api-v3.yaml\n- scope: https://www.googleapis.com/auth/analytics.manage.users.readonly\n  description: View Google Analytics user permissions\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-management-api-v3.yaml\n- scope: https://www.googleapis.com/auth/analytics.provision\n  description: Create a new Google Analytics account along with its default property and view\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-management-api-v3.yaml\n- scope: https://www.googleapis.com/auth/analytics.readonly\n\
  \  description: See and download your Google Analytics data\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-admin-api.yaml\n  - openapi/google-analytics-data-api.yaml\n  - openapi/google-analytics-management-api-v3.yaml\n  - openapi/google-analytics-reporting-api-v4.yaml\n- scope: https://www.googleapis.com/auth/analytics.user.deletion\n  description: Manage Google Analytics user deletion requests\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - openapi/google-analytics-management-api-v3.yaml\n  - openapi/google-analytics-user-deletion-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/scopes/google-analytics-scopes.yml
summary_line: 7 scopes · implicit/authorizationCode
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
token_urls:
- https://accounts.google.com/o/oauth2/token
- https://oauth2.googleapis.com/token
---
