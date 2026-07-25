---
api_specs:
- filename: paedae-applications-api-openapi.yml
  format: yaml
  label: Paedae Applications API
  slug: paedae-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-applications-api-openapi.yml
- filename: paedae-beacon-configurations-api-openapi.yml
  format: yaml
  label: Paedae Beacon Configurations API
  slug: paedae-beacon-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacon-configurations-api-openapi.yml
- filename: paedae-beacons-api-openapi.yml
  format: yaml
  label: Paedae Beacons API
  slug: paedae-beacons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-beacons-api-openapi.yml
- filename: paedae-communications-api-openapi.yml
  format: yaml
  label: Paedae Communications API
  slug: paedae-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-communications-api-openapi.yml
- filename: paedae-places-api-openapi.yml
  format: yaml
  label: Paedae Places API
  slug: paedae-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/openapi/paedae-places-api-openapi.yml
authorization_urls:
- https://manager.gimbal.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Paedae Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paedae uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://manager.gimbal.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paedae
provider_slug: paedae
schemes:
- description: Some Proximity APIs require an OAuth 2.0 access token instead of the organization server API key.
  flows:
  - authorizationUrl: https://manager.gimbal.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://manager.gimbal.com/oauth/token
  name: ProximityOAuth2
  source: openapi/paedae-rest-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paedae-scopes
source_filename: paedae-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/paedae-rest-openapi.yml\nschemes:\n- name: ProximityOAuth2\n  source: openapi/paedae-rest-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://manager.gimbal.com/oauth/authorize\n    tokenUrl: https://manager.gimbal.com/oauth/token\n  description: Some Proximity APIs require an OAuth 2.0 access token instead of the organization\n    server API key.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paedae/refs/heads/main/scopes/paedae-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Proximity
- Location
- Beacons
- Geofencing
- Mobile SDK
- Advertising
- Marketing
token_urls:
- https://manager.gimbal.com/oauth/token
---
