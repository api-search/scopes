---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Poppi Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from scopes_supported in the store's OIDC discovery document. This is the Shopify Customer Accounts scope set for poppi's own authentication tenant (issuer https://shopify.com/authentication/22399731). poppi publishes no scope reference page of its own and the UCP MCP endpoint at /api/ucp/mcp is anonymous, so no scopes apply there.
overview: 'Poppi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Poppi
provider_slug: poppi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: poppi-scopes
source_filename: poppi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://drinkpoppi.com/.well-known/openid-configuration\nnote: >-\n  Scopes are read verbatim from scopes_supported in the store's OIDC discovery document. This is the\n  Shopify Customer Accounts scope set for poppi's own authentication tenant (issuer\n  https://shopify.com/authentication/22399731). poppi publishes no scope reference page of its own and the\n  UCP MCP endpoint at /api/ucp/mcp is anonymous, so no scopes apply there.\nauthorization_server: https://shopify.com/authentication/22399731\nscope_count: 4\nscopes:\n- name: openid\n  description: OpenID Connect — request an ID token for the signed-in customer.\n- name: email\n  description: Release the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the Customer Account API on behalf of the signed-in customer.\n- name: customer-account-mcp-api:full\n  description: Full access to the Customer Account\
  \ MCP API on behalf of the signed-in customer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppi/refs/heads/main/scopes/poppi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer Packaged Goods
- Beverages
- Food and Beverage
- E-Commerce
- Direct to Consumer
- Retail
- Agentic Commerce
- Shopify
- MCP
token_urls: []
---
