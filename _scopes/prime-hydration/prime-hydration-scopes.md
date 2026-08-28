---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Prime Hydration Scopes
name_suffix: OAuth Scopes
note: Prime Hydration publishes no scopes reference page - there is no developer portal to host one. These four scopes are the ones the provider's own authorization-server metadata advertises for the Shopify Customer Accounts issuer bound to this store (shop 60993569009). The UCP shopping MCP endpoint at /api/ucp/mcp is anonymous and consumes no scope.
overview: 'Prime Hydration uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prime Hydration
provider_slug: prime-hydration
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: prime-hydration-scopes
source_filename: prime-hydration-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported read verbatim from https://drinkprime.com/.well-known/openid-configuration\n  (HTTP 200, probed 2026-08-26) and https://drinkprime.com/.well-known/oauth-authorization-server\n  (HTTP 200, byte-identical).\ndocs: null\nnote: >-\n  Prime Hydration publishes no scopes reference page - there is no developer portal to host one.\n  These four scopes are the ones the provider's own authorization-server metadata advertises for\n  the Shopify Customer Accounts issuer bound to this store (shop 60993569009). The UCP shopping\n  MCP endpoint at /api/ucp/mcp is anonymous and consumes no scope.\nauthorization_server: https://shopify.com/authentication/60993569009\nflow: authorization_code (PKCE S256)\nscope_count: 4\nscopes:\n- name: openid\n  description: >-\n    Standard OpenID Connect scope. Requests an ID token identifying the signed-in shopper.\n  standard: OpenID Connect Core 1.0\n- name: email\n  description:\
  \ >-\n    Standard OpenID Connect scope. Releases the email and email_verified claims for the\n    signed-in shopper.\n  standard: OpenID Connect Core 1.0\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for the authenticated shopper - their own\n    orders, addresses, payment methods and profile on the PRIME store.\n  standard: Shopify Customer Accounts\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API for the authenticated shopper - the\n    agent-facing projection of that same account data.\n  standard: Shopify Customer Accounts\n  note: >-\n    A probe of POST https://orders.drinkprime.com/customer-account-api/mcp returned HTTP 404\n    anonymously; the customer-account MCP surface, unlike the storefront UCP surface, is not\n    anonymously discoverable and its tool schemas would require an authenticated shopper session.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-hydration/refs/heads/main/scopes/prime-hydration-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Beverages
- Consumer Packaged Goods
- Food and Beverage
- Retail
- E-Commerce
- Direct to Consumer
- Agentic Commerce
- Universal Commerce Protocol
- Model Context Protocol
- Shopify
- Sports Nutrition
token_urls: []
---
