---
api_specs:
- filename: cogny-openapi.yml
  format: yaml
  label: Cogny API
  slug: cogny-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/openapi/cogny-openapi.yml
authorization_urls:
- https://cogny.com/api/mcp/oauth/authorize
description: ''
docs: https://cogny.com/docs/api-overview-authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cogny Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cogny publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cogny API on a user''s behalf.


  Tokens are issued from https://cogny.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cogny
provider_slug: cogny
schemes:
- description: OAuth 2.1 (DCR + PKCE) for MCP clients.
  flows:
  - authorizationUrl: https://cogny.com/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://cogny.com/api/mcp/oauth/token
  name: oauth2
  source: well-known/cogny-oauth-authorization-server.json
scope_count: 8
scope_names:
- read
- write
- tickets:read
- tickets:write
- reports:read
- reports:write
- warehouses:read
- warehouses:write
scopes:
- description: Read access
  flows: []
  scope: read
- description: Write access
  flows: []
  scope: write
- description: Read tickets
  flows: []
  scope: tickets:read
- description: Write tickets
  flows: []
  scope: tickets:write
- description: Read growth reports
  flows: []
  scope: reports:read
- description: Create/cancel growth reports
  flows: []
  scope: reports:write
- description: Read connected warehouses
  flows: []
  scope: warehouses:read
- description: Manage connected warehouses
  flows: []
  scope: warehouses:write
slug: cogny-scopes
source_filename: cogny-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cogny-openapi.yml\ndocs: https://cogny.com/docs/api-overview-authentication\nschemes:\n  - name: oauth2\n    source: well-known/cogny-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://cogny.com/api/mcp/oauth/authorize\n        tokenUrl: https://cogny.com/api/mcp/oauth/token\n    description: OAuth 2.1 (DCR + PKCE) for MCP clients.\nscopes:\n  # From the OAuth authorization-server metadata (MCP surface)\n  - {scope: read, description: Read access, source: well-known}\n  - {scope: write, description: Write access, source: well-known}\n  - {scope: 'tickets:read', description: Read tickets, source: well-known}\n  - {scope: 'tickets:write', description: Write tickets, source: well-known}\n  # From the REST API key-scope reference (docs)\n  - {scope: 'reports:read', description: Read growth reports, source: docs}\n  - {scope: 'reports:write', description: Create/cancel\
  \ growth reports, source: docs}\n  - {scope: 'warehouses:read', description: Read connected warehouses, source: docs}\n  - {scope: 'warehouses:write', description: Manage connected warehouses, source: docs}\nnotes: >-\n  Two scope surfaces: the OAuth MCP flow advertises read/write/tickets:*; the REST\n  API-key generator (Settings > API Keys) offers reports:*, tickets:read, warehouses:*.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogny/refs/heads/main/scopes/cogny-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Company
- Ai Enterprise Software
- Marketing
- Marketing Analytics
- Marketing Automation
- MCP
- Agents
- Data Warehouse
- Advertising
token_urls:
- https://cogny.com/api/mcp/oauth/token
---
