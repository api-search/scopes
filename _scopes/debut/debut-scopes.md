---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Debut Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Debut uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Debut
provider_slug: debut
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: debut-scopes
source_filename: debut-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://www.deinde.com/.well-known/oauth-authorization-server\n\napi: DEINDE Commerce (UCP MCP)\nissuer: https://shopify.com/authentication/75476861220\nauthorization_endpoint: https://account.deinde.com/authentication/oauth/authorize\ntoken_endpoint: https://account.deinde.com/authentication/oauth/token\ndocs: null\ndocs_note: >-\n  Debut publishes no scopes reference of its own. The scope list below is read verbatim\n  from scopes_supported in the authorization-server metadata the DEINDE store serves from\n  its own host; the semantics are Shopify customer-accounts semantics.\n\nscope_count: 4\nscopes:\n- name: openid\n  description: Request an ID token identifying the signed-in customer (OpenID Connect\n    core).\n  source: scopes_supported\n- name: email\n  description: Release the customer's email address and email_verified claim.\n  source: scopes_supported\n- name: customer-account-api:full\n  description: Full access\
  \ to the Shopify Customer Account API for the authenticated\n    customer — orders, addresses, profile and subscription data for that buyer.\n  source: scopes_supported\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP surface for the authenticated\n    customer, the buyer-scoped counterpart to the anonymous storefront UCP MCP endpoint.\n  source: scopes_supported\n\ngranularity: coarse\ngranularity_note: >-\n  Two of the four scopes are \":full\" grants. There is no read-only variant and no\n  per-resource decomposition, so an agent that needs to read a buyer's order history must\n  ask for full customer-account access. Scope design is Shopify's, not Debut's.\n\nprotected_resource:\n  metadata: https://www.deinde.com/.well-known/oauth-protected-resource\n  resource: https://www.deinde.com\n  authorization_servers:\n  - https://account.deinde.com\n  - https://shopify.com/authentication/75476861220\n  bearer_methods_supported:\n  - header\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/debut/refs/heads/main/scopes/debut-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Biotechnology
- Beauty
- Cosmetics
- Skincare
- Ingredients
- Synthetic Biology
- Artificial Intelligence
- Manufacturing
- Ecommerce
- Agentic Commerce
token_urls: []
---
