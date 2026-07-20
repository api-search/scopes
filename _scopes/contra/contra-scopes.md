---
api_specs:
- filename: contra-openapi-original.json
  format: json
  label: Contra Public API
  slug: contra-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contra/refs/heads/main/openapi/contra-openapi-original.json
authorization_urls:
- https://contra.com/api/mcp/oauth/authorize
description: ''
docs: https://contra.com/.well-known/oauth-protected-resource/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Contra Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Contra publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Contra API on a user''s behalf.


  Tokens are issued from https://contra.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Contra
provider_slug: contra
schemes:
- flows:
  - authorizationUrl: https://contra.com/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://contra.com/api/mcp/oauth/token
  name: McpOAuth2
  source: well-known/contra-openid-configuration.json
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Grants an authorized client access to invoke the tools exposed by the Contra MCP server (https://contra.com/mcp).
  flows:
  - authorizationCode
  scope: mcp:tools
slug: contra-scopes
source_filename: contra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://contra.com/.well-known/openid-configuration\ndocs: https://contra.com/.well-known/oauth-protected-resource/mcp\nschemes:\n- name: McpOAuth2\n  source: well-known/contra-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://contra.com/api/mcp/oauth/authorize\n    tokenUrl: https://contra.com/api/mcp/oauth/token\nscopes:\n- scope: mcp:tools\n  description: >-\n    Grants an authorized client access to invoke the tools exposed by the\n    Contra MCP server (https://contra.com/mcp).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/contra-openid-configuration.json\nnotes: >-\n  The Contra Public REST API uses a static X-API-Key header (no OAuth\n  scopes). OAuth scopes here apply only to the hosted MCP server, which\n  advertises a single scope, mcp:tools.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contra/refs/heads/main/scopes/contra-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Future Of Work
- Freelance Marketplace
- Talent
- Hiring
- Professional Network
- Model Context Protocol
- Developer API
token_urls:
- https://contra.com/api/mcp/oauth/token
---
