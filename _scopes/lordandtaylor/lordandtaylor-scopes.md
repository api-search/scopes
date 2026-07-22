---
authorization_urls:
- https://account.lordandtaylor.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lordandtaylor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lord & Taylor publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lord & Taylor API on a user''s behalf.


  Tokens are issued from https://account.lordandtaylor.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lord & Taylor
provider_slug: lordandtaylor
schemes:
- flows:
  - authorizationUrl: https://account.lordandtaylor.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.lordandtaylor.com/authentication/oauth/token
  name: oauth2
  source: https://www.lordandtaylor.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API (order status, returns, store-credit balances) for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: lordandtaylor-scopes
source_filename: lordandtaylor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.lordandtaylor.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: oauth2\n  source: https://www.lordandtaylor.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.lordandtaylor.com/authentication/oauth/authorize\n    tokenUrl: https://account.lordandtaylor.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the signed-in customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile).\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full\
  \ access to the Customer Account MCP API (order status, returns, store-credit balances) for the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lordandtaylor/refs/heads/main/scopes/lordandtaylor-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Shopping
- Department Store
- Agentic Commerce
- MCP
token_urls:
- https://account.lordandtaylor.com/authentication/oauth/token
---
