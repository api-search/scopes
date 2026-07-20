---
authorization_urls:
- https://app.archive.com/oauth/authorize
description: Archive's direct GraphQL API authenticates with a workspace-scoped bearer token, not OAuth, so it exposes no scope surface. OAuth is used only by Archive's hosted MCP server, whose RFC 8414 authorization-server metadata declares a single supported scope, "mcp".
docs: https://api-docs.archive.com
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Archive Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Archive Technologies publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Archive Technologies API on a user''s behalf.


  Tokens are issued from https://app.archive.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Archive Technologies
provider_slug: archive-technologies
schemes:
- flows:
  - authorizationUrl: https://app.archive.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.archive.com/oauth/token
  name: mcpOAuth
  source: https://app.archive.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth client access to the Archive MCP server (app.archive.com/api/v2/mcp), which fronts the Archive GraphQL API on the authorized user's behalf.
  flows:
  - authorizationCode
  scope: mcp
slug: archive-technologies-scopes
source_filename: archive-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.archive.com/.well-known/oauth-authorization-server\ndocs: https://api-docs.archive.com\ndescription: >-\n  Archive's direct GraphQL API authenticates with a workspace-scoped bearer token, not\n  OAuth, so it exposes no scope surface. OAuth is used only by Archive's hosted MCP server,\n  whose RFC 8414 authorization-server metadata declares a single supported scope, \"mcp\".\nschemes:\n- name: mcpOAuth\n  type: oauth2\n  source: https://app.archive.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.archive.com/oauth/authorize\n    tokenUrl: https://app.archive.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Grants an OAuth client access to the Archive MCP server (app.archive.com/api/v2/mcp),\n    which fronts the Archive GraphQL API on the authorized user's behalf.\n  flows: [authorizationCode]\n  sources: [https://app.archive.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archive-technologies/refs/heads/main/scopes/archive-technologies-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Creator Marketing
- Influencer Marketing
- Social Listening
- User Generated Content
- E-commerce
- GraphQL
- MCP
token_urls:
- https://app.archive.com/oauth/token
---
