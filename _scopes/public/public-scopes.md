---
authorization_urls: []
description: ''
docs: https://public.com/api/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Public Scopes
name_suffix: OAuth Scopes
note: Scopes advertised by Public's hosted MCP server via its RFC 9728 OAuth 2.0 Protected Resource metadata. The MCP OAuth flow (used by Claude/ChatGPT connectors) authorizes against the Public authorization server below. The direct Trading API (api.public.com) instead uses personal secret keys exchanged for short-lived bearer JWTs (see authentication/).
overview: 'Public publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Public API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Public
provider_slug: public
schemes:
- authorization_servers:
  - https://prod-api.154310543964.hellopublic.com/userapiauthservice/oauth2
  bearer_methods_supported:
  - header
  name: OAuth2
  source: https://mcp.public.com/.well-known/oauth-protected-resource
scope_count: 4
scope_names:
- trading.read
- trading.write
- marketdata
- openid
scopes:
- description: Read access to accounts, portfolio, positions, and order/transaction history.
  flows: []
  scope: trading.read
- description: Place, replace, and cancel orders and perform trading actions on the account.
  flows: []
  scope: trading.write
- description: Access real-time and historical market data (quotes, bars, option chains, greeks).
  flows: []
  scope: marketdata
- description: OpenID Connect authentication of the connecting user/agent.
  flows: []
  scope: openid
slug: public-scopes
source_filename: public-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.public.com/.well-known/oauth-protected-resource\ndocs: https://public.com/api/docs\nnote: >-\n  Scopes advertised by Public's hosted MCP server via its RFC 9728 OAuth 2.0\n  Protected Resource metadata. The MCP OAuth flow (used by Claude/ChatGPT\n  connectors) authorizes against the Public authorization server below. The\n  direct Trading API (api.public.com) instead uses personal secret keys\n  exchanged for short-lived bearer JWTs (see authentication/).\nschemes:\n- name: OAuth2\n  source: https://mcp.public.com/.well-known/oauth-protected-resource\n  authorization_servers:\n  - https://prod-api.154310543964.hellopublic.com/userapiauthservice/oauth2\n  bearer_methods_supported:\n  - header\nscopes:\n- scope: trading.read\n  description: Read access to accounts, portfolio, positions, and order/transaction history.\n  sources: [mcp.public.com oauth-protected-resource]\n- scope: trading.write\n  description: Place,\
  \ replace, and cancel orders and perform trading actions on the account.\n  sources: [mcp.public.com oauth-protected-resource]\n- scope: marketdata\n  description: Access real-time and historical market data (quotes, bars, option chains, greeks).\n  sources: [mcp.public.com oauth-protected-resource]\n- scope: openid\n  description: OpenID Connect authentication of the connecting user/agent.\n  sources: [mcp.public.com oauth-protected-resource]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public/refs/heads/main/scopes/public-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Consumer
- Investing
- Brokerage
- Trading
- Fintech
- Stocks
- Options
- Crypto
- Market Data
- Agentic
- MCP
token_urls: []
---
