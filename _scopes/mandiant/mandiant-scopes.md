---
api_specs:
- filename: mandiant-projects-api-openapi.yml
  format: yaml
  label: Mandiant Projects API
  slug: mandiant-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mandiant/openapi/mandiant-projects-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mandiant Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mandiant publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mandiant API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mandiant
provider_slug: mandiant
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/mandiant-projects-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: See, edit, configure, and delete your Google Cloud data and see the email address for your Google Account.
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
slug: mandiant-scopes
source_filename: mandiant-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/mandiant-projects-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/mandiant-projects-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: See, edit, configure, and delete your Google Cloud data and see the email address\n    for your Google Account.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mandiant-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mandiant/scopes/mandiant-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Incident Response
- Attack Surface Management
- Vulnerability Intelligence
- Malware
- Google Cloud
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
