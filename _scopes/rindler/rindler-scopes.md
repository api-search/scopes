---
authorization_urls:
- https://mcp.rindler.ai/auth/authorize
description: ''
docs: https://rindler.ai/docs/auth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rindler Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rindler publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rindler API on a user''s behalf.


  Tokens are issued from https://mcp.rindler.ai/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rindler
provider_slug: rindler
schemes:
- flows:
  - authorizationUrl: https://mcp.rindler.ai/auth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://mcp.rindler.ai/auth/register-client
    tokenUrl: https://mcp.rindler.ai/auth/token
  name: OAuth2
  source: https://mcp.rindler.ai/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 3
scope_names:
- site:*:read
- site:*:write
- site:*:schema
scopes:
- description: Read structured content and records from a mapped site session.
  flows:
  - authorizationCode
  scope: site:*:read
- description: Dispatch mapped write/action operations against a site session (submit forms, add to cart, stage moves, etc.).
  flows:
  - authorizationCode
  scope: site:*:write
- description: Access the typed schema/shape of a mapped site's tools and structured outputs.
  flows:
  - authorizationCode
  scope: site:*:schema
slug: rindler-scopes
source_filename: rindler-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.rindler.ai/.well-known/oauth-protected-resource\ndocs: https://rindler.ai/docs/auth\nschemes:\n  - name: OAuth2\n    type: oauth2\n    source: https://mcp.rindler.ai/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        pkce: S256\n        authorizationUrl: https://mcp.rindler.ai/auth/authorize\n        tokenUrl: https://mcp.rindler.ai/auth/token\n        registrationUrl: https://mcp.rindler.ai/auth/register-client\nscopes:\n  - scope: 'site:*:read'\n    description: Read structured content and records from a mapped site session.\n    flows: [authorizationCode]\n    sources: [well-known/rindler-mcp-oauth-protected-resource.json]\n  - scope: 'site:*:write'\n    description: Dispatch mapped write/action operations against a site session (submit forms, add to cart, stage moves, etc.).\n    flows: [authorizationCode]\n    sources: [well-known/rindler-mcp-oauth-protected-resource.json]\n\
  \  - scope: 'site:*:schema'\n    description: Access the typed schema/shape of a mapped site's tools and structured outputs.\n    flows: [authorizationCode]\n    sources: [well-known/rindler-mcp-oauth-protected-resource.json]\nnotes: >-\n  Scopes use a site:<site>:<capability> pattern; the '*' segment in the\n  advertised scopes_supported denotes the wildcard/all-sites grant surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rindler/refs/heads/main/scopes/rindler-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Web Automation
- Browser Automation
- Structured Data
- Website to API
- Agent Tools
- Y Combinator
token_urls:
- https://mcp.rindler.ai/auth/token
---
