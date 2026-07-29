---
api_specs:
- filename: alectra-utilities-green-button-espi-openapi.json
  format: json
  label: Alectra Utilities Green Button Connect My Data (CMD) API
  slug: alectra-green-button-connect-my-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-green-button-espi-openapi.json
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
name: Alectra Utilities Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alectra Utilities uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://sandbox.greenbuttonalliance.org:8443/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alectra Utilities
provider_slug: alectra-utilities
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  source: openapi/alectra-utilities-green-button-espi-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: alectra-utilities-scopes
source_filename: alectra-utilities-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/alectra-utilities-green-button-espi-openapi.json\ndocs: null\nprovenance_warning: >-\n  Derived from the Green Button Alliance OpenAPI harvested into openapi/, not from an\n  Alectra scopes reference. Alectra Utilities publishes no scope list, no OAuth\n  metadata and no consent-permission reference anywhere on alectrautilities.com or on\n  its Savage Data-hosted Green Button portal.\nschemes:\n- name: oauth2\n  source: openapi/alectra-utilities-green-button-espi-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\nscopes: []\nscope_count: 0\nfinding: >-\n  The oauth2 security scheme is declared and applied to every operation, but both\n  flows carry an EMPTY scopes\
  \ map in the source specification, and no operation\n  attaches a named scope in its security[] requirement. NAESB REQ.21 ESPI does define\n  a structured scope string for Connect My Data authorisations (function block,\n  interval duration and history parameters encoded into a single scope value), but\n  neither the harvested specification nor any Alectra surface enumerates one, so no\n  scope strings are recorded here. Nothing is invented.\nconsent_model: >-\n  Green Button Connect My Data authorisation is per customer and per data selection:\n  the customer chooses the data and the time period in Alectra's Green Button portal,\n  and the resulting Authorization resource carries the negotiated scope, grant_type,\n  token_type and expires_at. The scope value is therefore issued at consent time by\n  the data custodian rather than published in advance as a fixed catalogue.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/scopes/alectra-utilities-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Ontario
- Green Button
- Smart Metering
- Energy Data
- Grid
- Municipal Utility
- ESPI
token_urls:
- https://sandbox.greenbuttonalliance.org:8443/oauth/token
---
