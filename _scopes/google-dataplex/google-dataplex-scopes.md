---
api_specs:
- filename: google-dataplex-projects-api-openapi.yml
  format: yaml
  label: Google Dataplex Projects API
  slug: google-dataplex-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dataplex/openapi/google-dataplex-projects-api-openapi.yml
- filename: google-dataplex-organizations-api-openapi.yml
  format: yaml
  label: Google Dataplex Dataplex Organizations API
  slug: google-dataplex-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-dataplex/openapi/google-dataplex-organizations-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Dataplex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Dataplex publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Dataplex API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Dataplex
provider_slug: google-dataplex
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-dataplex-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-dataplex-projects-api-openapi.yml
scope_count: 4
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/cloud-platform.read-only
- https://www.googleapis.com/auth/dataplex.read-write
- https://www.googleapis.com/auth/dataplex.readonly
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View your data across Google Cloud services and see the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform.read-only
- description: See, edit, configure, and delete your Google Cloud Dataplex data and see the email address for your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dataplex.read-write
- description: See your Google Cloud Dataplex data and the email address of your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/dataplex.readonly
slug: google-dataplex-scopes
source_filename: google-dataplex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/google-dataplex-organizations-api-openapi.yml, openapi/google-dataplex-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-dataplex-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-dataplex-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dataplex-organizations-api-openapi.yml\n  - openapi/google-dataplex-projects-api-openapi.yml\n- scope:\
  \ https://www.googleapis.com/auth/cloud-platform.read-only\n  description: View your data across Google Cloud services and see the email address of your\n    Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dataplex-organizations-api-openapi.yml\n  - openapi/google-dataplex-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/dataplex.read-write\n  description: See, edit, configure, and delete your Google Cloud Dataplex data and see the\n    email address for your Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dataplex-organizations-api-openapi.yml\n  - openapi/google-dataplex-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/dataplex.readonly\n  description: See your Google Cloud Dataplex data and the email address of your Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-dataplex-organizations-api-openapi.yml\n  - openapi/google-dataplex-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-dataplex/scopes/google-dataplex-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Data Governance
- Metadata Management
- Google Cloud
- AI Agents
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
