---
api_specs:
- filename: university-of-sheffield-admin-api-openapi.yml
  format: yaml
  label: University of Sheffield Admin API
  slug: university-of-sheffield-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-admin-api-openapi.yml
- filename: university-of-sheffield-api-auth-api-openapi.yml
  format: yaml
  label: University of Sheffield API Auth API
  slug: university-of-sheffield-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-api-auth-api-openapi.yml
- filename: university-of-sheffield-auth-api-openapi.yml
  format: yaml
  label: University of Sheffield Auth API
  slug: university-of-sheffield-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-auth-api-openapi.yml
- filename: university-of-sheffield-health-api-openapi.yml
  format: yaml
  label: University of Sheffield Health API
  slug: university-of-sheffield-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-health-api-openapi.yml
- filename: university-of-sheffield-metrics-api-openapi.yml
  format: yaml
  label: University of Sheffield Metrics API
  slug: university-of-sheffield-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-metrics-api-openapi.yml
- filename: university-of-sheffield-pvforecast-api-openapi.yml
  format: yaml
  label: University of Sheffield Pvforecast API
  slug: university-of-sheffield-pvforecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-pvforecast-api-openapi.yml
- filename: university-of-sheffield-pvlive-api-openapi.yml
  format: yaml
  label: University of Sheffield Pvlive API
  slug: university-of-sheffield-pvlive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-pvlive-api-openapi.yml
- filename: university-of-sheffield-pvlive-eu-api-openapi.yml
  format: yaml
  label: University of Sheffield Pvlive Eu API
  slug: university-of-sheffield-pvlive-eu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-pvlive-eu-api-openapi.yml
- filename: university-of-sheffield-user-api-openapi.yml
  format: yaml
  label: University of Sheffield User API
  slug: university-of-sheffield-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-user-api-openapi.yml
- filename: university-of-sheffield-users-api-openapi.yml
  format: yaml
  label: University of Sheffield Users API
  slug: university-of-sheffield-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: University Of Sheffield Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'University of Sheffield uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /auth/jwt/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Sheffield
provider_slug: university-of-sheffield
schemes:
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-admin-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-api-auth-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-auth-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-health-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-metrics-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-pvforecast-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-pvlive-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-pvlive-eu-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-user-api-openapi.yml
- flows:
  - flow: password
    tokenUrl: /auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/university-of-sheffield-users-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: university-of-sheffield-scopes
source_filename: university-of-sheffield-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/university-of-sheffield-admin-api-openapi.yml, openapi/university-of-sheffield-api-auth-api-openapi.yml,\n  openapi/university-of-sheffield-auth-api-openapi.yml, openapi/university-of-sheffield-health-api-openapi.yml,\n  openapi/university-of-sheffield-metrics-api-openapi.yml, openapi/university-of-sheffield-pvforecast-api-openapi.yml,\n  openapi/university-of-sheffield-pvlive-api-openapi.yml, openapi/university-of-sheffield-pvlive-eu-api-openapi.yml,\n  openapi/university-of-sheffield-user-api-openapi.yml, openapi/university-of-sheffield-users-api-openapi.yml\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-admin-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-api-auth-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source:\
  \ openapi/university-of-sheffield-auth-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-health-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-metrics-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-pvforecast-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-pvlive-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-pvlive-eu-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-user-api-openapi.yml\n\
  \  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\n- name: OAuth2PasswordBearer\n  source: openapi/university-of-sheffield-users-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /auth/jwt/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/scopes/university-of-sheffield-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Access
- OAI-PMH
- Identity Federation
- Solar Energy
- Energy Data
- Research Computing
token_bound: false
token_urls:
- /auth/jwt/login
---
