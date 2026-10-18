---
api_specs:
- filename: paradox-authentication-api-openapi.yml
  format: yaml
  label: Paradox Authentication API
  slug: paradox-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-authentication-api-openapi.yml
- filename: paradox-candidate-attributes-api-openapi.yml
  format: yaml
  label: Paradox Candidate Attributes API
  slug: paradox-candidate-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-candidate-attributes-api-openapi.yml
- filename: paradox-candidates-api-openapi.yml
  format: yaml
  label: Paradox Candidates API
  slug: paradox-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-candidates-api-openapi.yml
- filename: paradox-company-api-openapi.yml
  format: yaml
  label: Paradox Company API
  slug: paradox-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-company-api-openapi.yml
- filename: paradox-location-areas-api-openapi.yml
  format: yaml
  label: Paradox Location Areas API
  slug: paradox-location-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-location-areas-api-openapi.yml
- filename: paradox-location-rooms-api-openapi.yml
  format: yaml
  label: Paradox Location Rooms API
  slug: paradox-location-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-location-rooms-api-openapi.yml
- filename: paradox-locations-api-openapi.yml
  format: yaml
  label: Paradox Locations API
  slug: paradox-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-locations-api-openapi.yml
- filename: paradox-reporting-api-openapi.yml
  format: yaml
  label: Paradox Reporting API
  slug: paradox-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-reporting-api-openapi.yml
- filename: paradox-scheduling-api-openapi.yml
  format: yaml
  label: Paradox Scheduling API
  slug: paradox-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-scheduling-api-openapi.yml
- filename: paradox-user-permissions-api-openapi.yml
  format: yaml
  label: Paradox User Permissions API
  slug: paradox-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-user-permissions-api-openapi.yml
- filename: paradox-users-api-openapi.yml
  format: yaml
  label: Paradox Users API
  slug: paradox-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/openapi/paradox-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Paradox Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Paradox uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paradox
provider_slug: paradox
schemes:
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-authentication-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-candidate-attributes-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-candidates-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-company-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-location-areas-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-location-rooms-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-locations-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-reporting-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-scheduling-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-user-permissions-api-openapi.yml
- description: OAuth 2.0 client credentials authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /auth/token
  name: oauth2
  source: openapi/paradox-users-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paradox-scopes
source_filename: paradox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/paradox-authentication-api-openapi.yml, openapi/paradox-candidate-attributes-api-openapi.yml,\n  openapi/paradox-candidates-api-openapi.yml, openapi/paradox-company-api-openapi.yml, openapi/paradox-location-areas-api-openapi.yml,\n  openapi/paradox-location-rooms-api-openapi.yml, openapi/paradox-locations-api-openapi.yml,\n  openapi/paradox-reporting-api-openapi.yml, openapi/paradox-scheduling-api-openapi.yml, openapi/paradox-user-permissions-api-openapi.yml,\n  openapi/paradox-users-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/paradox-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-candidate-attributes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n\
  \  source: openapi/paradox-candidates-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-company-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-location-areas-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-location-rooms-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-locations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-reporting-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-scheduling-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-user-permissions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\n- name: oauth2\n  source: openapi/paradox-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n  description: OAuth 2.0 client credentials authentication\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/scopes/paradox-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Candidate Screening
- Chatbots
- Conversational AI
- Hiring Automation
- HR Technology
- Interview Scheduling
- Recruiting
- SMS
- Talent Acquisition
token_bound: false
token_urls:
- /auth/token
---
