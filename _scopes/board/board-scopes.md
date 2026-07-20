---
authorization_urls:
- https://account.board.fun/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Board Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Board publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Board API on a user''s behalf.


  Tokens are issued from https://account.board.fun/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Board
provider_slug: board
schemes:
- flows:
  - authorizationUrl: https://account.board.fun/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.board.fun/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: https://board.fun/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface (agent-driven commerce via UCP).
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: board-scopes
source_filename: board-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://board.fun/.well-known/openid-configuration\nnotes: >-\n  OAuth/OIDC scopes advertised by Board's Shopify Customer Account authorization\n  server. The customer-account-mcp-api:full scope gates the UCP agent-commerce\n  MCP surface.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: https://board.fun/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.board.fun/authentication/oauth/authorize\n    tokenUrl: https://account.board.fun/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows:\n  - authorizationCode\n- scope: email\n  description: Access the customer's email address and verification status.\n  flows:\n  - authorizationCode\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the buyer.\n  flows:\n\
  \  - authorizationCode\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface (agent-driven commerce via UCP).\n  flows:\n  - authorizationCode\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/board/refs/heads/main/scopes/board-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- E-Commerce
- Board Games
- Agent Commerce
- Universal Commerce Protocol
- Shopify
- MCP
token_urls:
- https://account.board.fun/authentication/oauth/token
---
