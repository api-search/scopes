---
api_specs:
- filename: hydro-ottawa-green-button-espi-openapi.yml
  format: yaml
  label: Hydro Ottawa Green Button Connect My Data (CMD) API
  slug: hydro-ottawa-green-button-connect-my-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-green-button-espi-openapi.yml
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
name: Hydro Ottawa Scopes
name_suffix: OAuth Scopes
note: Zero scopes is the real, expected result. The oauth2 scheme in the Green Button Alliance source specification declares an EMPTY scopes object, and Hydro Ottawa publishes no scopes or permissions reference page anywhere — no scope names were invented. The authorization and token URLs below are the GBA sandbox's, not Hydro Ottawa's; Hydro Ottawa publishes no OAuth endpoints. In the Green Button model the effective grant is expressed through the customer's selection of data types, duration and frequency at authorization time, and is carried on the Authorization resource (fields scope, grant_type, expires_at, status) rather than through a published scope catalogue.
overview: 'Hydro Ottawa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hydro Ottawa
provider_slug: hydro-ottawa
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/hydro-ottawa-green-button-espi-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: hydro-ottawa-scopes
source_filename: hydro-ottawa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/hydro-ottawa-green-button-espi-openapi.yml\nnote: >-\n  Zero scopes is the real, expected result. The oauth2 scheme in the Green Button Alliance\n  source specification declares an EMPTY scopes object, and Hydro Ottawa publishes no\n  scopes or permissions reference page anywhere — no scope names were invented. The\n  authorization and token URLs below are the GBA sandbox's, not Hydro Ottawa's; Hydro Ottawa\n  publishes no OAuth endpoints. In the Green Button model the effective grant is expressed\n  through the customer's selection of data types, duration and frequency at authorization\n  time, and is carried on the Authorization resource (fields scope, grant_type, expires_at,\n  status) rather than through a published scope catalogue.\nschemes:\n- name: oauth2\n  source: openapi/hydro-ottawa-green-button-espi-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n\
  \    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/scopes/hydro-ottawa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Electricity Distribution
- Smart Metering
- Green Button
- ESPI
- Municipal Utility
- Renewables
- Hydroelectric
- Solar
- Demand Response
- Grid
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
