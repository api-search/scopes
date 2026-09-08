---
api_specs:
- filename: esri-arcgis-geocoding-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Geocoding API
  slug: esri-arcgis-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-geocoding-api-openapi.yml
- filename: esri-arcgis-places-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Places API
  slug: esri-arcgis-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-places-api-openapi.yml
- filename: esri-arcgis-portal-api-openapi.yml
  format: yaml
  label: ESRI ArcGIS Portal API
  slug: esri-arcgis-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/openapi/esri-arcgis-portal-api-openapi.yml
authorization_urls:
- https://www.arcgis.com/sharing/rest/oauth2/authorize
description: ''
docs: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
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
  source: openapi/esri-arcgis-geocoding-api-openapi.yml
- flows:
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: OAuth2
  source: openapi/esri-arcgis-places-api-openapi.yml
- flows:
  - authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token
  name: OAuth2
  source: openapi/esri-arcgis-portal-api-openapi.yml
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
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/, https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/,\n  https://www.arcgis.com/.well-known/oauth-authorization-server; baseline derived from openapi/ securitySchemes\nschemes:\n- name: OAuth2\n  source: openapi/esri-arcgis-geocoding-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n- name: OAuth2\n  source: openapi/esri-arcgis-places-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\n- name: OAuth2\n  source: openapi/esri-arcgis-portal-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.arcgis.com/sharing/rest/oauth2/authorize\n\
  \    tokenUrl: https://www.arcgis.com/sharing/rest/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/esri-arcgis-geocoding-api-openapi.yml\n  - openapi/esri-arcgis-places-api-openapi.yml\n  - openapi/esri-arcgis-portal-api-openapi.yml\n- scope: urn:arcgis:scope:root\n  description: Full access to ArcGIS Online\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/esri-arcgis-geocoding-api-openapi.yml\n  - openapi/esri-arcgis-places-api-openapi.yml\n  - openapi/esri-arcgis-portal-api-openapi.yml\ndocs: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/\nmodel:\n  kind: privileges\n  note: ArcGIS does not use a granular OAuth scope vocabulary. OAuth credentials request coarse scopes (openid,\n    urn:arcgis:scope:root) and the effective permission set is the PRIVILEGE list attached to the credential. Privileges\n    divide into standard scope (usable by public\
  \ apps) and personal scope (requires additional account permission;\n    only for personal/private apps).\n  reference: https://developers.arcgis.com/documentation/security-and-authentication/reference/privileges/\nprivileges_observed:\n- privilege: Portal service > General privileges > Apps and capabilities > Allow beta access\n  required_for: MCP for ArcGIS Location Services (beta)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\n- privilege: Location services > Geocoding > Geocode (stored)\n  required_for: find_address_candidates, reverse_geocode (MCP); findAddressCandidates with forStorage=true (REST)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\n  note: Only available for ArcGIS Location Platform accounts with pay-as-you-go enabled.\n- privilege: Location services > Routing > Simple routing\n  required_for: solve_route (MCP); routing service solve (REST)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\n\
  - privilege: Location services > Elevation > Elevation service\n  required_for: elevation_at_locations (MCP)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\n- privilege: Location services > Static maps > Static maps service\n  required_for: map_with_overlay (MCP)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\n- privilege: Location services > Data Enrichment > GeoEnrichment service\n  required_for: get_topic_fields, describe_location (MCP)\n  source: https://developers.arcgis.com/ai/mcp-arcgis-location-services/get-started/\ngaps:\n- Esri publishes no machine-readable list of privilege identifiers; the privileges reference page renders client-side\n  and gives human labels, so an agent cannot enumerate the permission surface programmatically.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esri-arcgis/refs/heads/main/scopes/esri-arcgis-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- GIS
- Geospatial
- Mapping
- Location
- Spatial Analysis
- Geocoding
- Routing
- Places
- OGC
- GraphQL
- MCP
token_urls:
- https://www.arcgis.com/sharing/rest/oauth2/token
---
