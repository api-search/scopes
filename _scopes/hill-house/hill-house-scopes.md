---
authorization_urls:
- https://account.hillhousehome.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hill House Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hill House publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hill House API on a user''s behalf.


  Tokens are issued from https://account.hillhousehome.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hill House
provider_slug: hill-house
schemes:
- flows:
  - authorizationUrl: https://account.hillhousehome.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.hillhousehome.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/9321794
  name: ShopifyCustomerAccountOIDC
  source: well-known/hill-house-openid-configuration.json
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
- description: Access the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-scoped Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: hill-house-scopes
source_filename: hill-house-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://hillhousehome.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/hill-house-openid-configuration.json\n  issuer: https://shopify.com/authentication/9321794\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.hillhousehome.com/authentication/oauth/authorize\n    tokenUrl: https://account.hillhousehome.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the authenticated customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n\
  \  description: Full access to the customer-scoped Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hill-house/refs/heads/main/scopes/hill-house-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-commerce
- Retail
- Home Goods
- Apparel
- Direct to Consumer
- Consumer Brand
- Shopify
- MCP
token_urls:
- https://account.hillhousehome.com/authentication/oauth/token
---
