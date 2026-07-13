---
api_specs:
- filename: uclapi.json
  format: json
  label: UCL API Room Bookings
  slug: roombookings
  spec_type: OpenAPI
  url: https://github.com/uclapi/uclapi-openapi/blob/master/uclapi.json
authorization_urls:
- /authorise
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Ucl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'UCL publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the UCL API on a user''s behalf.


  Tokens are issued from /token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: UCL
provider_slug: ucl
schemes:
- description: This API uses OAuth2 with the implicit grant flow. [More info](https://uclapi.com/docs#OAuthSecurity)
  flows:
  - authorizationUrl: /authorise
    flow: authorizationCode
    tokenUrl: /token
  name: OAuthSecurity
  source: openapi/ucl-uclapi.yaml
scope_count: 2
scope_names:
- personal_timetable
- student_number
scopes:
- description: read user's timetable
  flows:
  - authorizationCode
  scope: personal_timetable
- description: read user's student number
  flows:
  - authorizationCode
  scope: student_number
slug: ucl-scopes
source_filename: ucl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ucl-uclapi.yaml\nschemes:\n- name: OAuthSecurity\n  source: openapi/ucl-uclapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /authorise\n    tokenUrl: /token\n  description: This API uses OAuth2 with the implicit grant flow. [More info](https://uclapi.com/docs#OAuthSecurity)\nscopes:\n- scope: personal_timetable\n  description: read user's timetable\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ucl-uclapi.yaml\n- scope: student_number\n  description: read user's student number\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/ucl-uclapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucl/refs/heads/main/scopes/ucl-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Education
- Higher Education
- University
- United Kingdom
- Open Data
- Research
- Library
- Timetable
token_urls:
- /token
---
