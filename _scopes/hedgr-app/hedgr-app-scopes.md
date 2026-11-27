---
api_specs:
- filename: hedgr-app-health-api-openapi.yml
  format: yaml
  label: HEDGR Health API
  slug: hedgr-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-health-api-openapi.yml
- filename: hedgr-app-mcp-api-openapi.yml
  format: yaml
  label: HEDGR MCP API
  slug: hedgr-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-mcp-api-openapi.yml
- filename: hedgr-app-oauth-discovery-api-openapi.yml
  format: yaml
  label: HEDGR OAuth discovery API
  slug: hedgr-app-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-oauth-discovery-api-openapi.yml
- filename: hedgr-app-partner-api-api-openapi.yml
  format: yaml
  label: HEDGR Partner API
  slug: hedgr-app-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-partner-api-api-openapi.yml
- filename: hedgr-app-rates-api-openapi.yml
  format: yaml
  label: HEDGR Rates API
  slug: hedgr-app-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hedgr-app/openapi/hedgr-app-rates-api-openapi.yml
authorization_urls:
- https://hedgr.app/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: HEDGR Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HEDGR publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HEDGR API on a user''s behalf.


  Tokens are issued from https://hedgr.app/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HEDGR
provider_slug: hedgr-app
schemes:
- description: OAuth 2.1 authorization-code flow with PKCE and dynamic client registration. See /.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://hedgr.app/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://hedgr.app/mcp/oauth/token
  name: mcpOAuth
  source: openapi/hedgr-app-openapi.json
scope_count: 1
scope_names:
- fx:read
scopes:
- description: Read-only access to FX exposure, cash position, hedge portfolio, P&L, policy, and related dashboard data via MCP tools.
  flows:
  - authorizationCode
  scope: fx:read
slug: hedgr-app-scopes
source_filename: hedgr-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hedgr-app-openapi.json\nschemes:\n- name: mcpOAuth\n  source: openapi/hedgr-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hedgr.app/mcp/oauth/authorize\n    tokenUrl: https://hedgr.app/mcp/oauth/token\n  description: OAuth 2.1 authorization-code flow with PKCE and dynamic client registration.\n    See /.well-known/oauth-authorization-server.\nscopes:\n- scope: fx:read\n  description: Read-only access to FX exposure, cash position, hedge portfolio, P&L, policy,\n    and related dashboard data via MCP tools.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hedgr-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hedgr-app/scopes/hedgr-app-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Finance
- Artificial Intelligence
- Foreign Exchange
- Small Business
- Accounting
- Platform
token_bound: false
token_urls:
- https://hedgr.app/mcp/oauth/token
---
