---
api_specs:
- filename: evermuse-ingest-v1-openapi-original.yml
  format: yaml
  label: Evermuse Ingestion API
  slug: evermuse-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/openapi/evermuse-ingest-v1-openapi-original.yml
authorization_urls:
- https://api.evermuse.com/oauth/authorize
description: ''
docs: https://docs.evermuse.com/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Evermuse Scopes
name_suffix: OAuth Scopes
note: OAuth 2.1 scopes gate the hosted Evermuse MCP server (https://api.evermuse.com/api/mcp), not the REST Ingestion API (which uses `x-api-key` keys carrying `api:read`/`api:write` permissions). Scopes are advertised in the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata.
overview: 'Evermuse publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Evermuse API on a user''s behalf.


  Tokens are issued from https://api.evermuse.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evermuse
provider_slug: evermuse
schemes:
- flows:
  - authorizationUrl: https://api.evermuse.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.evermuse.com/oauth/token
  name: EvermuseOAuth
  source: well-known/evermuse-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- mcp:thirdparty
scopes:
- description: Read access via the Evermuse MCP server (query customer evidence, roadmap, insights).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access via the Evermuse MCP server.
  flows:
  - authorizationCode
  scope: mcp:write
- description: Third-party / delegated access via the Evermuse MCP server.
  flows:
  - authorizationCode
  scope: mcp:thirdparty
slug: evermuse-scopes
source_filename: evermuse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/evermuse-oauth-authorization-server.json\ndocs: https://docs.evermuse.com/authentication\nnote: |-\n  OAuth 2.1 scopes gate the hosted Evermuse MCP server (https://api.evermuse.com/api/mcp),\n  not the REST Ingestion API (which uses `x-api-key` keys carrying `api:read`/`api:write`\n  permissions). Scopes are advertised in the RFC 8414 authorization-server metadata and\n  the RFC 9728 protected-resource metadata.\nschemes:\n- name: EvermuseOAuth\n  source: well-known/evermuse-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.evermuse.com/oauth/authorize\n    tokenUrl: https://api.evermuse.com/oauth/token\n    pkce: S256\nscopes:\n- scope: mcp:read\n  description: Read access via the Evermuse MCP server (query customer evidence, roadmap, insights).\n  flows: [authorizationCode]\n  sources: [well-known/evermuse-oauth-authorization-server.json]\n- scope: mcp:write\n\
  \  description: Write access via the Evermuse MCP server.\n  flows: [authorizationCode]\n  sources: [well-known/evermuse-oauth-authorization-server.json]\n- scope: mcp:thirdparty\n  description: Third-party / delegated access via the Evermuse MCP server.\n  flows: [authorizationCode]\n  sources: [well-known/evermuse-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evermuse/refs/heads/main/scopes/evermuse-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Product Management
- Customer Feedback
- Voice of Customer
- Artificial Intelligence
- Data Ingestion
- Product Analytics
- MCP
- Developer Tools
token_urls:
- https://api.evermuse.com/oauth/token
---
