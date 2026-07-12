---
authorization_urls:
- https://oauth.employmenthero.com/oauth2/authorize
description: ''
docs: https://developer.employmenthero.com/api-references
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Employment Hero Scopes
name_suffix: OAuth Scopes
note: Employment Hero uses OAuth 2.0 scopes in URN form (e.g. urn:mainapp:organisations:read) selected once at application registration, but publishes no scopes reference — the docs state the scope list "will be provided by Employment Hero" via the Developer Portal (https://developer.employmenthero.com/api-references).
overview: 'Employment Hero uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://oauth.employmenthero.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Employment Hero
provider_slug: employment-hero
schemes:
- flows:
  - authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://oauth.employmenthero.com/oauth2/token
  name: oauth2
  source: openapi/employment-hero-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: employment-hero-scopes
source_filename: employment-hero-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/employment-hero-openapi.yml\ndocs: https://developer.employmenthero.com/api-references\nnote: >-\n  Employment Hero uses OAuth 2.0 scopes in URN form (e.g.\n  urn:mainapp:organisations:read) selected once at application registration,\n  but publishes no scopes reference — the docs state the scope list \"will be\n  provided by Employment Hero\" via the Developer Portal\n  (https://developer.employmenthero.com/api-references).\nschemes:\n- name: oauth2\n  source: openapi/employment-hero-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.employmenthero.com/oauth2/authorize\n    tokenUrl: https://oauth.employmenthero.com/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/employment-hero/refs/heads/main/scopes/employment-hero-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- HR
- HRIS
- Payroll
- Recruitment
- Employee Benefits
- Workforce Management
- HR Tech
token_urls:
- https://oauth.employmenthero.com/oauth2/token
---
