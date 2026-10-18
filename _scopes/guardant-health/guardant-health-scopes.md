---
api_specs:
- filename: guardant-health-orders-api-openapi.yml
  format: yaml
  label: Guardant Health Orders API
  slug: guardant-health-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-orders-api-openapi.yml
- filename: guardant-health-results-api-openapi.yml
  format: yaml
  label: Guardant Health Results API
  slug: guardant-health-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/openapi/guardant-health-results-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Guardant Health Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Guardant Health uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://example.invalid/guardant-health/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Guardant Health
provider_slug: guardant-health
schemes:
- description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding; no public auth flow is documented.
  flows:
  - flow: clientCredentials
    tokenUrl: https://example.invalid/guardant-health/oauth/token
  name: partnerOAuth2
  source: openapi/guardant-health-orders-api-openapi.yml
- description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding; no public auth flow is documented.
  flows:
  - flow: clientCredentials
    tokenUrl: https://example.invalid/guardant-health/oauth/token
  name: partnerOAuth2
  source: openapi/guardant-health-results-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: guardant-health-scopes
source_filename: guardant-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/guardant-health-orders-api-openapi.yml, openapi/guardant-health-results-api-openapi.yml\nschemes:\n- name: partnerOAuth2\n  source: openapi/guardant-health-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.invalid/guardant-health/oauth/token\n  description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding;\n    no public auth flow is documented.\n- name: partnerOAuth2\n  source: openapi/guardant-health-results-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.invalid/guardant-health/oauth/token\n  description: Placeholder. Partner-provisioned authentication is negotiated during EMR onboarding;\n    no public auth flow is documented.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardant-health/refs/heads/main/scopes/guardant-health-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Precision Oncology
- Liquid Biopsy
- Genomics
- EMR Integration
- Diagnostics
token_bound: false
token_urls:
- https://example.invalid/guardant-health/oauth/token
---
