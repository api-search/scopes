---
authorization_urls:
- https://www.arcgis.com/sharing/rest/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Esri Arcgis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ESRI ArcGIS publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ESRI ArcGIS API on a user''s behalf.


  Tokens are issued from https://www.arcgis.com/sharing/rest/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ESRI ArcGIS
provider_slug: esri-arcgis
schemes:
- flows:
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: OAuth2
  source: openapi/esri-arcgis-platform-openapi.yml
scope_count: 2
scope_names:
- openid
- urn:arcgis:scope:root
scopes:
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
- description: Full access to ArcGIS Online
  flows:
  - authorizationCode
  scope: urn:arcgis:scope:root
slug: esri-arcgis-scopes
source_filename: esri-arcgis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/esri-arcgis-platform-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/esri-arcgis-platform-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/esri-arcgis-platform-openapi.yml\n- scope: urn:arcgis:scope:root\n  description: Full access to ArcGIS Online\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/esri-arcgis-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/scopes/esri-arcgis-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
token_urls:
- https://www.arcgis.com/sharing/rest/oauth2/token
---
