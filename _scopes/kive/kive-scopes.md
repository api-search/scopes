---
authorization_urls:
- https://mcp.kive.ai/oauth/authorize
description: ''
docs: https://kive.ai/docs/mcp/overview.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Kive Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kive publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kive API on a user''s behalf.


  Tokens are issued from https://mcp.kive.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kive
provider_slug: kive
schemes:
- flows:
  - authorizationUrl: https://mcp.kive.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.kive.ai/oauth/token
  name: KiveMCPOAuth
  source: https://mcp.kive.ai/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- kive:mcp
- offline_access
scopes:
- description: Access the Kive MCP server on behalf of the authorizing user. Per Kive's MCP documentation this authorization allows a client to view and edit Kive assets, set up products, and spend Kive credits for supported generation actions.
  flows:
  - authorizationCode
  scope: kive:mcp
- description: Issue a refresh token so the client can keep access without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
slug: kive-scopes
source_filename: kive-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.kive.ai/.well-known/oauth-authorization-server\ndocs: https://kive.ai/docs/mcp/overview.md\nnotes: >-\n  Scopes are advertised by the Kive MCP authorization server (RFC 8414) and\n  echoed by its protected-resource metadata (RFC 9728). Kive exposes a single\n  coarse-grained product scope rather than per-resource scopes; the effective\n  permission boundary is the authorizing user's Kive workspace role and the\n  workspace credit balance, both enforced server-side at call time.\nschemes:\n- name: KiveMCPOAuth\n  source: https://mcp.kive.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.kive.ai/oauth/authorize\n    tokenUrl: https://mcp.kive.ai/oauth/token\nscopes:\n- scope: kive:mcp\n  description: >-\n    Access the Kive MCP server on behalf of the authorizing user. Per Kive's MCP\n    documentation this authorization allows a client to view and\
  \ edit Kive\n    assets, set up products, and spend Kive credits for supported generation\n    actions.\n  flows: [authorizationCode]\n  sources: [https://mcp.kive.ai/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Issue a refresh token so the client can keep access without\n    re-prompting the user.\n  flows: [authorizationCode]\n  sources: [https://mcp.kive.ai/.well-known/oauth-authorization-server]\nenforcement:\n  model: workspace-permission-and-credit\n  notes: >-\n    Kive enforces workspace access, account permissions, and credit availability\n    independently of the granted scope. A scoped token cannot exceed the\n    authorizing user's workspace role.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kive/refs/heads/main/scopes/kive-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- SaaS
- Artificial Intelligence
- Generative AI
- Creative
- Product Photography
- Digital Asset Management
- E-Commerce
- Images
- Video
- MCP
token_urls:
- https://mcp.kive.ai/oauth/token
---
