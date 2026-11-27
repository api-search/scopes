---
api_specs:
- filename: google-maps-pollen-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Maps Pollen Forecast API
  slug: google-maps-pollen-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-forecast-api-openapi.yml
- filename: google-maps-address-validation-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Address Validation V1 API
  slug: google-maps-address-validation-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-address-validation-v1-api-openapi.yml
- filename: google-maps-air-quality-currentconditions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality CurrentConditions API
  slug: google-maps-air-quality-currentconditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-currentconditions-api-openapi.yml
- filename: google-maps-air-quality-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality Forecast API
  slug: google-maps-air-quality-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-forecast-api-openapi.yml
- filename: google-maps-air-quality-history-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality History API
  slug: google-maps-air-quality-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-history-api-openapi.yml
- filename: google-maps-air-quality-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality MapTypes API
  slug: google-maps-air-quality-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-maptypes-api-openapi.yml
- filename: google-maps-area-insights-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Area Insights V1 API
  slug: google-maps-area-insights-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-area-insights-v1-api-openapi.yml
- filename: google-maps-pollen-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Pollen MapTypes API
  slug: google-maps-pollen-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-maptypes-api-openapi.yml
- filename: google-maps-solar-buildinginsights-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar BuildingInsights API
  slug: google-maps-solar-buildinginsights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-buildinginsights-api-openapi.yml
- filename: google-maps-solar-datalayers-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar DataLayers API
  slug: google-maps-solar-datalayers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-datalayers-api-openapi.yml
- filename: google-maps-solar-geotiff-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar GeoTiff API
  slug: google-maps-solar-geotiff-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-geotiff-api-openapi.yml
- filename: google-maps-street-view-publish-photo-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photo API
  slug: google-maps-street-view-publish-photo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photo-api-openapi.yml
- filename: google-maps-street-view-publish-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photos API
  slug: google-maps-street-view-publish-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photos-api-openapi.yml
- filename: google-maps-street-view-publish-photosequence-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequence API
  slug: google-maps-street-view-publish-photosequence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequence-api-openapi.yml
- filename: google-maps-street-view-publish-photosequences-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequences API
  slug: google-maps-street-view-publish-photosequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequences-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/maps/documentation/places/web-service/get-api-key
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Maps Platform Scopes
name_suffix: OAuth Scopes
note: The OpenAPI contracts in this repo declare only apiKey security. The docs state that Places API (New) also accepts OAuth 2.0 tokens and name a single required scope. The dedicated oauth-token page returned HTTP 404 to a direct fetch from here on 2026-11-05.
overview: 'Google Maps Platform publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Maps Platform API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Maps Platform
provider_slug: google-maps
schemes: []
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/cloud-platform
scopes:
- description: Required scope on OAuth 2.0 access tokens used with Places API (New).
  flows: []
  scope: https://www.googleapis.com/auth/cloud-platform
slug: google-maps-scopes
source_filename: google-maps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Google Maps Platform OAuth scopes\ngenerated: '2026-11-05'\nmethod: searched\nsource: https://developers.google.com/maps/documentation/places/web-service/get-api-key\ndocs: https://developers.google.com/maps/documentation/places/web-service/get-api-key\nnote: The OpenAPI contracts in this repo declare only apiKey security. The docs state that Places API (New)\n  also accepts OAuth 2.0 tokens and name a single required scope. The dedicated oauth-token page returned\n  HTTP 404 to a direct fetch from here on 2026-11-05.\nquote: 'To use OAuth with Places API (New), you must assign the OAuth token the following scope: https://www.googleapis.com/auth/cloud-platform'\nscopes:\n- name: https://www.googleapis.com/auth/cloud-platform\n  description: Required scope on OAuth 2.0 access tokens used with Places API (New).\n  applies_to: Places API (New) (places.googleapis.com)\n"
source_yaml_url: https://artifacts.apis.io/google-maps/scopes/google-maps-scopes.yml
summary_line: 1 scope
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
- Geospatial
token_bound: false
token_urls: []
---
