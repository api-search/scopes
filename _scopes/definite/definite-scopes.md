---
authorization_urls:
- https://api.definite.app/oauth/authorize
description: ''
docs: https://www.definite.app/docs/mcp/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Definite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Definite publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Definite API on a user''s behalf.


  Tokens are issued from https://api.definite.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Definite
provider_slug: definite
schemes:
- flows:
  - authorizationUrl: https://api.definite.app/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.definite.app/oauth/token
  name: oauth2Mcp
  source: /.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth-authorized MCP client access to the Definite Model Context Protocol server tools (query, semantic layer, integrations, syncs, docs, drive). The only scope advertised in the authorization-server metadata.
  flows:
  - authorizationCode
  scope: mcp
slug: definite-scopes
source_filename: definite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.definite.app/.well-known/oauth-authorization-server\ndocs: https://www.definite.app/docs/mcp/mcp\nschemes:\n- name: oauth2Mcp\n  source: /.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.definite.app/oauth/authorize\n    tokenUrl: https://api.definite.app/oauth/token\n    pkce: S256\nscopes:\n- scope: mcp\n  description: >-\n    Grants an OAuth-authorized MCP client access to the Definite Model Context\n    Protocol server tools (query, semantic layer, integrations, syncs, docs,\n    drive). The only scope advertised in the authorization-server metadata.\n  flows: [authorizationCode]\n  sources: [/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definite/refs/heads/main/scopes/definite-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Data
- Analytics
- Business Intelligence
- Data Integration
- Data Warehouse
- Lakehouse
- Semantic Layer
- Artificial Intelligence
- AI Agents
- Model Context Protocol
- ETL
token_urls:
- https://api.definite.app/oauth/token
---
