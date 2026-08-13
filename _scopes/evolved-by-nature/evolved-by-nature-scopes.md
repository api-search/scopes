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
overview: 'Evolved By Nature uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evolved By Nature
provider_slug: evolved-by-nature
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: evolved-by-nature-scopes
source_filename: evolved-by-nature-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://skincare.evolvedbynature.com/.well-known/oauth-authorization-server and\n  https://bioactives.evolvedbynature.com/.well-known/oauth-authorization-server (HTTP 200, 2026-08-12)\nname: Evolved By Nature — OAuth scopes\ndescription: >-\n  Scopes advertised by the Shopify Customer Accounts authorization servers named from Evolved By\n  Nature's two storefront hosts. Identical on both storefronts. Evolved By Nature publishes no scope\n  reference of its own.\nissuers:\n- https://shopify.com/authentication/62086119623\n- https://shopify.com/authentication/65777369280\nscopes:\n- name: openid\n  description: OpenID Connect authentication; issues an ID token identifying the buyer.\n  standard: true\n- name: email\n  description: Access to the buyer's email address claim.\n  standard: true\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in buyer.\n  standard:\
  \ false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API — the authenticated agent surface for a signed-in\n    buyer's account (orders, addresses, payment methods).\n  standard: false\nscope_count: 4\nnotes:\n- Scope names are Shopify-defined; the shop-scoped issuers are Evolved By Nature's.\n- The anonymous UCP/MCP commerce endpoints require no scope for discovery, catalog search or cart\n  creation. Checkout completion requires buyer approval.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolved-by-nature/refs/heads/main/scopes/evolved-by-nature-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Materials Science
- Sustainability
- Personal Care
- Cosmetics
- Specialty Chemicals
- Textiles
- eCommerce
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
token_urls: []
---
