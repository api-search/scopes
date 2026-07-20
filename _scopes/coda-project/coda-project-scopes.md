---
api_specs:
- filename: coda-project-openapi-original.json
  format: json
  label: Coda Docs API
  slug: coda-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/openapi/coda-project-openapi-original.json
- filename: coda-project-admin-openapi-original.json
  format: json
  label: Coda Admin API
  slug: coda-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/openapi/coda-project-admin-openapi-original.json
authorization_urls:
- https://coda.io/v4/api/oauth2/authorize
description: ''
docs: https://coda.io/developers/apis/v1
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coda Project Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coda Project publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coda Project API on a user''s behalf.


  Tokens are issued from https://coda.io/v4/api/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coda Project
provider_slug: coda-project
schemes:
- flows:
  - authorizationUrl: https://coda.io/v4/api/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://coda.io/v4/api/oauth2/register
    tokenUrl: https://coda.io/v4/api/oauth2/token
  name: OAuth2
  source: well-known/coda-project-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:all
scopes:
- description: Full access to Coda resources via the remote MCP server (read and write).
  flows:
  - authorizationCode
  scope: mcp:all
slug: coda-project-scopes
source_filename: coda-project-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://coda.io/.well-known/oauth-authorization-server\ndocs: https://coda.io/developers/apis/v1\nnotes: >-\n  Coda's Docs API and Admin API authenticate with Bearer API tokens (no OAuth scopes on those\n  schemes). Coda separately runs an OAuth 2.0 authorization server (RFC 8414 metadata below)\n  that powers third-party apps and the official remote MCP server, with PKCE (S256) and\n  dynamic client registration. Its advertised scope surface is a single coarse scope. Per-token\n  authorization on the Docs API is instead expressed as read/write access restrictions scoped\n  to documents or tables (see authentication/coda-project-authentication.yml).\nschemes:\n- name: OAuth2\n  source: well-known/coda-project-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://coda.io/v4/api/oauth2/authorize\n    tokenUrl: https://coda.io/v4/api/oauth2/token\n    registrationUrl: https://coda.io/v4/api/oauth2/register\n\
  \    pkce: S256\nscopes:\n- scope: \"mcp:all\"\n  description: Full access to Coda resources via the remote MCP server (read and write).\n  flows: [authorizationCode]\n  sources: [well-known/coda-project-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda-project/refs/heads/main/scopes/coda-project-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Productivity
- Documents
- Spreadsheets
- Collaboration
- No-Code
- Workspace
- AI
- Content Management
- SaaS
token_urls:
- https://coda.io/v4/api/oauth2/token
---
