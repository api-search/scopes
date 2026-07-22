---
authorization_urls:
- https://shopify.com/authentication/68449239327/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Source Beauty Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Source Beauty publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Source Beauty API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/68449239327/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Source Beauty
provider_slug: source-beauty
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/68449239327/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/68449239327/oauth/token
  name: ShopifyCustomerAccount
  source: https://sourcebeauty.com/.well-known/openid-configuration
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
- description: Access to the authenticated customer's email address.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API on behalf of the customer.
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for agent-driven customer-account operations.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: source-beauty-scopes
source_filename: source-beauty-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://sourcebeauty.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccount\n  source: https://sourcebeauty.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/68449239327/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/68449239327/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the customer.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the authenticated customer's email address.\n  flows: [authorizationCode]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the customer.\n  flows: [authorizationCode]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for\
  \ agent-driven customer-account operations.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/source-beauty/refs/heads/main/scopes/source-beauty-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beauty
- Cosmetics
- E-commerce
- Retail
- Marketplace
- Wellness
- Egypt
- Skincare
- Consumer
token_urls:
- https://shopify.com/authentication/68449239327/oauth/token
---
