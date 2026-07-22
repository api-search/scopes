---
authorization_urls:
- https://shopify.com/authentication/26410184/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Artofsport Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 / OIDC scopes are provided by the Shopify Customer Accounts authorization server exposed on the Art of Sport storefront host (issuer https://shopify.com/authentication/26410184). These are Shopify platform scopes for authenticated customer-account access, not a first-party Art of Sport API.
overview: 'Artofsport publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Artofsport API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/26410184/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Artofsport
provider_slug: artofsport
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/26410184/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://shopify.com/authentication/26410184/oauth/token
  issuer: https://shopify.com/authentication/26410184
  name: ShopifyCustomerAccounts
  source: well-known/artofsport-openid-configuration.json
  type: oauth2
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; returns an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: artofsport-scopes
source_filename: artofsport-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://artofsport.com/.well-known/openid-configuration\nnote: >-\n  OAuth 2.0 / OIDC scopes are provided by the Shopify Customer Accounts authorization server exposed on\n  the Art of Sport storefront host (issuer https://shopify.com/authentication/26410184). These are\n  Shopify platform scopes for authenticated customer-account access, not a first-party Art of Sport API.\nschemes:\n- name: ShopifyCustomerAccounts\n  type: oauth2\n  source: well-known/artofsport-openid-configuration.json\n  issuer: https://shopify.com/authentication/26410184\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/26410184/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/26410184/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n  flows: [authorizationCode]\n- scope: email\n  description:\
  \ Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artofsport/refs/heads/main/scopes/artofsport-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Packaged Goods
- Personal Care
- Skincare
- Body Care
- Athletics
- Direct to Consumer
- E-commerce
- Shopify
token_urls:
- https://shopify.com/authentication/26410184/oauth/token
---
