---
authorization_urls: []
description: The only OAuth scope surface MAKEUP BY MARIO exposes is the scopes_supported array of its per-merchant OpenID Connect discovery document, served from its own host. There is no scopes reference page, because there is no developer program to document one — these four values were read from the live discovery document, not from prose. The whole anonymous agent surface (GraphQL, Storefront MCP, UCP MCP) sits OUTSIDE this scope model and requires no token at all.
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Makeup By Mario Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Makeup by Mario uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Makeup by Mario
provider_slug: makeup-by-mario
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: makeup-by-mario-scopes
source_filename: makeup-by-mario-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://www.makeupbymario.com/.well-known/openid-configuration\ndescription: >-\n  The only OAuth scope surface MAKEUP BY MARIO exposes is the scopes_supported array of its\n  per-merchant OpenID Connect discovery document, served from its own host. There is no\n  scopes reference page, because there is no developer program to document one — these four\n  values were read from the live discovery document, not from prose. The whole anonymous\n  agent surface (GraphQL, Storefront MCP, UCP MCP) sits OUTSIDE this scope model and\n  requires no token at all.\nauthorization_server: https://shopify.com/authentication/27548221505\nissuer: https://shopify.com/authentication/27548221505\nauthorization_endpoint: https://shopify.com/authentication/27548221505/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/27548221505/oauth/token\nflows: [authorization_code]\npkce_required_methods: [S256]\nscope_count: 4\nscopes:\n- name:\
  \ openid\n  standard: OpenID Connect Core 1.0\n  description: Requests an id_token. Required to use the OIDC flow at all.\n  granularity: standard\n- name: email\n  standard: OpenID Connect Core 1.0\n  description: Releases the email and email_verified claims for the signed-in customer.\n  granularity: standard\n- name: customer-account-api:full\n  standard: Shopify Customer Account API\n  description: >-\n    Full read/write access to the signed-in customer's own account — orders, addresses,\n    saved payment methods, subscriptions.\n  granularity: coarse\n  note: >-\n    There is no read-only variant and no per-resource split. A customer authorizing an\n    application to see their order history necessarily also authorizes it to change their\n    addresses and payment methods. This is the notable weakness of the scope model here and\n    it is Shopify's design, not the merchant's.\n- name: customer-account-mcp-api:full\n  standard: Shopify Customer Account API (MCP)\n  description:\
  \ >-\n    Full access to the authenticated customer-account MCP surface — the agent-facing\n    projection of the same account data.\n  granularity: coarse\n  note: >-\n    Declared in discovery but not reachable anonymously, so its tool list could not be\n    probed. Its existence is the evidence that a THIRD MCP server exists on this store\n    beyond the two anonymous ones profiled in mcp/ — an authenticated one, scoped to a\n    signed-in customer.\ngaps:\n- No scopes documentation page exists on makeupbymario.com; there is no developer program.\n- No incremental or downscoped variants — both product scopes are ':full'.\n- >-\n  No /.well-known/oauth-protected-resource (RFC 9728), so an MCP client cannot discover\n  which authorization server protects the customer-account MCP endpoint by the standard\n  path.\ndocs: https://shopify.dev/docs/api/customer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makeup-by-mario/refs/heads/main/scopes/makeup-by-mario-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Beauty
- Cosmetics
- Consumer Packaged Goods
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- GraphQL
- MCP
- Universal Commerce Protocol
token_urls: []
---
