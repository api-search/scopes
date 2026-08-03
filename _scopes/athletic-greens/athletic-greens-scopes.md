---
authorization_urls:
- https://account.drinkag1.com/authentication/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Athletic Greens Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the live RFC 8414 authorization-server metadata served on AG1's hosts. AG1 publishes no scope reference page; descriptions below state the scope's effect as observed on the protected surfaces, and are marked derived where the metadata carries no description.
overview: 'AG1 publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AG1 API on a user''s behalf.


  Tokens are issued from https://account.drinkag1.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AG1
provider_slug: athletic-greens
schemes:
- flows:
  - authorizationUrl: https://account.drinkag1.com/authentication/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://account.drinkag1.com/authentication/oauth/token
  issuer: https://shopify.com/authentication/15234600
  name: shopify-customer-accounts-oidc
  source: well-known/athletic-greens-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect - issue an ID token identifying the AG1 customer.
  flows:
  - authorizationCode
  scope: openid
- description: Release the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the authenticated AG1 customer - orders, subscriptions, addresses, payment methods, store credit.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP server at https://account.drinkag1.com/customer/api/mcp - order status, store credit balances and return requests on the authenticated customer's behalf.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: athletic-greens-scopes
source_filename: athletic-greens-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://shop.drinkag1.com/.well-known/oauth-authorization-server\nnote: Scopes are read verbatim from the live RFC 8414 authorization-server metadata\n  served on AG1's hosts. AG1 publishes no scope reference page; descriptions below\n  state the scope's effect as observed on the protected surfaces, and are marked\n  derived where the metadata carries no description.\nschemes:\n- name: shopify-customer-accounts-oidc\n  source: well-known/athletic-greens-oauth-authorization-server.json\n  issuer: https://shopify.com/authentication/15234600\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.drinkag1.com/authentication/oauth/authorize\n    tokenUrl: https://account.drinkag1.com/authentication/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect - issue an ID token identifying the AG1 customer.\n  description_method: derived\n  flows: [authorizationCode]\n  sources: [well-known/athletic-greens-oauth-authorization-server.json]\n\
  - scope: email\n  description: Release the customer's email address and email_verified claim.\n  description_method: derived\n  flows: [authorizationCode]\n  sources: [well-known/athletic-greens-oauth-authorization-server.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the authenticated\n    AG1 customer - orders, subscriptions, addresses, payment methods, store credit.\n  description_method: derived\n  flows: [authorizationCode]\n  sources: [well-known/athletic-greens-oauth-authorization-server.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP server at\n    https://account.drinkag1.com/customer/api/mcp - order status, store credit balances\n    and return requests on the authenticated customer's behalf.\n  description_method: derived\n  flows: [authorizationCode]\n  sources: [well-known/athletic-greens-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletic-greens/refs/heads/main/scopes/athletic-greens-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Health
- Nutrition
- Supplements
- Direct to Consumer
- Ecommerce
- Subscription
- Wellness
- Agentic Commerce
- MCP
- UCP
- Shopify
- GraphQL
token_urls:
- https://account.drinkag1.com/authentication/oauth/token
---
