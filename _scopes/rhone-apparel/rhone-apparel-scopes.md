---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rhone Apparel Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from scopes_supported in the OIDC discovery document served on Rhone's customer-account host. Descriptions are the platform meaning of each scope; Rhone publishes no scope reference of its own.
overview: 'Rhone Apparel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rhone Apparel
provider_slug: rhone-apparel
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rhone-apparel-scopes
source_filename: rhone-apparel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://account.rhone.com/.well-known/openid-configuration\nnote: >-\n  Scopes read verbatim from scopes_supported in the OIDC discovery document served on Rhone's\n  customer-account host. Descriptions are the platform meaning of each scope; Rhone publishes no\n  scope reference of its own.\nauthorization_server: https://shopify.com/authentication/2497784\nscope_count: 4\nscopes:\n  - name: openid\n    description: Standard OIDC scope - issues an ID token identifying the signed-in Rhone customer.\n  - name: email\n    description: Releases the customer's email and email_verified claims.\n  - name: 'customer-account-api:full'\n    description: Full access to the Shopify Customer Account API for the signed-in Rhone customer (orders, addresses, profile).\n  - name: 'customer-account-mcp-api:full'\n    description: Full access to the Customer Account MCP API - the authenticated, customer-scoped agent surface alongside the anonymous\
  \ storefront UCP/MCP endpoint.\nx-evidence:\n  fetched: '2026-08-26'\n  url: https://account.rhone.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhone-apparel/refs/heads/main/scopes/rhone-apparel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Activewear
- Company
token_urls: []
---
