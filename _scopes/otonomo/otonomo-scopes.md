---
api_specs:
- filename: otonomo-fleet-openapi.yml
  format: yaml
  label: Otonomo Fleet API
  slug: otonomo-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/openapi/otonomo-fleet-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Otonomo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Otonomo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.otonomo.io/v1/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Otonomo
provider_slug: otonomo
schemes:
- description: 'OAuth2 client-credentials. Obtain a Bearer token from POST /v1/oauth/token/ then send it as Authorization: Bearer <token>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.otonomo.io/v1/oauth/token/
  name: oauth2
  source: openapi/otonomo-fleet-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: otonomo-scopes
source_filename: otonomo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/otonomo-fleet-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/otonomo-fleet-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.otonomo.io/v1/oauth/token/\n  description: 'OAuth2 client-credentials. Obtain a Bearer token from POST /v1/oauth/token/\n    then send it as Authorization: Bearer <token>.'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otonomo/refs/heads/main/scopes/otonomo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Connected Vehicles
- Automotive
- Fleet Management
- Telematics
- Vehicle Data
- Mobility
- IoT
- Location
- Connected Car
token_urls:
- https://api.otonomo.io/v1/oauth/token/
---
