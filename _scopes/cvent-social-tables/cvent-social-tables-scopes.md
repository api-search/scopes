---
api_specs:
- filename: cvent-social-tables-openapi.json
  format: json
  label: Social Tables Events API (Legacy)
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/openapi/cvent-social-tables-openapi.json
authorization_urls:
- https://auth.socialtables.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cvent Social Tables Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cvent Social Tables publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cvent Social Tables API on a user''s behalf.


  Tokens are issued from https://auth.socialtables.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cvent Social Tables
provider_slug: cvent-social-tables
schemes:
- description: OAuth
  flows:
  - authorizationUrl: https://auth.socialtables.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.socialtables.com/oauth/token
  name: oauth2
  source: openapi/cvent-social-tables-openapi.json
scope_count: 3
scope_names:
- authenticated
- create:oauth_client
- userdata
scopes:
- description: any authentication whatsoever
  flows:
  - authorizationCode
  scope: authenticated
- description: oauth client create
  flows:
  - authorizationCode
  scope: create:oauth_client
- description: All of the things.
  flows:
  - authorizationCode
  scope: userdata
slug: cvent-social-tables-scopes
source_filename: cvent-social-tables-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-social-tables-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/cvent-social-tables-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.socialtables.com/oauth/authorize\n    tokenUrl: https://auth.socialtables.com/oauth/token\n  description: OAuth\nscopes:\n- scope: authenticated\n  description: any authentication whatsoever\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n- scope: create:oauth_client\n  description: oauth client create\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n- scope: userdata\n  description: All of the things.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cvent-social-tables-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-social-tables/refs/heads/main/scopes/cvent-social-tables-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- 3D Design
- Catering
- Diagramming
- Event Design
- Event Management
- Events
- Floor Plans
- Hospitality
- Hotel
- Meetings
- Seating
- Seating Charts
- Venues
token_urls:
- https://auth.socialtables.com/oauth/token
---
