---
api_specs:
- filename: avis-budget-rental-cars-openapi.yml
  format: yaml
  label: Avis Budget Group Rental Cars API
  slug: avis-budget-group-rental-cars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/openapi/avis-budget-rental-cars-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.avis.com/getting-started
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Avis Budget Scopes
name_suffix: OAuth Scopes
note: No scopes exist. The OpenAPI declares an empty `scopes` map on the clientCredentials flow, and the Getting Started page documents the token exchange without any scope parameter; authorization is per approved Client Application, not per scope. The Okta tenant named in the API's WWW-Authenticate realm advertises only Okta's own platform scopes (okta.users.read etc.), which are not ABG API scopes and are not recorded here.
overview: 'Avis Budget Group uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://stage.abgapiservices.com/oauth/token/v2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Avis Budget Group
provider_slug: avis-budget
schemes:
- description: OAuth 2.0 client credentials flow used to authenticate all API requests in this package.
  flows:
  - flow: clientCredentials
    tokenUrl: https://stage.abgapiservices.com/oauth/token/v2
  name: ABG-Access-Token
  source: openapi/avis-budget-rental-cars-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: avis-budget-scopes
source_filename: avis-budget-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: openapi/avis-budget-rental-cars-openapi.yml\ndocs: https://developer.avis.com/getting-started\nschemes:\n- name: ABG-Access-Token\n  source: openapi/avis-budget-rental-cars-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://stage.abgapiservices.com/oauth/token/v2\n  description: OAuth 2.0 client credentials flow used to authenticate all API requests in this package.\nscopes: []\nscope_count: 0\nnote: >-\n  No scopes exist. The OpenAPI declares an empty `scopes` map on the clientCredentials flow, and the\n  Getting Started page documents the token exchange without any scope parameter; authorization is\n  per approved Client Application, not per scope. The Okta tenant named in the API's WWW-Authenticate\n  realm advertises only Okta's own platform scopes (okta.users.read etc.), which are not ABG API\n  scopes and are not recorded here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avis-budget/refs/heads/main/scopes/avis-budget-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 500
- Car Rental
- Travel
- Mobility
- Fleet Management
- Transportation
- Reservations
- Vehicle Rental
- Partner API
- Hospitality
token_urls:
- https://stage.abgapiservices.com/oauth/token/v2
---
