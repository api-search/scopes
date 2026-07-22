---
authorization_urls:
- https://shopify.com/authentication/59458650296/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Byheart Scopes
name_suffix: OAuth Scopes
note: OAuth scopes advertised by the Shopify Customer Account API authorization server for the ByHeart store (issuer shopify.com/authentication/59458650296).
overview: 'ByHeart publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ByHeart API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/59458650296/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ByHeart
provider_slug: byheart
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/59458650296/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/59458650296/oauth/token
  name: shopifyCustomerAccountOIDC
  source: well-known/byheart-openid-configuration.json
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
- description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: byheart-scopes
source_filename: byheart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.byheart.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  OAuth scopes advertised by the Shopify Customer Account API authorization\n  server for the ByHeart store (issuer shopify.com/authentication/59458650296).\nschemes:\n- name: shopifyCustomerAccountOIDC\n  source: well-known/byheart-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/59458650296/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/59458650296/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token for the customer.\n  flows: [authorizationCode]\n  sources: [well-known/byheart-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources: [well-known/byheart-openid-configuration.json]\n\
  - scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer (orders, profile, addresses).\n  flows: [authorizationCode]\n  sources: [well-known/byheart-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API surface for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/byheart-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/byheart/refs/heads/main/scopes/byheart-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer
- Infant Nutrition
- Baby Formula
- Direct-to-Consumer
- Ecommerce
- Health
- Shopify
token_urls:
- https://shopify.com/authentication/59458650296/oauth/token
---
