---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: The Naked Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Naked Market publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Naked Market API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Naked Market
provider_slug: the-naked-market
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication (ID token issuance).
  flows: []
  scope: openid
- description: Access to the customer's email address and verification status claims.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the customer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the customer.
  flows: []
  scope: customer-account-mcp-api:full
slug: the-naked-market-scopes
source_filename: the-naked-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://thenakedmarket.com/.well-known/openid-configuration (scopes_supported, live fetch)\nname: The Naked Market OAuth scopes\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  Scopes are published in the store's OIDC discovery document, served by Shopify Customer\n  Accounts for this storefront. They gate the Shopify Customer Account API and its MCP surface\n  for authenticated customers of this store.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (ID token issuance).\n- scope: email\n  description: Access to the customer's email address and verification status claims.\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the customer.\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API on behalf of the customer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-naked-market/refs/heads/main/scopes/the-naked-market-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Consumer
- Consumer Packaged Goods
- Food and Beverage
- Direct to Consumer
- Snacks
- Brand Incubator
- E-Commerce
token_urls: []
---
