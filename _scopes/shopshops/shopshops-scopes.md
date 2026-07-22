---
authorization_urls:
- https://shopify.com/authentication/59001897017/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Shopshops Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ShopShops publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ShopShops API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/59001897017/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ShopShops
provider_slug: shopshops
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/59001897017/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/59001897017/oauth/token
  name: CustomerAccountOIDC
  source: well-known/shopshops-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the buyer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the buyer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the buyer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API, enabling agent-driven access to the buyer's account over the Model Context Protocol.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: shopshops-scopes
source_filename: shopshops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.shopshopslive.com/.well-known/openid-configuration\nschemes:\n- name: CustomerAccountOIDC\n  source: well-known/shopshops-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/59001897017/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/59001897017/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the buyer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the buyer's email address and verification status.\n  flows: [authorizationCode]\n- scope: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API for the buyer.\n  flows: [authorizationCode]\n- scope: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the Customer Account MCP API, enabling agent-driven access to\n    the buyer's account over\
  \ the Model Context Protocol.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopshops/refs/heads/main/scopes/shopshops-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- Ecommerce
- Marketplace
- Live Shopping
- Luxury Resale
- Agent Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/59001897017/oauth/token
---
