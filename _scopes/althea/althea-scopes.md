---
authorization_urls:
- https://shopify.com/authentication/9377939535/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Althea Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Althea publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Althea API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/9377939535/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Althea
provider_slug: althea
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/9377939535/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/9377939535/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/althea-openid-configuration.json
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
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API for agent-driven customer account actions.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: althea-scopes
source_filename: althea-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://us.althea.kr/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/althea-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/9377939535/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/9377939535/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the authenticated customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Customer Account MCP API for agent-driven customer\
  \ account actions.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/althea/refs/heads/main/scopes/althea-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Retail
- Beauty
- Cosmetics
- K-Beauty
- Skincare
- Agent Commerce
- Shopify
token_urls:
- https://shopify.com/authentication/9377939535/oauth/token
---
