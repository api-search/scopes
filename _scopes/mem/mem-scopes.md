---
api_specs:
- filename: mem-openapi-original.json
  format: json
  label: Mem Public Client API
  slug: mem-public-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/openapi/mem-openapi-original.json
authorization_urls:
- https://mem.ai/oauth/consent
description: ''
docs: https://docs.mem.ai/mcp/setup
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Mem Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mem publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mem API on a user''s behalf.


  Tokens are issued from https://api.mem.ai/api/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mem
provider_slug: mem
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mem.ai/oauth/consent
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.mem.ai/api/v2/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://api.mem.ai/api/v2/oauth2/token
  issuer: https://api.mem.ai
  name: OAuth2
  registration_endpoint: https://api.mem.ai/oauth2/register
  source: https://api.mem.ai/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- content.read
- content.write
- profile.read
- profile.write
scopes:
- description: Read access to the user's Mem notes and collections.
  flows:
  - authorizationCode
  - clientCredentials
  scope: content.read
- description: Create, update, and organize the user's Mem notes and collections.
  flows:
  - authorizationCode
  - clientCredentials
  scope: content.write
- description: Read access to the user's Mem profile.
  flows:
  - authorizationCode
  scope: profile.read
- description: Write access to the user's Mem profile.
  flows:
  - authorizationCode
  scope: profile.write
slug: mem-scopes
source_filename: mem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.mem.ai/.well-known/oauth-authorization-server\ndocs: https://docs.mem.ai/mcp/setup\nschemes:\n  - name: OAuth2\n    source: https://api.mem.ai/.well-known/oauth-authorization-server\n    issuer: https://api.mem.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mem.ai/oauth/consent\n        tokenUrl: https://api.mem.ai/api/v2/oauth2/token\n        pkce: S256\n      - flow: clientCredentials\n        tokenUrl: https://api.mem.ai/api/v2/oauth2/token\n    registration_endpoint: https://api.mem.ai/oauth2/register\n    dynamic_client_registration: true\nscopes:\n  - scope: content.read\n    description: Read access to the user's Mem notes and collections.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/mem-oauth-authorization-server.json, well-known/mem-oauth-protected-resource.json]\n  - scope: content.write\n    description: Create, update, and organize the\
  \ user's Mem notes and collections.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/mem-oauth-authorization-server.json, well-known/mem-oauth-protected-resource.json]\n  - scope: profile.read\n    description: Read access to the user's Mem profile.\n    flows: [authorizationCode]\n    sources: [well-known/mem-openid-configuration.json]\n  - scope: profile.write\n    description: Write access to the user's Mem profile.\n    flows: [authorizationCode]\n    sources: [well-known/mem-openid-configuration.json]\nnotes: >-\n  Scopes are advertised via OAuth 2.0 Authorization Server Metadata (RFC 8414)\n  and OIDC discovery on api.mem.ai. The hosted MCP server (mcp.mem.ai) scopes\n  its protected resource to content.read + content.write. The REST API's own\n  OpenAPI securitySchemes declare bearer-token (API key) auth; OAuth 2.0 is the\n  mechanism used for the MCP server and third-party app connectors.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mem/refs/heads/main/scopes/mem-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Notes
- Knowledge Management
- Productivity
- Artificial Intelligence
- Note Taking
- Search
- MCP
- Agents
- Meetings
token_urls:
- https://api.mem.ai/api/v2/oauth2/token
---
