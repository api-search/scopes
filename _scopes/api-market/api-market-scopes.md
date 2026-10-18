---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Api Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'API.market publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the API.market API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: API.market
provider_slug: api-market
schemes: []
scope_count: 2
scope_names:
- mcp:use
- offline_access
scopes:
- description: Use the API.market MCP gateway (the only scope the protected-resource document for https://api.market/api/mcp/gateway lists).
  flows: []
  scope: mcp:use
- description: Issue a refresh token (grant_types_supported includes refresh_token).
  flows: []
  scope: offline_access
slug: api-market-scopes
source_filename: api-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: https://api.market/.well-known/oauth-authorization-server\nscopes:\n- name: mcp:use\n  description: Use the API.market MCP gateway (the only scope the protected-resource document for https://api.market/api/mcp/gateway\n    lists).\n- name: offline_access\n  description: Issue a refresh token (grant_types_supported includes refresh_token).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-market/refs/heads/main/scopes/api-market-scopes.yml
summary_line: 2 scopes
tags:
- API Marketplace
- MCP
- AI Agents
- API Monetization
- Subscription
- Usage Metering
- Authentication
token_bound: false
token_urls: []
---
