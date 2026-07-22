---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised for authenticated buyer and agent access to Winc's Shopify Customer Account API, taken verbatim from the store's OpenID Connect discovery document (scopes_supported).
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Winc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Winc uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Winc
provider_slug: winc
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: winc-scopes
source_filename: winc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://winc.com/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nname: Winc OAuth Scopes\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised for authenticated buyer and agent access to\n  Winc's Shopify Customer Account API, taken verbatim from the store's OpenID Connect\n  discovery document (scopes_supported).\nprovider: Shopify Customer Account API\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; issues an ID token identifying the buyer.\n- name: email\n  description: Grants access to the buyer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: Full access to the Shopify Customer Account API (orders, addresses, profile) for the authenticated buyer.\n- name: customer-account-mcp-api:full\n  description: Full access to the customer-account MCP API surface, enabling agent-driven authenticated account actions over MCP.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/winc/refs/heads/main/scopes/winc-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Wine
- Ecommerce
- Retail
- Subscription
- Agentic Commerce
- MCP
- Shopify
- UCP
token_urls: []
---
