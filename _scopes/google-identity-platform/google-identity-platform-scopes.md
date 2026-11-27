---
api_specs:
- filename: google-identity-platform-accounts-api-openapi.yml
  format: yaml
  label: Google Identity Platform Accounts API
  slug: google-identity-platform-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-identity-platform/openapi/google-identity-platform-accounts-api-openapi.yml
- filename: google-identity-platform-projects-api-openapi.yml
  format: yaml
  label: Google Identity Platform Identity Platform Projects API
  slug: google-identity-platform-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-identity-platform/openapi/google-identity-platform-projects-api-openapi.yml
- filename: google-identity-platform-defaultsupportedidps-api-openapi.yml
  format: yaml
  label: Google Identity Platform Default Supported Idps API
  slug: google-identity-platform-defaultsupportedidps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-identity-platform/openapi/google-identity-platform-defaultsupportedidps-api-openapi.yml
- filename: google-identity-platform-recaptchaconfig-api-openapi.yml
  format: yaml
  label: Google Identity Platform Recaptcha Config API
  slug: google-identity-platform-recaptchaconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-identity-platform/openapi/google-identity-platform-recaptchaconfig-api-openapi.yml
- filename: google-identity-platform-password-policy-api-openapi.yml
  format: yaml
  label: Google Identity Platform Password Policy API
  slug: google-identity-platform-password-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-identity-platform/openapi/google-identity-platform-password-policy-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Identity Platform Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Identity Platform publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Identity Platform API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Identity Platform
provider_slug: google-identity-platform
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-identity-platform-accounts-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-identity-platform-default-supported-idps-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-identity-platform-projects-api-openapi.yml
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-identity-platform-v2-api-openapi.yml
scope_count: 2
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/firebase
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View and administer all your Firebase data and settings
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/firebase
slug: google-identity-platform-scopes
source_filename: google-identity-platform-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-identity-platform-accounts-api-openapi.yml, openapi/google-identity-platform-default-supported-idps-api-openapi.yml,\n  openapi/google-identity-platform-projects-api-openapi.yml, openapi/google-identity-platform-v2-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-identity-platform-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-identity-platform-default-supported-idps-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-identity-platform-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n\
  \    tokenUrl: https://oauth2.googleapis.com/token\n- name: oauth2\n  source: openapi/google-identity-platform-v2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-identity-platform-accounts-api-openapi.yml\n  - openapi/google-identity-platform-default-supported-idps-api-openapi.yml\n  - openapi/google-identity-platform-projects-api-openapi.yml\n  - openapi/google-identity-platform-v2-api-openapi.yml\n- scope: https://www.googleapis.com/auth/firebase\n  description: View and administer all your Firebase data and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-identity-platform-accounts-api-openapi.yml\n\
  \  - openapi/google-identity-platform-default-supported-idps-api-openapi.yml\n  - openapi/google-identity-platform-projects-api-openapi.yml\n  - openapi/google-identity-platform-v2-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-identity-platform/scopes/google-identity-platform-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Authentication
- Google Cloud
- Identity
- Multi-Tenancy
- OpenID Connect
- SAML
- Identity Federation
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
