---
api_specs:
- filename: esri-openapi.yml
  format: yaml
  label: Esri ArcGIS Platform API
  slug: esri-arcgis-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri/refs/heads/main/openapi/esri-openapi.yml
authorization_urls:
- https://www.arcgis.com/sharing/rest/oauth2/authorize
description: ''
docs: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Esri Scopes
name_suffix: OAuth Scopes
note: Esri ArcGIS OAuth 2.0 does not use OAuth scopes — the /oauth2/authorize endpoint has no scope parameter, and access is instead governed by privileges assigned to ArcGIS accounts and developer credentials (https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/).
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
  source: openapi/esri-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: esri-scopes
source_filename: esri-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/esri-openapi.yml\ndocs: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/\nnote: >-\n  Esri ArcGIS OAuth 2.0 does not use OAuth scopes — the /oauth2/authorize\n  endpoint has no scope parameter, and access is instead governed by\n  privileges assigned to ArcGIS accounts and developer credentials\n  (https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/).\nschemes:\n- name: oauth2\n  source: openapi/esri-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\nscopes: []\n"
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
