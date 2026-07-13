---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Google Places API
  slug: google-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/openapi/openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Places Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Places publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Places API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Places
provider_slug: google-places
schemes:
- description: OAuth 2.0 bearer token authorization for the Google Maps Platform.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  source: openapi/openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/maps-platform.places
scopes:
- description: Access the Places API
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/maps-platform.places
slug: google-places-scopes
source_filename: google-places-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n  description: OAuth 2.0 bearer token authorization for the Google Maps Platform.\nscopes:\n- scope: https://www.googleapis.com/auth/maps-platform.places\n  description: Access the Places API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-places/refs/heads/main/scopes/google-places-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Restaurant
- Geolocation
- Google
- Locations
- Maps
- Places
- Points of Interest
token_urls:
- https://oauth2.googleapis.com/token
---
