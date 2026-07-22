---
authorization_urls:
- https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/auth
description: ''
docs: https://mcp.cumbuca.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cumbuca Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cumbuca publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cumbuca API on a user''s behalf.


  Tokens are issued from https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cumbuca
provider_slug: cumbuca
schemes:
- flows:
  - authorizationUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token
  name: cumbuca-mcp
  source: https://idc.cumbuca.com/realms/cumbuca-mcp
scope_count: 4
scope_names:
- openid
- profile
- offline_access
- open-finance
scopes:
- description: OIDC authentication of the end user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  scope: profile
- description: Refresh-token issuance for long-lived MCP sessions.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access to the user's Open Finance data (bank statements, credit-card transactions) surfaced through the Cumbuca Open Finance Data MCP server.
  flows:
  - authorizationCode
  scope: open-finance
slug: cumbuca-scopes
source_filename: cumbuca-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://mcp.cumbuca.com/.well-known/oauth-protected-resource\ndocs: https://mcp.cumbuca.com/.well-known/oauth-protected-resource\nschemes:\n  - name: cumbuca-mcp\n    source: https://idc.cumbuca.com/realms/cumbuca-mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/auth\n        tokenUrl: https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token\nscopes:\n  - scope: openid\n    description: OIDC authentication of the end user.\n    flows: [authorizationCode]\n    sources: [https://mcp.cumbuca.com/.well-known/oauth-protected-resource]\n  - scope: profile\n    description: Basic profile claims for the authenticated user.\n    flows: [authorizationCode]\n    sources: [https://mcp.cumbuca.com/.well-known/oauth-protected-resource]\n  - scope: offline_access\n    description: Refresh-token issuance for long-lived MCP sessions.\n\
  \    flows: [authorizationCode]\n    sources: [https://mcp.cumbuca.com/.well-known/oauth-protected-resource]\n  - scope: open-finance\n    description: >\n      Access to the user's Open Finance data (bank statements, credit-card\n      transactions) surfaced through the Cumbuca Open Finance Data MCP server.\n    flows: [authorizationCode]\n    sources: [https://mcp.cumbuca.com/.well-known/oauth-protected-resource]\nnotes: >\n  Scopes read verbatim from the MCP server's RFC 9728 protected-resource\n  metadata (scopes_supported). Tokens are mTLS certificate-bound.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cumbuca/refs/heads/main/scopes/cumbuca-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Fintech
- Open Finance
- Pix
- Payments
- Banking
- Brazil
- Open Banking
- Financial Data
- MCP
token_urls:
- https://idc.cumbuca.com/realms/cumbuca-mcp/protocol/openid-connect/token
---
