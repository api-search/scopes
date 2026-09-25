---
api_specs:
- filename: piknik-spot-openapi.yml
  format: yaml
  label: Piknik.Spot REST API
  slug: piknikspot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/openapi/piknik-spot-openapi.yml
authorization_urls:
- https://piknik.spot/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Piknik Spot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Piknik.Spot publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Piknik.Spot API on a user''s behalf.


  Tokens are issued from https://piknik.spot/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Piknik.Spot
provider_slug: piknik-spot
schemes:
- description: OAuth 2.0 authentication for external applications and AI agents
  flows:
  - authorizationUrl: https://piknik.spot/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://piknik.spot/api/oauth/token
  name: oauth2
  source: openapi/piknik-spot-openapi.yml
scope_count: 4
scope_names:
- events:write
- marketplace:write
- read:profile
- write:profile
scopes:
- description: Create and manage community events
  flows:
  - authorizationCode
  scope: events:write
- description: Create and manage marketplace listings
  flows:
  - authorizationCode
  scope: marketplace:write
- description: Read user profile information
  flows:
  - authorizationCode
  scope: read:profile
- description: Update user profile information
  flows:
  - authorizationCode
  scope: write:profile
slug: piknik-spot-scopes
source_filename: piknik-spot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: derived\nsource: openapi/piknik-spot-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/piknik-spot-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://piknik.spot/api/oauth/authorize\n    tokenUrl: https://piknik.spot/api/oauth/token\n  description: OAuth 2.0 authentication for external applications and AI agents\nscopes:\n- scope: events:write\n  description: Create and manage community events\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/piknik-spot-openapi.yml\n- scope: marketplace:write\n  description: Create and manage marketplace listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/piknik-spot-openapi.yml\n- scope: read:profile\n  description: Read user profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/piknik-spot-openapi.yml\n- scope: write:profile\n  description: Update user profile information\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/piknik-spot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piknik-spot/refs/heads/main/scopes/piknik-spot-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Local Food
- Agriculture
- Farmers Markets
- Marketplace
- Event
- Job
- Recipes
- Geolocation
- Community
- Food Systems
- MCP
- A2A
- Agent-Native
- Ontario
- Canada
token_urls:
- https://piknik.spot/api/oauth/token
---
