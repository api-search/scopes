---
api_specs:
- filename: digital-turbine-openapi-generated.yml
  format: yaml
  label: Digital Turbine (Fyber) API
  slug: digital-turbine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/digital-turbine/openapi/_ae-authored/digital-turbine-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Digital Turbine Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Digital Turbine (Fyber) uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://console.fyber.com/api/v2/management/auth.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Digital Turbine (Fyber)
provider_slug: digital-turbine
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://console.fyber.com/api/v2/management/auth
  name: DT_Management_API_OAuth2
  source: openapi/digital-turbine-openapi-generated.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://reporting.fyber.com/auth/v1/token
  name: Offerwall_Reporting_API_OAuth2
  source: openapi/digital-turbine-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: digital-turbine-scopes
source_filename: digital-turbine-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: none\nsource: openapi/digital-turbine-openapi-generated.yml\nschemes:\n- name: DT_Management_API_OAuth2\n  source: openapi/digital-turbine-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://console.fyber.com/api/v2/management/auth\n- name: Offerwall_Reporting_API_OAuth2\n  source: openapi/digital-turbine-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://reporting.fyber.com/auth/v1/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/digital-turbine/scopes/digital-turbine-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Mobile
- Advertising
- Monetization
- SDK
token_bound: false
token_urls:
- https://console.fyber.com/api/v2/management/auth
- https://reporting.fyber.com/auth/v1/token
---
