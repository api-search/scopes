---
authorization_urls:
- https://shopify.com/authentication/1239679049/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: To The Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TO THE MARKET publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TO THE MARKET API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/1239679049/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TO THE MARKET
provider_slug: to-the-market
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/1239679049/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/1239679049/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/to-the-market-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-account MCP API surface for agent-driven customer actions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: to-the-market-scopes
source_filename: to-the-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tothemarket.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/to-the-market-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/1239679049/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/1239679049/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/to-the-market-openid-configuration.json]\n- scope: email\n  description: Access to the authenticated customer's email address.\n  flows: [authorizationCode]\n  sources: [well-known/to-the-market-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows:\
  \ [authorizationCode]\n  sources: [well-known/to-the-market-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface for agent-driven customer actions.\n  flows: [authorizationCode]\n  sources: [well-known/to-the-market-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/to-the-market/refs/heads/main/scopes/to-the-market-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Commerce
- Ecommerce
- Sustainability
- Supply Chain
- Agent Commerce
- Shopify
- MCP
token_urls:
- https://shopify.com/authentication/1239679049/oauth/token
---
