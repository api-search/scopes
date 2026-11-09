---
api_specs:
- filename: google-maps-autocomplete-api-openapi.yml
  format: yaml
  label: Google Maps Platform Autocomplete API
  slug: google-maps-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-autocomplete-api-openapi.yml
- filename: google-maps-directions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-openapi.yml
- filename: google-maps-geocoding-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-openapi.yml
- filename: google-maps-nearby-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Nearby Search API
  slug: google-maps-nearby-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-nearby-search-api-openapi.yml
- filename: google-maps-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Photos API
  slug: google-maps-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-photos-api-openapi.yml
- filename: google-maps-place-details-api-openapi.yml
  format: yaml
  label: Google Maps Platform Place Details API
  slug: google-maps-place-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-place-details-api-openapi.yml
- filename: google-maps-text-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Text Search API
  slug: google-maps-text-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-text-search-api-openapi.yml
- filename: google-maps-directions-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-api-openapi.yml
- filename: google-maps-distance-matrix-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Distance Matrix API
  slug: google-maps-distance-matrix-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-distance-matrix-api-api-openapi.yml
- filename: google-maps-elevation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Elevation API
  slug: google-maps-elevation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-elevation-api-api-openapi.yml
- filename: google-maps-geocoding-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-api-openapi.yml
- filename: google-maps-geolocation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geolocation API
  slug: google-maps-geolocation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geolocation-api-api-openapi.yml
- filename: google-maps-places-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Places API
  slug: google-maps-places-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-places-api-api-openapi.yml
- filename: google-maps-roads-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Roads API
  slug: google-maps-roads-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-roads-api-api-openapi.yml
- filename: google-maps-street-view-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View API
  slug: google-maps-street-view-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-api-api-openapi.yml
- filename: google-maps-time-zone-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Time Zone API
  slug: google-maps-time-zone-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-time-zone-api-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developers.google.com/maps/documentation/places/web-service/get-api-key
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Google Maps Scopes
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
