---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Rad Power Bikes Scopes
name_suffix: OAuth Scopes
note: Scopes are read verbatim from the store's own OpenID Connect discovery document (scopes_supported). Shopify Customer Accounts uses coarse full-access scopes rather than a granular per-resource scope catalog; there is no published scope reference page for this merchant because there is no public developer program.
overview: 'Rad Power Bikes uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rad Power Bikes
provider_slug: rad-power-bikes
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rad-power-bikes-scopes
source_filename: rad-power-bikes-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.radpowerbikes.com/.well-known/openid-configuration\nnote: >-\n  Scopes are read verbatim from the store's own OpenID Connect discovery document\n  (scopes_supported). Shopify Customer Accounts uses coarse full-access scopes rather than a\n  granular per-resource scope catalog; there is no published scope reference page for this\n  merchant because there is no public developer program.\nauthorization_server: https://shopify.com/authentication/7999645\nauthorization_endpoint: https://account.radpowerbikes.com/authentication/oauth/authorize\ntoken_endpoint: https://account.radpowerbikes.com/authentication/oauth/token\nflows:\n- authorization_code\n- refresh_token\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated customer.\n- name: email\n  description: Release the customer's email address and email_verified claim.\n- name: customer-account-api:full\n\
  \  description: Full access to the Shopify Customer Account API on behalf of the signed-in customer.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Shopify Customer Account MCP API on behalf of the signed-in customer\n    — the authenticated, buyer-scoped counterpart to the anonymous storefront UCP MCP\n    endpoint.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rad-power-bikes/refs/heads/main/scopes/rad-power-bikes-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Electric Bikes
- Micromobility
- E-Commerce
- Retail
- Consumer Products
- Agentic Commerce
- Shopify
- MCP
- Universal Commerce Protocol
token_urls: []
---
