---
authorization_urls:
- https://account.cotopaxi.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cotopaxi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cotopaxi publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cotopaxi API on a user''s behalf.


  Tokens are issued from https://account.cotopaxi.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cotopaxi
provider_slug: cotopaxi
schemes:
- flows:
  - authorizationUrl: https://account.cotopaxi.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.cotopaxi.com/authentication/oauth/token
  name: ShopifyCustomerAccountsOAuth2
  source: well-known/cotopaxi-oauth-authorization-server.json
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
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the authenticated Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: cotopaxi-scopes
source_filename: cotopaxi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cotopaxi.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnotes: >-\n  OAuth scopes advertised by the Cotopaxi Shopify Customer Accounts\n  authorization server (scopes_supported in the live discovery documents).\nschemes:\n- name: ShopifyCustomerAccountsOAuth2\n  source: well-known/cotopaxi-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.cotopaxi.com/authentication/oauth/authorize\n    tokenUrl: https://account.cotopaxi.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API for\
  \ the signed-in customer (orders, profile, addresses).\n  flows: [authorizationCode]\n- scope: 'customer-account-mcp-api:full'\n  description: Full access to the authenticated Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cotopaxi/refs/heads/main/scopes/cotopaxi-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Outdoor
- Apparel
- Ecommerce
- Retail
- Shopify
- MCP
token_urls:
- https://account.cotopaxi.com/authentication/oauth/token
---
