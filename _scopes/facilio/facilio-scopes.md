---
api_specs:
- filename: facilio-openapi-original.yaml
  format: yaml
  label: Facilio REST API v5
  slug: facilio-rest-api-v5
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/openapi/facilio-openapi-original.yaml
authorization_urls:
- https://us.facilioapis.com/identity/oauth2/authorize
- https://mcp.facilio.com/authorize
description: ''
docs: https://mcp.facilio.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: searched
name: Facilio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Facilio publishes 7 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Facilio API on a user''s behalf.


  Tokens are issued from https://us.facilioapis.com/identity/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Facilio
provider_slug: facilio
schemes:
- flows:
  - authorizationUrl: https://us.facilioapis.com/identity/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://us.facilioapis.com/identity/oauth2/token
  - flow: password
    tokenUrl: https://us.facilioapis.com/identity/oauth2/token
  name: oauth2
  source: openapi/facilio-openapi-original.yaml
- flows:
  - authorizationUrl: https://mcp.facilio.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.facilio.com/token
  name: mcp-oauth2
  source: https://mcp.facilio.com/.well-known/oauth-authorization-server
scope_count: 7
scope_names:
- openid
- email
- profile
- connections:actions.execute.read
- connections:actions.execute.write
- connections:actions.execute.destructive
- api
scopes:
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Access the authenticated user's email
  flows:
  - authorizationCode
  scope: email
- description: Access the authenticated user's basic profile
  flows:
  - authorizationCode
  scope: profile
- description: Execute read-only actions/queries through Facilio connections
  flows:
  - authorizationCode
  scope: connections:actions.execute.read
- description: Execute write actions (create/update) through Facilio connections
  flows:
  - authorizationCode
  scope: connections:actions.execute.write
- description: Execute destructive actions (delete); the MCP server requires explicit user confirmation before performing these
  flows:
  - authorizationCode
  scope: connections:actions.execute.destructive
- description: Coarse-grained API access scope advertised by the MCP server card
  flows:
  - authorizationCode
  scope: api
slug: facilio-scopes
source_filename: facilio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/facilio-openapi-original.yaml\ndocs: https://mcp.facilio.com/.well-known/oauth-authorization-server\nnotes: >-\n  The Facilio REST API OpenAPI declares an oauth2 scheme with empty scope maps\n  (coarse-grained bearer access). The granular published scope surface lives on\n  Facilio's hosted MCP OAuth 2.0 Authorization Server (https://mcp.facilio.com),\n  captured verbatim below from its RFC 8414 authorization-server metadata\n  (well-known/facilio-mcp-oauth-authorization-server.json).\nschemes:\n- name: oauth2\n  source: openapi/facilio-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.facilioapis.com/identity/oauth2/authorize\n    tokenUrl: https://us.facilioapis.com/identity/oauth2/token\n  - flow: password\n    tokenUrl: https://us.facilioapis.com/identity/oauth2/token\n- name: mcp-oauth2\n  source: https://mcp.facilio.com/.well-known/oauth-authorization-server\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://mcp.facilio.com/authorize\n    tokenUrl: https://mcp.facilio.com/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: email\n  description: Access the authenticated user's email\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Access the authenticated user's basic profile\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: connections:actions.execute.read\n  description: Execute read-only actions/queries through Facilio connections\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: connections:actions.execute.write\n  description: Execute write actions (create/update)\
  \ through Facilio connections\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: connections:actions.execute.destructive\n  description: >-\n    Execute destructive actions (delete); the MCP server requires explicit user\n    confirmation before performing these\n  flows: [authorizationCode]\n  sources: [https://mcp.facilio.com/.well-known/oauth-authorization-server]\n- scope: api\n  description: Coarse-grained API access scope advertised by the MCP server card\n  flows: [authorizationCode]\n  sources: [https://facilio.com/.well-known/mcp/server-card.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facilio/refs/heads/main/scopes/facilio-scopes.yml
summary_line: 7 scopes · authorizationCode/password
tags:
- Company
- Ai
- Facility Management
- CMMS
- Property Operations
- Maintenance
- Asset Management
- Real Estate
- IoT
- Buildings
token_urls:
- https://us.facilioapis.com/identity/oauth2/token
- https://mcp.facilio.com/token
---
