---
authorization_urls:
- https://auth.gamma.app/oauth/authorize
description: ''
docs: https://developers.gamma.app/mcp/mcp-tools-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Gamma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gamma publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gamma API on a user''s behalf.


  Tokens are issued from https://auth.gamma.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gamma
provider_slug: gamma
schemes:
- flows:
  - authorizationUrl: https://auth.gamma.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://auth.gamma.app/oauth/token
  name: OAuth2
  source: https://auth.gamma.app/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- generate
- gamma:read
scopes:
- description: Create and generate gammas (presentations, documents, websites, social posts).
  flows:
  - authorizationCode
  scope: generate
- description: Read existing gammas, themes, folders, and analytics.
  flows:
  - authorizationCode
  scope: gamma:read
slug: gamma-scopes
source_filename: gamma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.gamma.app/.well-known/oauth-protected-resource\ndocs: https://developers.gamma.app/mcp/mcp-tools-reference\nnotes: >-\n  OAuth scopes apply to the Gamma remote MCP server / OAuth surface. The REST\n  Generate API itself authenticates with an X-API-KEY header and has no scope\n  model. Scopes discovered from the RFC 9728 protected-resource metadata and the\n  RFC 8414 authorization-server metadata at auth.gamma.app.\nschemes:\n- name: OAuth2\n  source: https://auth.gamma.app/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.gamma.app/oauth/authorize\n    tokenUrl: https://auth.gamma.app/oauth/token\nscopes:\n- scope: generate\n  description: Create and generate gammas (presentations, documents, websites, social posts).\n  flows: [authorizationCode]\n  sources: [https://mcp.gamma.app/.well-known/oauth-protected-resource]\n- scope: gamma:read\n  description:\
  \ Read existing gammas, themes, folders, and analytics.\n  flows: [authorizationCode]\n  sources: [https://mcp.gamma.app/.well-known/oauth-protected-resource]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gamma/refs/heads/main/scopes/gamma-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Productivity
- Presentations
- Documents
- Websites
- Artificial Intelligence
- Generative AI
- Content Generation
- Design
token_urls:
- https://auth.gamma.app/oauth/token
---
