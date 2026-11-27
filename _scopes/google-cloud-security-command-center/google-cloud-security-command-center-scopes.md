---
api_specs:
- filename: google-cloud-security-command-center-folders-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Folders API
  slug: google-cloud-security-command-center-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-security-command-center/openapi/google-cloud-security-command-center-folders-api-openapi.yml
- filename: google-cloud-security-command-center-organizations-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Organizations API
  slug: google-cloud-security-command-center-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-security-command-center/openapi/google-cloud-security-command-center-organizations-api-openapi.yml
- filename: google-cloud-security-command-center-projects-api-openapi.yml
  format: yaml
  label: Google Cloud Security Command Center Projects API
  slug: google-cloud-security-command-center-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-cloud-security-command-center/openapi/google-cloud-security-command-center-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Cloud Security Command Center Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Cloud Security Command Center publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Cloud Security Command Center API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Cloud Security Command Center
provider_slug: google-cloud-security-command-center
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-security-command-center-securitycenter-folders-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-security-command-center-securitycenter-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-security-command-center-securitycenter-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-security-command-center-securityposture-organizations-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-cloud-security-command-center-websecurityscanner-projects-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/securitycenter
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: See, edit, configure, and delete your Google Cloud Security Command Center data and see the email address for your Google Account
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/securitycenter
slug: google-cloud-security-command-center-scopes
source_filename: google-cloud-security-command-center-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-cloud-security-command-center-securitycenter-folders-api-openapi.yml,\n  openapi/google-cloud-security-command-center-securitycenter-organizations-api-openapi.yml,\n  openapi/google-cloud-security-command-center-securitycenter-projects-api-openapi.yml, openapi/google-cloud-security-command-center-securityposture-organizations-api-openapi.yml,\n  openapi/google-cloud-security-command-center-websecurityscanner-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-cloud-security-command-center-securitycenter-folders-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-security-command-center-securitycenter-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-security-command-center-securitycenter-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-security-command-center-securityposture-organizations-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-cloud-security-command-center-websecurityscanner-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data\
  \ and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-security-command-center-securitycenter-folders-api-openapi.yml\n  - openapi/google-cloud-security-command-center-securitycenter-organizations-api-openapi.yml\n  - openapi/google-cloud-security-command-center-securitycenter-projects-api-openapi.yml\n  - openapi/google-cloud-security-command-center-securityposture-organizations-api-openapi.yml\n  - openapi/google-cloud-security-command-center-websecurityscanner-projects-api-openapi.yml\n- scope: https://www.googleapis.com/auth/securitycenter\n  description: See, edit, configure, and delete your Google Cloud Security Command Center data\n    and see the email address for your Google Account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-cloud-security-command-center-securitycenter-folders-api-openapi.yml\n  - openapi/google-cloud-security-command-center-securitycenter-organizations-api-openapi.yml\n\
  \  - openapi/google-cloud-security-command-center-securitycenter-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-cloud-security-command-center/scopes/google-cloud-security-command-center-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Cloud Security
- Compliance
- Risk Management
- Security
- Threat Detection
- Vulnerability Management
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
