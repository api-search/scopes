---
authorization_urls:
- https://shopify.com/authentication/56010965185/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Hero Bread Scopes
name_suffix: OAuth Scopes
note: Scopes are read from the live RFC 8414 authorization-server metadata served on Hero Bread's own storefront host. The authorization server itself is Shopify's customer-accounts issuer, scoped to this merchant's shop id (56010965185). No OpenAPI declares these — the discovery document is the only published source.
overview: 'Hero Bread publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hero Bread API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/56010965185/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hero Bread
provider_slug: hero-bread
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/56010965185/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/56010965185/oauth/token
  issuer: https://shopify.com/authentication/56010965185
  name: shopify-customer-accounts
  source: well-known/hero-bread-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the buyer's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the customer account API for this store (orders, addresses, subscriptions).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API for this store — the authenticated agent surface.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: hero-bread-scopes
source_filename: hero-bread-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://shop.hero.co/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are read from the live RFC 8414 authorization-server metadata served on Hero Bread's own\n  storefront host. The authorization server itself is Shopify's customer-accounts issuer, scoped to\n  this merchant's shop id (56010965185). No OpenAPI declares these — the discovery document is the\n  only published source.\nschemes:\n- name: shopify-customer-accounts\n  issuer: https://shopify.com/authentication/56010965185\n  source: well-known/hero-bread-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/56010965185/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/56010965185/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication for the buyer.\n  flows: [authorizationCode]\n  sources: [well-known/hero-bread-oauth-authorization-server.json]\n\
  - scope: email\n  description: Access to the buyer's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/hero-bread-oauth-authorization-server.json]\n- scope: customer-account-api:full\n  description: Full access to the customer account API for this store (orders, addresses, subscriptions).\n  flows: [authorizationCode]\n  sources: [well-known/hero-bread-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API for this store — the authenticated agent surface.\n  flows: [authorizationCode]\n  sources: [well-known/hero-bread-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hero-bread/refs/heads/main/scopes/hero-bread-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agent Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
token_urls:
- https://shopify.com/authentication/56010965185/oauth/token
---
