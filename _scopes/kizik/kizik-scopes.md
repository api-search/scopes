---
authorization_urls: []
description: ''
docs: https://kizik.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kizik Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kizik uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kizik
provider_slug: kizik
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kizik-scopes
source_filename: kizik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://kizik.com/.well-known/openid-configuration\ndocs: https://kizik.com/.well-known/openid-configuration\nissuer: https://shopify.com/authentication/22811461\nflows:\n- type: authorization_code\n  pkce: S256\n  authorization_url: https://shopify.com/authentication/22811461/oauth/authorize\n  token_url: https://shopify.com/authentication/22811461/oauth/token\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope. Requests an ID token identifying the Kizik customer.\n- name: email\n  description: Releases the customer's email address and email_verified claim.\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API for this shop on behalf of the signed-in Kizik\n    customer — orders, addresses, and profile.\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the Customer Account MCP API for this shop. This is the authenticated,\
  \ customer-scoped\n    counterpart to the anonymous UCP commerce MCP endpoint at /api/ucp/mcp.\nnotes:\n- Scope names are read verbatim from the scopes_supported array of the served discovery document; none\n  were inferred.\n- The anonymous UCP/MCP commerce endpoint at https://kizik.com/api/ucp/mcp uses no OAuth scopes at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kizik/refs/heads/main/scopes/kizik-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Retail
- E-Commerce
- Footwear
- Consumer Goods
- Agent Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- Direct to Consumer
token_urls: []
---
