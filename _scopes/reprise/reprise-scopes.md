---
authorization_urls:
- https://app.getreprise.com/r/mcp/oauth/authorize
description: ''
docs: https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Reprise Scopes
name_suffix: OAuth Scopes
note: 'Reprise publishes no OpenAPI and its RFC 8414 authorization-server metadata does not advertise a scopes_supported array, so there is no machine-readable scope registry to derive from. The one scope Reprise documents by name is read_only. Effective authorization is not scope-carried: every MCP token inherits the authorizing user''s existing Reprise RBAC role, and the MCP boundary can only narrow that, never widen it.'
overview: 'Reprise publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Reprise API on a user''s behalf.


  Tokens are issued from https://app.getreprise.com/r/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Reprise
provider_slug: reprise
schemes:
- flows:
  - authorizationUrl: https://app.getreprise.com/r/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.getreprise.com/r/mcp/oauth/token
  issuer: https://app.getreprise.com
  name: MCPOAuth2
  scopes_supported_advertised: false
  source: well-known/reprise-oauth-authorization-server.json
scope_count: 1
scope_names:
- read_only
scopes:
- description: Requested at token issue time (scope=read_only) to give an AI assistant read access to Reprise content while blocking every write. Writes are rejected at the MCP boundary rather than in the backend.
  flows:
  - authorizationCode
  scope: read_only
slug: reprise-scopes
source_filename: reprise-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\ndocs: https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\nnote: >\n  Reprise publishes no OpenAPI and its RFC 8414 authorization-server metadata does not advertise\n  a scopes_supported array, so there is no machine-readable scope registry to derive from. The\n  one scope Reprise documents by name is read_only. Effective authorization is not\n  scope-carried: every MCP token inherits the authorizing user's existing Reprise RBAC role, and\n  the MCP boundary can only narrow that, never widen it.\n\nschemes:\n  - name: MCPOAuth2\n    source: well-known/reprise-oauth-authorization-server.json\n    issuer: https://app.getreprise.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.getreprise.com/r/mcp/oauth/authorize\n        tokenUrl: https://app.getreprise.com/r/mcp/oauth/token\n\
  \    scopes_supported_advertised: false\n\nscopes:\n  - scope: read_only\n    description: >\n      Requested at token issue time (scope=read_only) to give an AI assistant read access to\n      Reprise content while blocking every write. Writes are rejected at the MCP boundary rather\n      than in the backend.\n    flows: [authorizationCode]\n    sources:\n      - https://reprise.zendesk.com/hc/en-us/articles/50081170817691-The-Reprise-MCP-Meet-your-AI-Demo-Engineer\n\nimplicit_scoping:\n  - mechanism: endpoint selection\n    description: >\n      Product-scoped MCP endpoints act as a coarse capability scope. /v2/mcp/tour/ exposes only\n      tour_* tools, /v2/mcp/injection/ only injection_*, /v2/mcp/clone/ only clone_*, while\n      /mcp/ exposes the full catalog. Reprise recommends the scoped endpoints for AI clients\n      that silently drop tools past a cap.\n  - mechanism: RBAC inheritance\n    description: >\n      The token carries the user's Reprise role. Custom roles, builder\
  \ vs presenter licensing,\n      group sharing and folder-level permissions all apply unchanged to MCP calls.\n  - mechanism: tenant isolation\n    description: >\n      Enforced in three layers per Reprise — an MCP scope check, request-context client binding,\n      and an ORM client= filter on every backend query.\n\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://app.getreprise.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reprise/refs/heads/main/scopes/reprise-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Demo Automation
- Product Tours
- Sales Demos
- Interactive Demos
- Sandbox Environments
- Enterprise Sales
- Marketing Technology
- Sales Enablement
- Model Context Protocol
- Agent Tooling
- Demo Analytics
token_urls:
- https://app.getreprise.com/r/mcp/oauth/token
---
