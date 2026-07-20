---
authorization_urls:
- https://www.instrumentl.com/oauth/authorize
description: ''
docs: https://www.instrumentl.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Instrumentl Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Instrumentl publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instrumentl API on a user''s behalf.


  Tokens are issued from https://www.instrumentl.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instrumentl
provider_slug: instrumentl
schemes:
- flows:
  - authorizationUrl: https://www.instrumentl.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://www.instrumentl.com/oauth/token
    tokenUrl: https://www.instrumentl.com/oauth/token
  name: OAuth2
  source: https://www.instrumentl.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access to Instrumentl data via the remote MCP server (mcp.instrumentl.com).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access to Instrumentl data via the remote MCP server (mcp.instrumentl.com).
  flows:
  - authorizationCode
  scope: mcp:write
slug: instrumentl-scopes
source_filename: instrumentl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.instrumentl.com/.well-known/oauth-protected-resource\ndocs: https://www.instrumentl.com/.well-known/oauth-authorization-server\nschemes:\n  - name: OAuth2\n    source: https://www.instrumentl.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.instrumentl.com/oauth/authorize\n        tokenUrl: https://www.instrumentl.com/oauth/token\n        refreshUrl: https://www.instrumentl.com/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp:read\n    description: Read access to Instrumentl data via the remote MCP server (mcp.instrumentl.com).\n    flows: [authorizationCode]\n    sources: [https://mcp.instrumentl.com/.well-known/oauth-protected-resource]\n  - scope: mcp:write\n    description: Write access to Instrumentl data via the remote MCP server (mcp.instrumentl.com).\n    flows: [authorizationCode]\n    sources: [https://mcp.instrumentl.com/.well-known/oauth-protected-resource]\n\
  notes: >-\n  Scopes are the two MCP scopes advertised by the OAuth authorization-server and\n  protected-resource discovery documents. Instrumentl publishes no public REST\n  API/OpenAPI, so these OAuth scopes govern the MCP surface only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instrumentl/refs/heads/main/scopes/instrumentl-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Grants
- Nonprofit
- Fundraising
- Grant Management
- Foundation Data
- Philanthropy
- MCP
token_urls:
- https://www.instrumentl.com/oauth/token
---
