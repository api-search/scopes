---
api_specs:
- filename: openstreetmap-capabilities-api-openapi.yml
  format: yaml
  label: OpenStreetMap Capabilities API
  slug: openstreetmap-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-capabilities-api-openapi.yml
- filename: openstreetmap-changesets-api-openapi.yml
  format: yaml
  label: OpenStreetMap Changesets API
  slug: openstreetmap-changesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-changesets-api-openapi.yml
- filename: openstreetmap-map-data-api-openapi.yml
  format: yaml
  label: OpenStreetMap Map Data API
  slug: openstreetmap-map-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-map-data-api-openapi.yml
- filename: openstreetmap-nodes-api-openapi.yml
  format: yaml
  label: OpenStreetMap Nodes API
  slug: openstreetmap-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-nodes-api-openapi.yml
- filename: openstreetmap-notes-api-openapi.yml
  format: yaml
  label: OpenStreetMap Notes API
  slug: openstreetmap-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-notes-api-openapi.yml
- filename: openstreetmap-relations-api-openapi.yml
  format: yaml
  label: OpenStreetMap Relations API
  slug: openstreetmap-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-relations-api-openapi.yml
- filename: openstreetmap-users-api-openapi.yml
  format: yaml
  label: OpenStreetMap Users API
  slug: openstreetmap-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-users-api-openapi.yml
- filename: openstreetmap-ways-api-openapi.yml
  format: yaml
  label: OpenStreetMap Ways API
  slug: openstreetmap-ways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-ways-api-openapi.yml
- filename: openstreetmap-geocoding-api-openapi.yml
  format: yaml
  label: OpenStreetMap Geocoding API
  slug: openstreetmap-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-geocoding-api-openapi.yml
- filename: openstreetmap-status-api-openapi.yml
  format: yaml
  label: OpenStreetMap Status API
  slug: openstreetmap-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-status-api-openapi.yml
authorization_urls:
- https://www.openstreetmap.org/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Openstreetmap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OpenStreetMap publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OpenStreetMap API on a user''s behalf.


  Tokens are issued from https://www.openstreetmap.org/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OpenStreetMap
provider_slug: openstreetmap
schemes:
- description: OAuth 2.0 — required for write operations
  flows:
  - authorizationUrl: https://www.openstreetmap.org/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://www.openstreetmap.org/oauth2/token
  name: OAuth2
  source: openapi/openstreetmap-main-openapi.yml
scope_count: 7
scope_names:
- read_gpx
- read_prefs
- write_api
- write_diary
- write_gpx
- write_notes
- write_prefs
scopes:
- description: Read private GPS traces
  flows:
  - authorizationCode
  scope: read_gpx
- description: Read user preferences
  flows:
  - authorizationCode
  scope: read_prefs
- description: Modify the map (nodes, ways, relations, changesets)
  flows:
  - authorizationCode
  scope: write_api
- description: Create diary entries
  flows:
  - authorizationCode
  scope: write_diary
- description: Upload GPS traces
  flows:
  - authorizationCode
  scope: write_gpx
- description: Create, comment on, and close notes
  flows:
  - authorizationCode
  scope: write_notes
- description: Modify user preferences
  flows:
  - authorizationCode
  scope: write_prefs
slug: openstreetmap-scopes
source_filename: openstreetmap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openstreetmap-main-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/openstreetmap-main-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.openstreetmap.org/oauth2/authorize\n    tokenUrl: https://www.openstreetmap.org/oauth2/token\n  description: OAuth 2.0 — required for write operations\nscopes:\n- scope: read_gpx\n  description: Read private GPS traces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n- scope: read_prefs\n  description: Read user preferences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n- scope: write_api\n  description: Modify the map (nodes, ways, relations, changesets)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n- scope: write_diary\n  description: Create diary entries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n\
  - scope: write_gpx\n  description: Upload GPS traces\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n- scope: write_notes\n  description: Create, comment on, and close notes\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n- scope: write_prefs\n  description: Modify user preferences\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openstreetmap-main-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/scopes/openstreetmap-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Geospatial
- Mapping
- Open Data
- Geocoding
- Editing
token_urls:
- https://www.openstreetmap.org/oauth2/token
---
