---
authorization_urls:
- https://shopify.com/authentication/73264758967/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Beautypie Scopes
name_suffix: OAuth Scopes
note: scopes_supported from the live Shopify Customer Account OIDC discovery document served under beautypie.com. These are Shopify platform scopes, not beautypie-defined.
overview: 'Beauty Pie publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Beauty Pie API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/73264758967/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Beauty Pie
provider_slug: beautypie
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/73264758967/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/73264758967/oauth/token
  name: ShopifyCustomerAccountOAuth2
  source: well-known/beautypie-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in customer.
  flows:
  - authorizationCode
  scope: openid
- description: Access the customer's email address and email_verified claim.
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
slug: beautypie-scopes
source_filename: beautypie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.beautypie.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nnote: >-\n  scopes_supported from the live Shopify Customer Account OIDC discovery document\n  served under beautypie.com. These are Shopify platform scopes, not beautypie-defined.\nschemes:\n- name: ShopifyCustomerAccountOAuth2\n  source: well-known/beautypie-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/73264758967/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/73264758967/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/beautypie-openid-configuration.json]\n- scope: email\n  description: Access the customer's email address and email_verified claim.\n  flows: [authorizationCode]\n  sources:\
  \ [well-known/beautypie-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/beautypie-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer.\n  flows: [authorizationCode]\n  sources: [well-known/beautypie-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beautypie/refs/heads/main/scopes/beautypie-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Beauty
- Skincare
- Cosmetics
- Ecommerce
- Direct-to-Consumer
- Membership
- Retail
- Shopify
- Storefront MCP
token_urls:
- https://shopify.com/authentication/73264758967/oauth/token
---
