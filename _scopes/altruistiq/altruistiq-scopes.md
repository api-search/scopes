---
api_specs:
- filename: altruistiq-datasource-api-openapi.yml
  format: yaml
  label: Altruistiq Datasource API
  slug: altruistiq-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-datasource-api-openapi.yml
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
authorization_urls: []
description: ''
docs: https://docs.altruistiq.com
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Altruistiq Scopes
name_suffix: OAuth Scopes
note: Altruistiq authenticates via the OAuth 2.0 client credentials flow (RFC 6749) against /api/public/v1/oauth2/token using only client_id and client_secret, and no OAuth scopes are documented or used (https://docs.altruistiq.com).
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
  source: openapi/altruistiq-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: altruistiq-scopes
source_filename: altruistiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/altruistiq-openapi.yml\ndocs: https://docs.altruistiq.com\nnote: >-\n  Altruistiq authenticates via the OAuth 2.0 client credentials flow (RFC 6749) against\n  /api/public/v1/oauth2/token using only client_id and client_secret, and no OAuth scopes\n  are documented or used (https://docs.altruistiq.com).\nschemes:\n- name: oauth2\n  source: openapi/altruistiq-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.altruistiq.com/api/public/v1/oauth2/token\nscopes: []\n"
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
- FMCG
- Food and Beverage
- ESG
- CSRD
- SBTi
- PACT
- Sustainability Intelligence
token_urls:
- https://app.altruistiq.com/api/public/v1/oauth2/token
---
