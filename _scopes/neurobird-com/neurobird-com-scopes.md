---
api_specs:
- filename: neurobird-com-admin-api-openapi.yml
  format: yaml
  label: Neurobird Admin API
  slug: neurobird-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-admin-api-openapi.yml
- filename: neurobird-com-analyze-api-openapi.yml
  format: yaml
  label: Neurobird Analyze API
  slug: neurobird-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-analyze-api-openapi.yml
- filename: neurobird-com-aurora-api-openapi.yml
  format: yaml
  label: Neurobird Aurora API
  slug: neurobird-com-aurora-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-aurora-api-openapi.yml
- filename: neurobird-com-auth-api-openapi.yml
  format: yaml
  label: Neurobird Auth API
  slug: neurobird-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-auth-api-openapi.yml
- filename: neurobird-com-billing-api-openapi.yml
  format: yaml
  label: Neurobird Billing API
  slug: neurobird-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-billing-api-openapi.yml
- filename: neurobird-com-contact-api-openapi.yml
  format: yaml
  label: Neurobird Contact API
  slug: neurobird-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-contact-api-openapi.yml
- filename: neurobird-com-dashboard-api-openapi.yml
  format: yaml
  label: Neurobird Dashboard API
  slug: neurobird-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-dashboard-api-openapi.yml
- filename: neurobird-com-dashboard-html-api-openapi.yml
  format: yaml
  label: Neurobird Dashboard.html API
  slug: neurobird-com-dashboard-html-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-dashboard-html-api-openapi.yml
- filename: neurobird-com-download-api-openapi.yml
  format: yaml
  label: Neurobird Download API
  slug: neurobird-com-download-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-download-api-openapi.yml
- filename: neurobird-com-files-preview-api-openapi.yml
  format: yaml
  label: Neurobird Files Preview API
  slug: neurobird-com-files-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-files-preview-api-openapi.yml
- filename: neurobird-com-generate-files-api-openapi.yml
  format: yaml
  label: Neurobird Generate Files API
  slug: neurobird-com-generate-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-generate-files-api-openapi.yml
- filename: neurobird-com-guest-usage-api-openapi.yml
  format: yaml
  label: Neurobird Guest Usage API
  slug: neurobird-com-guest-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-guest-usage-api-openapi.yml
- filename: neurobird-com-result-api-openapi.yml
  format: yaml
  label: Neurobird Result API
  slug: neurobird-com-result-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-result-api-openapi.yml
- filename: neurobird-com-screenshot-api-openapi.yml
  format: yaml
  label: Neurobird Screenshot API
  slug: neurobird-com-screenshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-screenshot-api-openapi.yml
- filename: neurobird-com-stats-api-openapi.yml
  format: yaml
  label: Neurobird Stats API
  slug: neurobird-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-stats-api-openapi.yml
- filename: neurobird-com-status-api-openapi.yml
  format: yaml
  label: Neurobird Status API
  slug: neurobird-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurobird-com/openapi/neurobird-com-status-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Neurobird Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Neurobird uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/auth/jwt/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Neurobird
provider_slug: neurobird-com
schemes:
- flows:
  - flow: password
    tokenUrl: /api/auth/jwt/login
  name: OAuth2PasswordBearer
  source: openapi/geo-neurobird-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: neurobird-com-scopes
source_filename: neurobird-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: none\nsource: openapi/geo-neurobird-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/geo-neurobird-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /api/auth/jwt/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/neurobird-com/scopes/neurobird-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Agency
- Product Studio
- Machine Learning
- Automation
- Consulting
token_bound: false
token_urls:
- /api/auth/jwt/login
---
