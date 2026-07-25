---
api_specs:
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-airport-info-api-openapi.yml
  format: yaml
  label: VATSIM Airport info API
  slug: vatsim-airport-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-airport-info-api-openapi.yml
- filename: vatsim-atc-api-openapi.yml
  format: yaml
  label: VATSIM atc API
  slug: vatsim-atc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-atc-api-openapi.yml
- filename: vatsim-audio-api-openapi.yml
  format: yaml
  label: VATSIM Audio API
  slug: vatsim-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-audio-api-openapi.yml
- filename: vatsim-community-api-openapi.yml
  format: yaml
  label: VATSIM community API
  slug: vatsim-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-community-api-openapi.yml
- filename: vatsim-data-feed-api-openapi.yml
  format: yaml
  label: VATSIM Data feed API
  slug: vatsim-data-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-data-feed-api-openapi.yml
- filename: vatsim-event-info-api-openapi.yml
  format: yaml
  label: VATSIM Event info API
  slug: vatsim-event-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-event-info-api-openapi.yml
- filename: vatsim-events-api-openapi.yml
  format: yaml
  label: VATSIM Events API
  slug: vatsim-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-events-api-openapi.yml
- filename: vatsim-members-api-openapi.yml
  format: yaml
  label: VATSIM members API
  slug: vatsim-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-members-api-openapi.yml
- filename: vatsim-metar-api-openapi.yml
  format: yaml
  label: VATSIM METAR API
  slug: vatsim-metar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-metar-api-openapi.yml
- filename: vatsim-oauth2-api-openapi.yml
  format: yaml
  label: VATSIM OAuth2 API
  slug: vatsim-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-oauth2-api-openapi.yml
- filename: vatsim-orgs-api-openapi.yml
  format: yaml
  label: VATSIM orgs API
  slug: vatsim-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-orgs-api-openapi.yml
- filename: vatsim-servers-api-openapi.yml
  format: yaml
  label: VATSIM Servers API
  slug: vatsim-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-servers-api-openapi.yml
- filename: vatsim-user-api-openapi.yml
  format: yaml
  label: VATSIM User API
  slug: vatsim-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-user-api-openapi.yml
- filename: vatsim-users-api-openapi.yml
  format: yaml
  label: VATSIM Users API
  slug: vatsim-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/openapi/vatsim-users-api-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Vatsim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VATSIM publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the VATSIM API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VATSIM
provider_slug: vatsim
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: connect
  source: openapi/connect.yaml
scope_count: 4
scope_names:
- country
- email
- full_name
- vatsim_details
scopes:
- description: Read the user's country of residence
  flows:
  - authorizationCode
  scope: country
- description: Read the user's email address
  flows:
  - authorizationCode
  scope: email
- description: Read the user's full name
  flows:
  - authorizationCode
  scope: full_name
- description: Read the user's VATSIM ratings and divisions
  flows:
  - authorizationCode
  scope: vatsim_details
slug: vatsim-scopes
source_filename: vatsim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/connect.yaml\nschemes:\n- name: connect\n  source: openapi/connect.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\nscopes:\n- scope: country\n  description: Read the user's country of residence\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: email\n  description: Read the user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: full_name\n  description: Read the user's full name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: vatsim_details\n  description: Read the user's VATSIM ratings and divisions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/scopes/vatsim-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
token_urls:
- /oauth/token
---
