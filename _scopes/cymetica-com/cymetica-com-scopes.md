---
api_specs:
- filename: cymetica-com-eventtrader-public-api-openapi.yml
  format: yaml
  label: EventTrader Public API
  slug: eventtrader-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/openapi/cymetica-com-eventtrader-public-api-openapi.yml
authorization_urls:
- https://cymetica.com/oauth/authorize
description: ''
docs: https://cymetica.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cymetica Com Scopes
name_suffix: OAuth Scopes
note: The three scopes in the spec are exactly the scopes_supported in the RFC 8414 and RFC 9728 documents; no scopes/permissions reference page exists beyond those. OAuth tokens cannot withdraw (docs); withdraw is an API-key permission reserved for registered agent keys.
overview: 'Cymetica publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cymetica API on a user''s behalf.


  Tokens are issued from https://cymetica.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cymetica
provider_slug: cymetica-com
schemes:
- flows:
  - authorizationUrl: https://cymetica.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://cymetica.com/oauth/token
  name: OAuth2
  source: openapi/cymetica-com-eventtrader-public-api-openapi.yml
scope_count: 3
scope_names:
- portfolio
- read
- trade
scopes:
- description: Read portfolio positions
  flows:
  - authorizationCode
  scope: portfolio
- description: Read public and account data
  flows:
  - authorizationCode
  scope: read
- description: Place and cancel orders
  flows:
  - authorizationCode
  scope: trade
slug: cymetica-com-scopes
source_filename: cymetica-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/cymetica-com-eventtrader-public-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/cymetica-com-eventtrader-public-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cymetica.com/oauth/authorize\n    tokenUrl: https://cymetica.com/oauth/token\nscopes:\n- scope: portfolio\n  description: Read portfolio positions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\n- scope: read\n  description: Read public and account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\n- scope: trade\n  description: Place and cancel orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cymetica-com-eventtrader-public-api-openapi.yml\ndocs: https://cymetica.com/.well-known/oauth-authorization-server\nsources_searched:\n- 'https://cymetica.com/.well-known/oauth-authorization-server\
  \ (scopes_supported: read, portfolio, trade)'\n- https://cymetica.com/.well-known/oauth-protected-resource (scopes_supported identical)\n- https://cymetica.com/.well-known/mcp.json (authentication.oauth.scopes identical)\n- https://cymetica.com/api-docs (API key permissions read/trade/withdraw — a parallel permission model for keys,\n  not OAuth scopes)\nnote: The three scopes in the spec are exactly the scopes_supported in the RFC 8414 and RFC 9728 documents; no scopes/permissions\n  reference page exists beyond those. OAuth tokens cannot withdraw (docs); withdraw is an API-key permission reserved\n  for registered agent keys.\napi_key_permissions:\n- permission: read\n  description: market data / account reads\n- permission: trade\n  description: place/cancel orders\n- permission: withdraw\n  description: registered agent keys only — moves the agent's own balance through the standard withdrawal gates\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cymetica-com/refs/heads/main/scopes/cymetica-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Prediction Markets
- Cryptocurrency Exchange
- Trading
- AI Agents
- MCP
- Agent-Native
- Blockchain
- DeFi
- Financial Services
- Market Data
- A2A
- Real-Time
token_urls:
- https://cymetica.com/oauth/token
---
