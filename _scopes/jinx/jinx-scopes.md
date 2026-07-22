---
authorization_urls:
- https://shopify.com/authentication/27716059229/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jinx Scopes
name_suffix: OAuth Scopes
note: OAuth scopes advertised by the store's Shopify Customer Account API OIDC discovery document (scopes_supported). These govern customer-account access on the storefront, including the customer-account MCP surface; there is no first-party Jinx API with its own scope registry.
overview: 'Jinx publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jinx API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/27716059229/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jinx
provider_slug: jinx
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/27716059229/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/27716059229/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/jinx-openid-configuration.json
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
- description: Access the customer's email address and verification status.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: jinx-scopes
source_filename: jinx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://thinkjinx.com/.well-known/openid-configuration\nnote: >-\n  OAuth scopes advertised by the store's Shopify Customer Account API OIDC\n  discovery document (scopes_supported). These govern customer-account access on\n  the storefront, including the customer-account MCP surface; there is no\n  first-party Jinx API with its own scope registry.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/jinx-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/27716059229/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/27716059229/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/jinx-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address and verification status.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/jinx-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/jinx-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/jinx-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jinx/refs/heads/main/scopes/jinx-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Pet Food
- Pet Nutrition
- Ecommerce
- Direct to Consumer
- Dogs
- Cats
- Shopify
token_urls:
- https://shopify.com/authentication/27716059229/oauth/token
---
