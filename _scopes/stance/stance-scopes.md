---
authorization_urls:
- https://account.stance.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Stance Scopes
name_suffix: OAuth Scopes
note: OAuth scopes advertised by stance.com's OpenID Connect discovery document (Shopify Customer Account API). Captured verbatim from scopes_supported.
overview: 'Stance publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Stance API on a user''s behalf.


  Tokens are issued from https://account.stance.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Stance
provider_slug: stance
schemes:
- flows:
  - authorizationUrl: https://account.stance.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.stance.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/stance-openid-configuration.json
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
- description: Access to the authenticated customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: stance-scopes
source_filename: stance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://stance.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  OAuth scopes advertised by stance.com's OpenID Connect discovery document\n  (Shopify Customer Account API). Captured verbatim from scopes_supported.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/stance-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.stance.com/authentication/oauth/authorize\n    tokenUrl: https://account.stance.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token identifying the customer.\n  flows: [authorizationCode]\n  sources: [well-known/stance-openid-configuration.json]\n- scope: email\n  description: Access to the authenticated customer's email address and verification status.\n  flows: [authorizationCode]\n  sources: [well-known/stance-openid-configuration.json]\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile).\n  flows: [authorizationCode]\n  sources: [well-known/stance-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/stance-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stance/refs/heads/main/scopes/stance-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Apparel
- Retail
- E-commerce
- Socks
- Direct-to-Consumer
- Shopify
token_urls:
- https://account.stance.com/authentication/oauth/token
---
