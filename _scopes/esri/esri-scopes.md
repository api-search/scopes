---
api_specs:
- filename: esri-auth-api-openapi.yml
  format: yaml
  label: Esri Auth API
  slug: esri-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-auth-api-openapi.yml
- filename: esri-geocoding-api-openapi.yml
  format: yaml
  label: Esri Geocoding API
  slug: esri-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-geocoding-api-openapi.yml
- filename: esri-routing-api-openapi.yml
  format: yaml
  label: Esri Routing API
  slug: esri-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-routing-api-openapi.yml
authorization_urls:
- https://www.arcgis.com/sharing/rest/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Esri Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Esri uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://www.arcgis.com/sharing/rest/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Esri
provider_slug: esri
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: oauth2
  source: openapi/esri-auth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: oauth2
  source: openapi/esri-geocoding-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: oauth2
  source: openapi/esri-routing-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: esri-scopes
source_filename: esri-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/esri-auth-api-openapi.yml, openapi/esri-geocoding-api-openapi.yml, openapi/esri-routing-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/esri-auth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n- name: oauth2\n  source: openapi/esri-geocoding-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n- name: oauth2\n  source: openapi/esri-routing-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/scopes/esri-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Geographic
- Geospatial
- GIS
- Location
- Mapping
- Maps
- Spatial Analysis
token_urls:
- https://www.arcgis.com/sharing/rest/oauth2/token
---
