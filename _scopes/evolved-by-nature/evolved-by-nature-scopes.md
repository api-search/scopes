---
authorization_urls: []
description: Scopes advertised by the Shopify Customer Accounts authorization servers named from Evolved By Nature's two storefront hosts. Identical on both storefronts. Evolved By Nature publishes no scope reference of its own.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Evolved By Nature Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Evolved By Nature publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Evolved By Nature API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evolved By Nature
provider_slug: evolved-by-nature
schemes: []
scope_count: 4
scope_names:
- openid
- email
- customer-account-api:full
- customer-account-mcp-api:full
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the buyer.
  flows: []
  scope: openid
- description: Access to the buyer's email address claim.
  flows: []
  scope: email
- description: Full access to the Shopify Customer Account API for the signed-in buyer.
  flows: []
  scope: customer-account-api:full
- description: Full access to the Customer Account MCP API — the authenticated agent surface for a signed-in buyer's account (orders, addresses, payment methods).
  flows: []
  scope: customer-account-mcp-api:full
slug: evolved-by-nature-scopes
source_filename: evolved-by-nature-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://skincare.evolvedbynature.com/.well-known/oauth-authorization-server and\n  https://bioactives.evolvedbynature.com/.well-known/oauth-authorization-server (HTTP 200, 2026-08-12)\nname: Evolved By Nature — OAuth scopes\ndescription: >-\n  Scopes advertised by the Shopify Customer Accounts authorization servers named from Evolved By\n  Nature's two storefront hosts. Identical on both storefronts. Evolved By Nature publishes no scope\n  reference of its own.\nissuers:\n- https://shopify.com/authentication/62086119623\n- https://shopify.com/authentication/65777369280\nscopes:\n- name: openid\n  description: OpenID Connect authentication; issues an ID token identifying the buyer.\n  standard: true\n- name: email\n  description: Access to the buyer's email address claim.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n  standard:\
  \ false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API — the authenticated agent surface for a signed-in\n    buyer's account (orders, addresses, payment methods).\n  standard: false\nscope_count: 4\nnotes:\n- Scope names are Shopify-defined; the shop-scoped issuers are Evolved By Nature's.\n- The anonymous UCP/MCP commerce endpoints require no scope for discovery, catalog search or cart\n  creation. Checkout completion requires buyer approval.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolved-by-nature/refs/heads/main/scopes/evolved-by-nature-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Biotechnology
- Materials Science
- Sustainability
- Personal Care
- Cosmetics
- Specialty Chemicals
- Textiles
- E-Commerce
- Agentic Commerce
- MCP
- Universal Commerce Protocol
token_bound: false
token_urls: []
---
