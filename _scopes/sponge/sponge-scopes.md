---
api_specs:
- filename: sponge-openapi-original.json
  format: json
  label: Sponge Wallet API
  slug: sponge-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/openapi/sponge-openapi-original.json
authorization_urls: []
description: Sponge's Wallet API is primarily bearer API-key authenticated, but the hosted MCP servers are fronted by an OAuth 2.0 / OIDC authorization server (dynamic client registration, S256 PKCE) whose discovery metadata advertises the scopes below. These scopes gate OAuth-connected MCP clients (e.g. Claude, ChatGPT).
docs: https://docs.paysponge.com/wallet/mcp.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Sponge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sponge publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sponge API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sponge
provider_slug: sponge
schemes:
- authorization_url: https://api.wallet.paysponge.com/oauth/authorize
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://api.wallet.paysponge.com
  name: OAuth2
  pkce: S256
  registration_url: https://api.wallet.paysponge.com/oauth/register
  revocation_url: https://api.wallet.paysponge.com/oauth/revoke
  source: well-known/sponge-openid-configuration.json
  token_url: https://api.wallet.paysponge.com/oauth/token
  type: oauth2
scope_count: 5
scope_names:
- openid
- mcp:tools
- wallet:read
- wallet:transfer
- sponge:all
scopes:
- description: OpenID Connect authentication of the connecting agent identity.
  flows: []
  scope: openid
- description: Access to the Sponge MCP tool surface for the authorized agent.
  flows: []
  scope: mcp:tools
- description: Read-only access to wallet addresses, balances, and transaction history.
  flows: []
  scope: wallet:read
- description: Authorize outbound transfers, swaps, and payments from the agent wallet.
  flows: []
  scope: wallet:transfer
- description: Full access to all Sponge wallet capabilities for the authorized agent.
  flows: []
  scope: sponge:all
slug: sponge-scopes
source_filename: sponge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.wallet.paysponge.com/.well-known/openid-configuration\ndocs: https://docs.paysponge.com/wallet/mcp.md\ndescription: >-\n  Sponge's Wallet API is primarily bearer API-key authenticated, but the hosted\n  MCP servers are fronted by an OAuth 2.0 / OIDC authorization server (dynamic\n  client registration, S256 PKCE) whose discovery metadata advertises the scopes\n  below. These scopes gate OAuth-connected MCP clients (e.g. Claude, ChatGPT).\nschemes:\n- name: OAuth2\n  type: oauth2\n  source: well-known/sponge-openid-configuration.json\n  issuer: https://api.wallet.paysponge.com\n  authorization_url: https://api.wallet.paysponge.com/oauth/authorize\n  token_url: https://api.wallet.paysponge.com/oauth/token\n  registration_url: https://api.wallet.paysponge.com/oauth/register\n  revocation_url: https://api.wallet.paysponge.com/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\nscopes:\n-\
  \ scope: openid\n  description: OpenID Connect authentication of the connecting agent identity.\n  sources: [well-known/sponge-openid-configuration.json]\n- scope: mcp:tools\n  description: Access to the Sponge MCP tool surface for the authorized agent.\n  sources: [well-known/sponge-openid-configuration.json]\n- scope: wallet:read\n  description: Read-only access to wallet addresses, balances, and transaction history.\n  sources: [well-known/sponge-openid-configuration.json]\n- scope: wallet:transfer\n  description: Authorize outbound transfers, swaps, and payments from the agent wallet.\n  sources: [well-known/sponge-openid-configuration.json]\n- scope: sponge:all\n  description: Full access to all Sponge wallet capabilities for the authorized agent.\n  sources: [well-known/sponge-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sponge/refs/heads/main/scopes/sponge-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Agent Payments
- AI Agents
- Wallets
- Cryptocurrency
- Payments
- Stablecoins
- x402
- MPP
- Financial Infrastructure
- MCP
- Fintech
- Cards
- Onramp
token_urls: []
---
