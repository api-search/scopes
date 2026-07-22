---
authorization_urls:
- https://shopify.com/authentication/26030735465/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tenlittle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ten Little publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ten Little API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/26030735465/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ten Little
provider_slug: tenlittle
schemes:
- flows:
  - authorizationUrl: https://shopify.com/authentication/26030735465/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/26030735465/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/tenlittle-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access to the customer's email address.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in shopper.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Shopify Customer Account MCP API for the signed-in shopper.
  flows: []
  scope: customer-account-mcp-api:full
slug: tenlittle-scopes
source_filename: tenlittle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tenlittle.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\n# scopes_supported published verbatim by the Shopify Customer Account OIDC\n# discovery document served on the tenlittle.com domain. These are Shopify\n# platform scopes for shopper (customer-account) access, not a first-party\n# Ten Little API scope model.\nfirst_party: false\nprovider: Shopify (Customer Account API)\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/tenlittle-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/26030735465/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/26030735465/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n  sources: [well-known/tenlittle-openid-configuration.json]\n- scope: email\n  description: Access to the customer's email address.\n  sources:\
  \ [well-known/tenlittle-openid-configuration.json]\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in shopper.\n  sources: [well-known/tenlittle-openid-configuration.json]\n- scope: customer-account-mcp-api:full\n  description: Full access to the Shopify Customer Account MCP API for the signed-in shopper.\n  sources: [well-known/tenlittle-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenlittle/refs/heads/main/scopes/tenlittle-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Retail
- E-commerce
- Consumer Goods
- Children
- Footwear
- Direct-to-Consumer
- Shopify
token_urls:
- https://shopify.com/authentication/26030735465/oauth/token
---
