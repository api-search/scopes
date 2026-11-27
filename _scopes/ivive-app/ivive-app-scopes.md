---
api_specs:
- filename: ivive-app-auth-api-openapi.yml
  format: yaml
  label: ivive.app Auth API
  slug: ivive-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-auth-api-openapi.yml
- filename: ivive-app-correction-equations-api-openapi.yml
  format: yaml
  label: ivive.app Correction Equations API
  slug: ivive-app-correction-equations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-correction-equations-api-openapi.yml
- filename: ivive-app-health-api-openapi.yml
  format: yaml
  label: ivive.app Health API
  slug: ivive-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-health-api-openapi.yml
- filename: ivive-app-ivivc-api-openapi.yml
  format: yaml
  label: ivive.app Ivivc API
  slug: ivive-app-ivivc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-ivivc-api-openapi.yml
- filename: ivive-app-ivive-api-openapi.yml
  format: yaml
  label: ivive.app Ivive API
  slug: ivive-app-ivive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-ivive-api-openapi.yml
- filename: ivive-app-library-api-openapi.yml
  format: yaml
  label: ivive.app Library API
  slug: ivive-app-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-library-api-openapi.yml
- filename: ivive-app-molecule-api-openapi.yml
  format: yaml
  label: ivive.app Molecule API
  slug: ivive-app-molecule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-molecule-api-openapi.yml
- filename: ivive-app-pk-api-openapi.yml
  format: yaml
  label: ivive.app Pk API
  slug: ivive-app-pk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-pk-api-openapi.yml
- filename: ivive-app-prediction-api-openapi.yml
  format: yaml
  label: ivive.app Prediction API
  slug: ivive-app-prediction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-prediction-api-openapi.yml
- filename: ivive-app-reference-compounds-api-openapi.yml
  format: yaml
  label: ivive.app Reference Compounds API
  slug: ivive-app-reference-compounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-reference-compounds-api-openapi.yml
- filename: ivive-app-scaling-api-openapi.yml
  format: yaml
  label: ivive.app Scaling API
  slug: ivive-app-scaling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-scaling-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: ivive.app Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'ivive.app uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/auth/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ivive.app
provider_slug: ivive-app
schemes:
- flows:
  - flow: password
    tokenUrl: /api/auth/login
  name: OAuth2PasswordBearer
  source: openapi/ivive-app-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: ivive-app-scopes
source_filename: ivive-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: none\nsource: openapi/ivive-app-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/ivive-app-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /api/auth/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/ivive-app/scopes/ivive-app-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- IVIVE
- Drug Discovery
- HepaticClearance
- Open Source
token_bound: false
token_urls:
- /api/auth/login
---
