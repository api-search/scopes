---
authorization_urls:
- https://account.skullcandy.com/authentication/oauth/authorize
description: ''
docs: https://shopify.dev/docs/api/customer
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Skullcandy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Skullcandy publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Skullcandy API on a user''s behalf.


  Tokens are issued from https://account.skullcandy.com/authentication/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Skullcandy
provider_slug: skullcandy
schemes:
- flows:
  - authorizationUrl: https://account.skullcandy.com/authentication/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://account.skullcandy.com/authentication/oauth/token
  name: ShopifyCustomerAccountOIDC
  source: well-known/skullcandy-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: Standard OpenID Connect scope; issues an ID token identifying the customer.
  flows:
  - authorizationCode
  scope: openid
- description: Grants access to the customer's email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in customer (orders, addresses, profile).
  flows:
  - authorizationCode
  scope: customer-account-api:full
- description: Full access to the customer-scoped Model Context Protocol surface of the Customer Account API.
  flows:
  - authorizationCode
  scope: customer-account-mcp-api:full
slug: skullcandy-scopes
source_filename: skullcandy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://skullcandy.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  source: well-known/skullcandy-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://account.skullcandy.com/authentication/oauth/authorize\n    tokenUrl: https://account.skullcandy.com/authentication/oauth/token\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; issues an ID token identifying the customer.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/skullcandy-openid-configuration.json\n- scope: email\n  description: Grants access to the customer's email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/skullcandy-openid-configuration.json\n- scope: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in\
  \ customer (orders, addresses, profile).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/skullcandy-openid-configuration.json\n- scope: customer-account-mcp-api:full\n  description: Full access to the customer-scoped Model Context Protocol surface of the Customer Account API.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/skullcandy-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skullcandy/refs/heads/main/scopes/skullcandy-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Consumer Electronics
- Audio
- Headphones
- E-Commerce
- Retail
- Shopify
- Agentic Commerce
- MCP
- Universal Commerce Protocol
token_urls:
- https://account.skullcandy.com/authentication/oauth/token
---
