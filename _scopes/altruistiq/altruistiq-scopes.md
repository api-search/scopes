---
api_specs:
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq Datasource API
  slug: altruistiq-datasource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
- filename: altruistiq-openapi.yml
  format: yaml
  label: Altruistiq PACT API
  slug: altruistiq-pact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altruistiq/refs/heads/main/openapi/altruistiq-openapi.yml
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
