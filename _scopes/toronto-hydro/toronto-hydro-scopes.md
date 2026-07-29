---
api_specs:
- filename: toronto-hydro-green-button-espi-openapi.yml
  format: yaml
  label: Toronto Hydro Green Button Connect My Data
  slug: toronto-hydro-green-button-connect-my-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/openapi/toronto-hydro-green-button-espi-openapi.yml
authorization_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Toronto Hydro Scopes
name_suffix: OAuth Scopes
note: Zero scopes is the real, expected result. The oauth2 scheme in the Green Button Alliance source specification declares an EMPTY scopes object, and Toronto Hydro publishes no scopes or permissions reference page anywhere — no scope names were invented. The authorization and token URLs below are the GBA sandbox's, not Toronto Hydro's; Toronto Hydro publishes no OAuth endpoints. In the Green Button model the effective grant is expressed through the customer's authorization at consent time and carried on the Authorization resource (fields scope, grant_type, expires_at, status) rather than through a published scope catalogue. Toronto Hydro describes the data classes covered — consumption details, billing information and customer information — but does not express them as scopes.
overview: 'Toronto Hydro uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Toronto Hydro
provider_slug: toronto-hydro
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/toronto-hydro-green-button-espi-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: toronto-hydro-scopes
source_filename: toronto-hydro-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/toronto-hydro-green-button-espi-openapi.yml\nnote: >-\n  Zero scopes is the real, expected result. The oauth2 scheme in the Green Button Alliance\n  source specification declares an EMPTY scopes object, and Toronto Hydro publishes no\n  scopes or permissions reference page anywhere — no scope names were invented. The\n  authorization and token URLs below are the GBA sandbox's, not Toronto Hydro's; Toronto\n  Hydro publishes no OAuth endpoints. In the Green Button model the effective grant is\n  expressed through the customer's authorization at consent time and carried on the\n  Authorization resource (fields scope, grant_type, expires_at, status) rather than\n  through a published scope catalogue. Toronto Hydro describes the data classes covered —\n  consumption details, billing information and customer information — but does not\n  express them as scopes.\nschemes:\n- name: oauth2\n  source: openapi/toronto-hydro-green-button-espi-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toronto-hydro/refs/heads/main/scopes/toronto-hydro-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Smart Metering
- Green Button
- Grid
- Ontario
- Consumer Data
- Electricity Distribution
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
