---
api_specs:
- filename: clever-data-api-openapi.yml
  format: yaml
  label: Clever Data API
  slug: clever-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-data-api-openapi.yml
- filename: clever-lms-connect-api-openapi.yml
  format: yaml
  label: Clever LMS Connect API
  slug: clever-lms-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-lms-connect-api-openapi.yml
- filename: clever-events-api-openapi.yml
  format: yaml
  label: Clever Events API
  slug: clever-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-events-api-openapi.yml
authorization_urls:
- https://clever.com/oauth/authorize
description: ''
docs: https://dev.clever.com/docs/setting-up-district-sso
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clever Scopes
name_suffix: OAuth Scopes
note: Clever manages scopes through application configuration rather than client-requested scope parameters (https://dev.clever.com/docs/oidc-implementation); the documented Clever Single Sign-On access tier scopes are listed below, while full Data API roster access uses district-app tokens instead of OAuth scopes.
overview: 'Clever publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clever API on a user''s behalf.


  Tokens are issued from https://clever.com/oauth/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clever
provider_slug: clever
schemes:
- flows:
  - authorizationUrl: https://clever.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clever.com/oauth/tokens
  name: oauth
  source: openapi/clever-data-api-openapi.yml
- flows:
  - authorizationUrl: https://clever.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clever.com/oauth/tokens
  name: oauth
  source: openapi/clever-events-api-openapi.yml
- flows:
  - authorizationUrl: https://clever.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clever.com/oauth/tokens
  name: oauth
  source: openapi/clever-lms-connect-api-openapi.yml
scope_count: 5
scope_names:
- read:user_id
- read:students_basic
- read:teachers_basic
- read:school_admins_basic
- read:district_admins_basic
scopes:
- description: Read the authorizing user's Clever user identifier via the /me endpoint; part of the Clever Single Sign-On access tier.
  flows: []
  scope: read:user_id
- description: Read basic student information for the authorizing user; part of the Clever Single Sign-On access tier.
  flows: []
  scope: read:students_basic
- description: Read basic teacher information for the authorizing user; part of the Clever Single Sign-On access tier.
  flows: []
  scope: read:teachers_basic
- description: Read basic school administrator information for the authorizing user; part of the Clever Single Sign-On access tier.
  flows: []
  scope: read:school_admins_basic
- description: Read basic district administrator information for the authorizing user; part of the Clever Single Sign-On access tier.
  flows: []
  scope: read:district_admins_basic
slug: clever-scopes
source_filename: clever-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\ndocs: https://dev.clever.com/docs/setting-up-district-sso\nnote: Clever manages scopes through application configuration rather than client-requested\n  scope parameters (https://dev.clever.com/docs/oidc-implementation); the documented\n  Clever Single Sign-On access tier scopes are listed below, while full Data API roster\n  access uses district-app tokens instead of OAuth scopes.\nsource: openapi/clever-data-api-openapi.yml, openapi/clever-events-api-openapi.yml, openapi/clever-lms-connect-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/clever-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clever.com/oauth/authorize\n    tokenUrl: https://clever.com/oauth/tokens\n- name: oauth\n  source: openapi/clever-events-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clever.com/oauth/authorize\n    tokenUrl: https://clever.com/oauth/tokens\n- name:\
  \ oauth\n  source: openapi/clever-lms-connect-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clever.com/oauth/authorize\n    tokenUrl: https://clever.com/oauth/tokens\nscopes:\n- scope: read:user_id\n  description: Read the authorizing user's Clever user identifier via the /me endpoint;\n    part of the Clever Single Sign-On access tier.\n  sources:\n  - https://dev.clever.com/docs/setting-up-district-sso\n- scope: read:students_basic\n  description: Read basic student information for the authorizing user; part of the\n    Clever Single Sign-On access tier.\n  sources:\n  - https://dev.clever.com/docs/setting-up-district-sso\n- scope: read:teachers_basic\n  description: Read basic teacher information for the authorizing user; part of the\n    Clever Single Sign-On access tier.\n  sources:\n  - https://dev.clever.com/docs/setting-up-district-sso\n- scope: read:school_admins_basic\n  description: Read basic school administrator information for the authorizing\
  \ user;\n    part of the Clever Single Sign-On access tier.\n  sources:\n  - https://dev.clever.com/docs/setting-up-district-sso\n- scope: read:district_admins_basic\n  description: Read basic district administrator information for the authorizing\n    user; part of the Clever Single Sign-On access tier.\n  sources:\n  - https://dev.clever.com/docs/setting-up-district-sso\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/scopes/clever-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Education
- K-12
- EdTech
- Single Sign-On
- Rostering
- Identity
- SSO
- Student Data
- LMS
- SIS
token_urls:
- https://clever.com/oauth/tokens
---
