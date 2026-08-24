---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Johnnie O Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the scopes_supported array of the OIDC discovery document served on Johnnie-O's own primary domain. This is Shopify's customer-accounts scope set for merchant tenant 22750137 — Johnnie-O publishes no scope reference page of its own, and no additional scopes were found anywhere on its site. Recorded exactly as advertised; nothing inferred.
overview: 'Johnnie-O uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Johnnie-O
provider_slug: johnnie-o
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: johnnie-o-scopes
source_filename: johnnie-o-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://checkout.johnnie-o.com/.well-known/openid-configuration\nnote: >-\n  Read verbatim from the scopes_supported array of the OIDC discovery document served on\n  Johnnie-O's own primary domain. This is Shopify's customer-accounts scope set for merchant\n  tenant 22750137 — Johnnie-O publishes no scope reference page of its own, and no additional\n  scopes were found anywhere on its site. Recorded exactly as advertised; nothing inferred.\nflow: authorization_code\npkce: S256\nissuer: https://shopify.com/authentication/22750137\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope — requests an ID token identifying the customer.\n- name: email\n  description: Releases the customer's email and email_verified claims.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API for the signed-in customer of\n    this store — orders, addresses, profile.\n- name: customer-account-mcp-api:full\n\
  \  description: Full access to the Customer Account MCP API for the signed-in customer, the\n    agent-facing projection of the same customer data.\nscope_count: 4\ndocs: null\ndocs_note: Johnnie-O publishes no OAuth scope reference; the discovery document is the only\n  published source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnnie-o/refs/heads/main/scopes/johnnie-o-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Apparel
- Retail
- E-Commerce
- Direct to Consumer
- Golf
- Fashion
- Consumer Goods
- Shopify
- Agentic Commerce
token_urls: []
---
