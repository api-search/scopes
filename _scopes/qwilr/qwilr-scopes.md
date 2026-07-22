---
authorization_urls:
- https://api.qwilr.com/oauth/authorize
description: ''
docs: https://mcp.qwilr.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Qwilr Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Qwilr publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Qwilr API on a user''s behalf.


  Tokens are issued from https://api.qwilr.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qwilr
provider_slug: qwilr
schemes:
- flows:
  - authorizationUrl: https://api.qwilr.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.qwilr.com/oauth/token
  name: mcpOAuth2
  source: api.qwilr.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth client access to the Qwilr hosted MCP server at https://mcp.qwilr.com. This is the only scope advertised by Qwilr's OAuth 2.0 authorization server metadata (scopes_supported).
  flows:
  - authorizationCode
  scope: mcp
slug: qwilr-scopes
source_filename: qwilr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.qwilr.com/.well-known/oauth-authorization-server\ndocs: https://mcp.qwilr.com/.well-known/oauth-protected-resource\nschemes:\n- name: mcpOAuth2\n  source: api.qwilr.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.qwilr.com/oauth/authorize\n    tokenUrl: https://api.qwilr.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Grants an OAuth client access to the Qwilr hosted MCP server at\n    https://mcp.qwilr.com. This is the only scope advertised by Qwilr's\n    OAuth 2.0 authorization server metadata (scopes_supported).\n  flows:\n  - authorizationCode\n  sources:\n  - api.qwilr.com/.well-known/oauth-authorization-server\nnotes: >-\n  The REST API (api.qwilr.com/v1) uses opaque bearer JWT tokens generated in-app,\n  not OAuth scopes. The only documented OAuth scope surface is the single \"mcp\"\n  scope fronting the MCP server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qwilr/refs/heads/main/scopes/qwilr-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Proposals
- Documents
- Sales
- Quotes
- Contracts
- E-Signature
- Webhooks
- MCP
- SaaS
token_urls:
- https://api.qwilr.com/oauth/token
---
