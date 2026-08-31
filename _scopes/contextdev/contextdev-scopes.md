---
api_specs:
- filename: contextdev-brand-intelligence-api-openapi.yml
  format: yaml
  label: Context.dev Brand Intelligence API
  slug: contextdev-brand-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-brand-intelligence-api-openapi.yml
- filename: contextdev-monitors-api-openapi.yml
  format: yaml
  label: Context.dev Monitors API
  slug: contextdev-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-monitors-api-openapi.yml
- filename: contextdev-parsing-api-openapi.yml
  format: yaml
  label: Context.dev Parsing API
  slug: contextdev-parsing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-parsing-api-openapi.yml
- filename: contextdev-people-api-openapi.yml
  format: yaml
  label: Context.dev People API
  slug: contextdev-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-people-api-openapi.yml
- filename: contextdev-utility-api-openapi.yml
  format: yaml
  label: Context.dev Utility API
  slug: contextdev-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-utility-api-openapi.yml
- filename: contextdev-web-extraction-api-openapi.yml
  format: yaml
  label: Context.dev Web Extraction API
  slug: contextdev-web-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-web-extraction-api-openapi.yml
- filename: contextdev-web-scraping-api-openapi.yml
  format: yaml
  label: Context.dev Web Scraping API
  slug: contextdev-web-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/openapi/contextdev-web-scraping-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.context.dev/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Contextdev Scopes
name_suffix: OAuth Scopes
note: 'Context.dev exposes the SAME two scopes (api.read, api.write) through three different credential paths: a static ctxt_secret_ API key (no scopes attached, full key privilege), the AgentAuth JWT-bearer/claim ceremony on www.context.dev, and OAuth authorization_code + PKCE on mcp.context.dev for the hosted MCP server. The OpenAPI declares only bearerAuth (http bearer); the scope surface lives entirely in the well-known metadata and auth.md, so a consumer reading the spec alone would not know scopes exist. Only two scopes cover a 49-operation API, so the granularity is coarse — an api.write token can delete every monitor and every batch.'
overview: 'Context.dev publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Context.dev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Context.dev
provider_slug: contextdev
schemes:
- authorization_server: https://www.context.dev
  grant_types:
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:workos:agent-auth:grant-type:claim
  name: AgentAuth
  revocation_endpoint: https://www.context.dev/oauth2/revoke
  source: well-known/contextdev-oauth-authorization-server.json
  token_endpoint: https://www.context.dev/oauth2/token
- added: '2026-08-14'
  authorization_endpoint: https://mcp.context.dev/authorize
  authorization_server: https://mcp.context.dev
  bearer_methods:
  - header
  code_challenge_methods:
  - S256
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.context.dev
  name: MCP OAuth (hosted MCP server)
  note: Discovered 2026-08-14. This is the browser sign-in flow an MCP client uses to reach https://mcp.context.dev/mcp — distinct from the AgentAuth JWT-bearer/claim ceremony on www.context.dev, and distinct again from the static ctxt_secret_ API key. Same two scopes across all three.
  protected_resource: https://mcp.context.dev/mcp
  registration_endpoint: https://mcp.context.dev/register
  response_types:
  - code
  source: well-known/contextdev-mcp-oauth-authorization-server.json
  token_endpoint: https://mcp.context.dev/token
  token_endpoint_auth_methods:
  - client_secret_post
  - none
scope_count: 2
scope_names:
- api.read
- api.write
scopes:
- description: Read access to Context.dev API endpoints (brand lookup, web scrape/crawl, search, enrichment, and related read operations).
  flows: []
  scope: api.read
- description: Write access for mutating API operations (e.g. creating/updating/deleting monitors). Agent credentials are issued with both api.read and api.write after the claim ceremony.
  flows: []
  scope: api.write
slug: contextdev-scopes
source_filename: contextdev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://www.context.dev/.well-known/oauth-authorization-server, https://www.context.dev/auth.md,\n  https://mcp.context.dev/.well-known/oauth-authorization-server, https://mcp.context.dev/.well-known/oauth-protected-resource/mcp\ndocs: https://www.context.dev/auth.md\nschemes:\n- name: AgentAuth\n  source: well-known/contextdev-oauth-authorization-server.json\n  authorization_server: https://www.context.dev\n  token_endpoint: https://www.context.dev/oauth2/token\n  revocation_endpoint: https://www.context.dev/oauth2/revoke\n  grant_types:\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:workos:agent-auth:grant-type:claim\n- name: MCP OAuth (hosted MCP server)\n  source: well-known/contextdev-mcp-oauth-authorization-server.json\n  authorization_server: https://mcp.context.dev\n  issuer: https://mcp.context.dev\n  authorization_endpoint: https://mcp.context.dev/authorize\n  token_endpoint: https://mcp.context.dev/token\n\
  \  registration_endpoint: https://mcp.context.dev/register\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - none\n  dynamic_client_registration: true\n  protected_resource: https://mcp.context.dev/mcp\n  bearer_methods:\n  - header\n  added: '2026-08-14'\n  note: Discovered 2026-08-14. This is the browser sign-in flow an MCP client uses to reach https://mcp.context.dev/mcp\n    — distinct from the AgentAuth JWT-bearer/claim ceremony on www.context.dev, and distinct again from\n    the static ctxt_secret_ API key. Same two scopes across all three.\nscopes:\n- scope: api.read\n  description: Read access to Context.dev API endpoints (brand lookup, web scrape/crawl, search, enrichment,\n    and related read operations).\n  sources:\n  - well-known/contextdev-oauth-authorization-server.json\n  - well-known/contextdev-mcp-oauth-authorization-server.json\n \
  \ - well-known/contextdev-mcp-oauth-protected-resource-mcp.json\n  granted_by:\n  - AgentAuth (www.context.dev)\n  - MCP OAuth (mcp.context.dev)\n- scope: api.write\n  description: Write access for mutating API operations (e.g. creating/updating/deleting monitors). Agent\n    credentials are issued with both api.read and api.write after the claim ceremony.\n  sources:\n  - well-known/contextdev-oauth-authorization-server.json\n  - well-known/contextdev-mcp-oauth-authorization-server.json\n  - well-known/contextdev-mcp-oauth-protected-resource-mcp.json\n  granted_by:\n  - AgentAuth (www.context.dev)\n  - MCP OAuth (mcp.context.dev)\nnote: 'Context.dev exposes the SAME two scopes (api.read, api.write) through three different credential\n  paths: a static ctxt_secret_ API key (no scopes attached, full key privilege), the AgentAuth JWT-bearer/claim\n  ceremony on www.context.dev, and OAuth authorization_code + PKCE on mcp.context.dev for the hosted MCP\n  server. The OpenAPI declares only\
  \ bearerAuth (http bearer); the scope surface lives entirely in the\n  well-known metadata and auth.md, so a consumer reading the spec alone would not know scopes exist. Only\n  two scopes cover a 49-operation API, so the granularity is coarse — an api.write token can delete every\n  monitor and every batch.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextdev/refs/heads/main/scopes/contextdev-scopes.yml
summary_line: 2 scopes
tags:
- Web Scraping
- Brand Intelligence
- Data Enrichment
- AI Agents
- Web Data
- Classification
- Website Monitoring
- Company Data
- Developer Tools
token_urls: []
---
