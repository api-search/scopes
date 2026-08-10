---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the authorization server behind the Athletic Brewing storefront, taken verbatim from the scopes_supported array of the discovery document the store serves at its own domain. Athletic Brewing publishes no scope reference page of its own; these four values are the complete published set.
docs: https://athleticbrewing.com/.well-known/oauth-authorization-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Athletic Brewing Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Athletic Brewing uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Athletic Brewing
provider_slug: athletic-brewing
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: athletic-brewing-scopes
source_filename: athletic-brewing-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://athleticbrewing.com/.well-known/openid-configuration\ndocs: https://athleticbrewing.com/.well-known/oauth-authorization-server\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the authorization server behind the\n  Athletic Brewing storefront, taken verbatim from the scopes_supported array of the\n  discovery document the store serves at its own domain. Athletic Brewing publishes no\n  scope reference page of its own; these four values are the complete published set.\nissuer: https://shopify.com/authentication/7931756625\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; requests an ID token for the signed-in customer.\n  standard: true\n- name: email\n  description: Releases the email and email_verified claims for the signed-in customer.\n  standard: true\n- name: customer-account-api:full\n  description: >-\n    Full access to the Shopify Customer Account API on\
  \ behalf of the signed-in buyer —\n    orders, addresses, payment methods and profile for that customer only.\n  standard: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP API on behalf of the signed-in buyer. This is\n    the scope that lets an agent act on a buyer's authenticated account through MCP rather\n    than only browsing the anonymous catalog.\n  standard: false\nnotes:\n- No granular read/write split is published; both non-standard scopes are \":full\".\n- PKCE S256 is required; see authentication/athletic-brewing-authentication.yml.\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - url: https://athleticbrewing.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletic-brewing/refs/heads/main/scopes/athletic-brewing-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Non-Alcoholic Beer
- Beverage
- Consumer Packaged Goods
- Direct to Consumer
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
token_urls: []
---
