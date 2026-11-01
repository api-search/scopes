---
api_specs:
- filename: myopl-net-mcp-api-openapi.yml
  format: yaml
  label: myopl-net MCP API
  slug: myopl-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myopl-net/openapi/myopl-net-mcp-api-openapi.yml
authorization_urls:
- https://api.myopl.net/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Myopl Net Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'myopl-net publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the myopl-net API on a user''s behalf.


  Tokens are issued from https://api.myopl.net/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: myopl-net
provider_slug: myopl-net
schemes:
- description: Authorization code with PKCE S256; discover current registration and renewal behavior from authorization-server metadata.
  flows:
  - authorizationUrl: https://api.myopl.net/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.myopl.net/oauth/token
  name: myoplOAuth
  source: openapi/myopl-net-openapi.json
scope_count: 4
scope_names:
- myopl:rating:read
- myopl:rsvp:write
- myopl:sessions:read
- myopl:statistics:read
scopes:
- description: Read the consenting player published OPL ratings
  flows:
  - authorizationCode
  scope: myopl:rating:read
- description: Prepare RSVP for explicit confirmation in MYOPL; does not submit attendance
  flows:
  - authorizationCode
  scope: myopl:rsvp:write
- description: Find the consenting player league sessions
  flows:
  - authorizationCode
  scope: myopl:sessions:read
- description: Read own statistics cards without a paid upgrade
  flows:
  - authorizationCode
  scope: myopl:statistics:read
slug: myopl-net-scopes
source_filename: myopl-net-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/myopl-net-openapi.json\nschemes:\n- name: myoplOAuth\n  source: openapi/myopl-net-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.myopl.net/oauth/authorize\n    tokenUrl: https://api.myopl.net/oauth/token\n  description: Authorization code with PKCE S256; discover current registration and renewal\n    behavior from authorization-server metadata.\nscopes:\n- scope: myopl:rating:read\n  description: Read the consenting player published OPL ratings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myopl-net-openapi.json\n- scope: myopl:rsvp:write\n  description: Prepare RSVP for explicit confirmation in MYOPL; does not submit attendance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myopl-net-openapi.json\n- scope: myopl:sessions:read\n  description: Find the consenting player league sessions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myopl-net-openapi.json\n\
  - scope: myopl:statistics:read\n  description: Read own statistics cards without a paid upgrade\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/myopl-net-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/myopl-net/scopes/myopl-net-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Pickleball
- Sports
- Community
- Platform
token_bound: false
token_urls:
- https://api.myopl.net/oauth/token
---
