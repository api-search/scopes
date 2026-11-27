---
api_specs:
- filename: odooconsole-com-discovery-api-openapi.yml
  format: yaml
  label: OConsole Discovery API
  slug: odooconsole-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-discovery-api-openapi.yml
- filename: odooconsole-com-mcp-api-openapi.yml
  format: yaml
  label: OConsole MCP API
  slug: odooconsole-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/odooconsole-com/openapi/odooconsole-com-mcp-api-openapi.yml
authorization_urls:
- https://auth.odooconsole.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: OConsole Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OConsole publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the OConsole API on a user''s behalf.


  Tokens are issued from https://auth.odooconsole.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OConsole
provider_slug: odooconsole-com
schemes:
- description: Authorization code with PKCE. Clients register themselves at `https://auth.odooconsole.com/oauth2/register` (RFC 7591) — there is no client id to copy out of a dashboard.
  flows:
  - authorizationUrl: https://auth.odooconsole.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://auth.odooconsole.com/oauth2/token
  name: odooconsole
  source: openapi/odooconsole-com-openapi.json
scope_count: 4
scope_names:
- instances:read
- instances:write
- odoo:read
- odoo:write
scopes:
- description: List instances on the account and read their status and logs
  flows:
  - authorizationCode
  scope: instances:read
- description: Create, restart and delete instances
  flows:
  - authorizationCode
  scope: instances:write
- description: Read records, models and views in the instance this connector is authorised for
  flows:
  - authorizationCode
  scope: odoo:read
- description: Create, update and delete records in that instance
  flows:
  - authorizationCode
  scope: odoo:write
slug: odooconsole-com-scopes
source_filename: odooconsole-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/odooconsole-com-openapi.json\nschemes:\n- name: odooconsole\n  source: openapi/odooconsole-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.odooconsole.com/oauth2/auth\n    tokenUrl: https://auth.odooconsole.com/oauth2/token\n  description: Authorization code with PKCE. Clients register themselves at `https://auth.odooconsole.com/oauth2/register`\n    (RFC 7591) — there is no client id to copy out of a dashboard.\nscopes:\n- scope: instances:read\n  description: List instances on the account and read their status and logs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/odooconsole-com-openapi.json\n- scope: instances:write\n  description: Create, restart and delete instances\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/odooconsole-com-openapi.json\n- scope: odoo:read\n  description: Read records, models and views in the instance this connector is authorised\
  \ for\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/odooconsole-com-openapi.json\n- scope: odoo:write\n  description: Create, update and delete records in that instance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/odooconsole-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/odooconsole-com/scopes/odooconsole-com-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- ERP
- Hosting
- Odoo
token_bound: false
token_urls:
- https://auth.odooconsole.com/oauth2/token
---
