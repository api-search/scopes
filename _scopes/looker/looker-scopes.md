---
api_specs:
- filename: looker-projects-api-openapi.yml
  format: yaml
  label: Looker Projects API
  slug: looker-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/looker/openapi/looker-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Looker Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Looker publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Looker API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Looker
provider_slug: looker
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/looker-projects-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: looker-scopes
source_filename: looker-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/looker-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/looker-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/looker-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/looker/scopes/looker-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
