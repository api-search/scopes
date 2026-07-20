---
authorization_urls:
- https://app.gripsintelligence.com/authorize
description: ''
docs: https://app.gripsintelligence.com/.well-known/oauth-protected-resource/api/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Grips Intelligence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Grips Intelligence publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Grips Intelligence API on a user''s behalf.


  Tokens are issued from https://app.gripsintelligence.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Grips Intelligence
provider_slug: grips-intelligence
schemes:
- flows:
  - authorizationUrl: https://app.gripsintelligence.com/authorize
    flow: authorizationCode
    tokenUrl: https://app.gripsintelligence.com/token
  name: peekdDataMcpOAuth
  source: https://app.gripsintelligence.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the Peekd Data MCP server (https://app.gripsintelligence.com/api/mcp) exposing Grips Intelligence e-commerce intelligence data to agents.
  flows:
  - authorizationCode
  scope: mcp
slug: grips-intelligence-scopes
source_filename: grips-intelligence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://app.gripsintelligence.com/.well-known/oauth-authorization-server\ndocs: https://app.gripsintelligence.com/.well-known/oauth-protected-resource/api/mcp\nschemes:\n- name: peekdDataMcpOAuth\n  source: https://app.gripsintelligence.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.gripsintelligence.com/authorize\n    tokenUrl: https://app.gripsintelligence.com/token\nscopes:\n- scope: mcp\n  description: >-\n    Access to the Peekd Data MCP server (https://app.gripsintelligence.com/api/mcp)\n    exposing Grips Intelligence e-commerce intelligence data to agents.\n  flows: [authorizationCode]\n  sources: [https://app.gripsintelligence.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grips-intelligence/refs/heads/main/scopes/grips-intelligence-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- E-commerce Intelligence
- Competitive Intelligence
- Market Research
- Analytics
- Product Intelligence
- Retail
- Data
token_urls:
- https://app.gripsintelligence.com/token
---
