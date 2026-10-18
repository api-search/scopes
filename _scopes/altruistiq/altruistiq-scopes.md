---
api_specs:
- filename: altruistiq-export-api-openapi.yml
  format: yaml
  label: Altruistiq Export API
  slug: altruistiq-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-export-api-openapi.yml
- filename: altruistiq-facility-api-openapi.yml
  format: yaml
  label: Altruistiq Facility API
  slug: altruistiq-facility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-facility-api-openapi.yml
- filename: altruistiq-location-api-openapi.yml
  format: yaml
  label: Altruistiq Location API
  slug: altruistiq-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-location-api-openapi.yml
- filename: altruistiq-organization-api-openapi.yml
  format: yaml
  label: Altruistiq Organization API
  slug: altruistiq-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-organization-api-openapi.yml
- filename: altruistiq-product-api-openapi.yml
  format: yaml
  label: Altruistiq Product API
  slug: altruistiq-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-product-api-openapi.yml
- filename: altruistiq-product-structure-api-openapi.yml
  format: yaml
  label: Altruistiq Product structure API
  slug: altruistiq-product-structure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-product-structure-api-openapi.yml
- filename: altruistiq-product-structure-inputs-api-openapi.yml
  format: yaml
  label: Altruistiq Product structure inputs API
  slug: altruistiq-product-structure-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-product-structure-inputs-api-openapi.yml
- filename: altruistiq-security-api-openapi.yml
  format: yaml
  label: Altruistiq Security API
  slug: altruistiq-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-security-api-openapi.yml
- filename: altruistiq-data-source-api-openapi.yml
  format: yaml
  label: Altruistiq Data Source API
  slug: altruistiq-data-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-data-source-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Altruistiq Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Altruistiq uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.altruistiq.com/api/public/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Altruistiq
provider_slug: altruistiq
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-data-source-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-export-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-facility-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-location-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-organization-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-product-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-product-structure-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-product-structure-inputs-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token
  name: oauth2
  source: openapi/altruistiq-security-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: altruistiq-scopes
source_filename: altruistiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/altruistiq-data-source-api-openapi.yml, openapi/altruistiq-export-api-openapi.yml,\n  openapi/altruistiq-facility-api-openapi.yml, openapi/altruistiq-location-api-openapi.yml,\n  openapi/altruistiq-organization-api-openapi.yml, openapi/altruistiq-product-api-openapi.yml,\n  openapi/altruistiq-product-structure-api-openapi.yml, openapi/altruistiq-product-structure-inputs-api-openapi.yml,\n  openapi/altruistiq-security-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/altruistiq-data-source-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-export-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-facility-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n\
  - name: oauth2\n  source: openapi/altruistiq-location-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-organization-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-product-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-product-structure-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-product-structure-inputs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\n- name: oauth2\n  source: openapi/altruistiq-security-api-openapi.yml\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/scopes/altruistiq-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sustainability
- Climate
- Carbon Accounting
- Emissions
- Greenhouse Gas
- Scope 3
- Product Carbon Footprint
- Corporate Carbon Footprint
- Supply Chain
- Consumer Packaged Goods
- Food and Beverage
- ESG
- CSRD
- SBTi
- PACT
- Sustainability Intelligence
token_bound: false
token_urls:
- https://app.altruistiq.com/api/public/v1/oauth2/token
---
