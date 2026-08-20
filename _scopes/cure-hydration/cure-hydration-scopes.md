---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cure Hydration Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cure Hydration uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cure Hydration
provider_slug: cure-hydration
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cure-hydration-scopes
source_filename: cure-hydration-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://www.curehydration.com/.well-known/openid-configuration\nsummary: >-\n  Four OAuth 2.0 / OpenID Connect scopes are advertised in the authorization-server metadata\n  served under Cure Hydration's own apex domain. They are the Shopify Customer Accounts\n  scope set for this store (shop id 7323713602). Cure publishes no scope reference page of\n  its own; the descriptions below are read from the OIDC/OAuth metadata plus Shopify's\n  platform documentation and are marked accordingly.\nissuer: https://shopify.com/authentication/7323713602\nauthorization_endpoint: https://shopify.com/authentication/7323713602/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/7323713602/oauth/token\nflows:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\npkce_required_methods: [S256]\ndocs: https://shopify.dev/docs/api/customer\nscope_count: 4\nscopes:\n  - name: openid\n    description:\
  \ Standard OpenID Connect scope. Requests an ID token identifying the signed-in shopper.\n    standard: true\n    source: openid-configuration scopes_supported\n  - name: email\n    description: Releases the shopper's email address and email_verified claim into the ID token.\n    standard: true\n    source: openid-configuration scopes_supported\n  - name: 'customer-account-api:full'\n    description: >-\n      Full access to the Shopify Customer Account API on behalf of the signed-in shopper —\n      orders, addresses, subscriptions, and profile.\n    standard: false\n    source: openid-configuration scopes_supported\n  - name: 'customer-account-mcp-api:full'\n    description: >-\n      Full access to the Shopify Customer Account MCP API — the authenticated, shopper-scoped\n      counterpart to the anonymous UCP commerce MCP server at /api/ucp/mcp. This is the scope\n      an agent needs to read a specific buyer's orders rather than the public catalog.\n    standard: false\n    source:\
  \ openid-configuration scopes_supported\nnotes:\n  - >-\n    These scopes govern shopper identity, not developer access. There is no partner, admin,\n    or integrator scope surface published for this store.\n  - >-\n    The presence of customer-account-mcp-api:full is the notable finding: the store advertises\n    an authenticated, per-buyer MCP surface alongside the anonymous commerce one.\nx-evidence:\n  - fetched: '2026-08-11'\n    url: https://www.curehydration.com/.well-known/openid-configuration\n    http_status: 200\n  - fetched: '2026-08-11'\n    url: https://www.curehydration.com/.well-known/oauth-authorization-server\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cure-hydration/refs/heads/main/scopes/cure-hydration-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer Packaged Goods
- Beverages
- Health and Wellness
- E-Commerce
- Direct to Consumer
- Retail
- Shopify
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- GraphQL
token_urls: []
---
