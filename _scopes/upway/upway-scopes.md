---
authorization_urls: []
description: Scopes advertised by the OpenID Connect / OAuth 2.0 discovery documents served from upway.co for the store's customer-account identity provider. Read from the live discovery document, not from prose. The UCP MCP commerce endpoint itself is anonymous and consumes none of these scopes.
docs: https://upway.co/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Upway Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Upway uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Upway
provider_slug: upway
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: upway-scopes
source_filename: upway-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://upway.co/.well-known/openid-configuration\nname: Upway OAuth Scopes\ndescription: >-\n  Scopes advertised by the OpenID Connect / OAuth 2.0 discovery documents served from\n  upway.co for the store's customer-account identity provider. Read from the live\n  discovery document, not from prose. The UCP MCP commerce endpoint itself is anonymous\n  and consumes none of these scopes.\ndocs: https://upway.co/.well-known/openid-configuration\nissuer: https://shopify.com/authentication/65864040675\nauthorization_endpoint: https://shopify.com/authentication/65864040675/oauth/authorize\ntoken_endpoint: https://shopify.com/authentication/65864040675/oauth/token\njwks_uri: https://shopify.com/authentication/65864040675/.well-known/jwks.json\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- 'urn:ietf:params:oauth:grant-type:jwt-bearer'\ncode_challenge_methods_supported:\n- S256\nscope_count: 4\nscopes:\n- name: openid\n\
  \  description: Issue an ID token identifying the signed-in customer.\n  standard: true\n- name: email\n  description: Release the customer's email address and the email_verified claim.\n  standard: true\n- name: 'customer-account-api:full'\n  description: Full access to the Shopify Customer Account API for this shop (orders, addresses, profile).\n  standard: false\n- name: 'customer-account-mcp-api:full'\n  description: >-\n    Full access to the authenticated customer-account MCP API for this shop - the\n    signed-in counterpart to the anonymous storefront UCP MCP endpoint.\n  standard: false\nclaims_supported:\n- iss\n- sub\n- aud\n- exp\n- iat\n- nonce\n- sid\n- email\n- email_verified\nx-evidence:\n  fetched: '2026-09-02'\n  url: https://upway.co/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upway/refs/heads/main/scopes/upway-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- E-Commerce
- Retail
- Marketplace
- Agentic Commerce
- Model Context Protocol
- Universal Commerce Protocol
- Electric Bikes
- Micromobility
- Circular Economy
- Refurbished Goods
- Shopping Agents
token_urls: []
---
