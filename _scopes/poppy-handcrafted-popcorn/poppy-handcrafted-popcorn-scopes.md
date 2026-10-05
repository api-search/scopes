---
authorization_urls:
- https://shopify.com/authentication/42483876008/oauth/authorize
description: ''
docs: ''
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: probed
name: Poppy Handcrafted Popcorn Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securitySchemes because there is no OpenAPI. These are the scopes_supported values the provider's own live OIDC discovery document advertises for its customer-account authorization server. Descriptions state the standard meaning of each scope; the provider publishes no scope reference page of its own.
overview: 'Poppy Handcrafted Popcorn publishes 4 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Poppy Handcrafted Popcorn API on a user''s behalf.


  Tokens are issued from https://shopify.com/authentication/42483876008/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Poppy Handcrafted Popcorn
provider_slug: poppy-handcrafted-popcorn
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect sign-in; requests an ID token identifying the customer.
  flows: []
  scope: openid
- description: Access to the customer's email address claim.
  flows: []
  scope: email
- description: Full access to the authenticated customer's account data - orders, addresses, payment methods.
  flows: []
  scope: customer-account-api:full
- description: Full access to the authenticated customer's account through the MCP transport. This is the scope that lets an agent act on a signed-in buyer's account rather than anonymously.
  flows: []
  scope: customer-account-mcp-api:full
slug: poppy-handcrafted-popcorn-scopes
source_filename: poppy-handcrafted-popcorn-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://poppyhandcraftedpopcorn.com/.well-known/openid-configuration (HTTP 200)\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securitySchemes because there is no OpenAPI.\n  These are the scopes_supported values the provider's own live OIDC discovery document\n  advertises for its customer-account authorization server. Descriptions state the standard\n  meaning of each scope; the provider publishes no scope reference page of its own.\ndocs: null\nissuer: https://shopify.com/authentication/42483876008\nflows:\n- type: authorization_code\n  pkce_required_method: S256\n  authorization_url: https://shopify.com/authentication/42483876008/oauth/authorize\n  token_url: https://shopify.com/authentication/42483876008/oauth/token\nscope_count: 4\nscopes:\n- name: openid\n  description: OpenID Connect sign-in; requests an ID token identifying the customer.\n  standard: OIDC Core 1.0\n- name: email\n  description: Access to the customer's\
  \ email address claim.\n  standard: OIDC Core 1.0\n- name: 'customer-account-api:full'\n  description: Full access to the authenticated customer's account data - orders, addresses, payment methods.\n  standard: Shopify Customer Account API\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the authenticated customer's account through the MCP transport. This is the\n    scope that lets an agent act on a signed-in buyer's account rather than anonymously.\n  standard: Shopify Customer Account MCP API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppy-handcrafted-popcorn/refs/heads/main/scopes/poppy-handcrafted-popcorn-scopes.yml
summary_line: 4 scopes · authorization_code
tags:
- Company
- Food and Beverage
- Consumer Packaged Goods
- Retail
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Snacks
token_bound: false
token_urls:
- https://shopify.com/authentication/42483876008/oauth/token
---
