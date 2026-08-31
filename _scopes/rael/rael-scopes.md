---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rael Scopes
name_suffix: OAuth Scopes
note: These four scopes are the scopes_supported list published by the Shopify Customer Accounts authorization server discovered on Rael's own domain. They govern shopper sign-in to Rael's store, not a developer API. Rael publishes no scope reference page of its own; the descriptions below are read from the scope names and the OIDC document's own claims_supported list, and are marked derived where the provider states nothing.
overview: 'Rael uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rael
provider_slug: rael
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rael-scopes
source_filename: rael-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.getrael.com/.well-known/openid-configuration\nname: Rael OAuth / OIDC scopes\ndocs: null\nnote: >-\n  These four scopes are the scopes_supported list published by the Shopify Customer Accounts\n  authorization server discovered on Rael's own domain. They govern shopper sign-in to Rael's\n  store, not a developer API. Rael publishes no scope reference page of its own; the descriptions\n  below are read from the scope names and the OIDC document's own claims_supported list, and are\n  marked derived where the provider states nothing.\nissuer: https://shopify.com/authentication/22463213\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an id_token identifying the signed-in shopper.\n  source: scopes_supported\n- name: email\n  description: Releases the email and email_verified claims (both listed in claims_supported).\n  source: scopes_supported\n- name: 'customer-account-api:full'\n\
  \  description: Full access to the signed-in shopper's own customer account data (orders, addresses, subscriptions).\n  source: scopes_supported\n  description_method: derived\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the customer-account MCP API on behalf of the signed-in shopper. Notable\n    separately from the anonymous storefront commerce MCP endpoint at /api/ucp/mcp — this scope\n    is the authenticated, account-scoped agent surface.\n  source: scopes_supported\n  description_method: derived\ncode_challenge_methods_supported: [S256]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rael/refs/heads/main/scopes/rael-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Retail
- E-Commerce
- Consumer Goods
- Health and Wellness
- Personal Care
- Agentic Commerce
- MCP
- Universal Commerce Protocol
- Shopify
token_urls: []
---
