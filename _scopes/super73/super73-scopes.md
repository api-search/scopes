---
authorization_urls: []
description: ''
docs: https://shopify.dev/docs/api/customer
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Super73 Scopes
name_suffix: OAuth Scopes
note: These are the scopes the SUPER73 storefront's own OpenID Connect discovery document advertises as supported. They are Shopify customer-account scopes served per-merchant; SUPER73 publishes no scope reference page of its own, so descriptions below are read from the scope names and Shopify's customer account documentation, not invented.
overview: 'Super73 uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Super73
provider_slug: super73
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: super73-scopes
source_filename: super73-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://super73.com/.well-known/openid-configuration (HTTP 200, 2026-08-29)\ndocs: https://shopify.dev/docs/api/customer\nissuer: https://shopify.com/authentication/13743231\nnote: >-\n  These are the scopes the SUPER73 storefront's own OpenID Connect discovery document advertises as\n  supported. They are Shopify customer-account scopes served per-merchant; SUPER73 publishes no scope\n  reference page of its own, so descriptions below are read from the scope names and Shopify's customer\n  account documentation, not invented.\nscopes:\n- name: openid\n  description: Standard OpenID Connect scope; returns an ID token identifying the signed-in buyer.\n  standard: true\n- name: email\n  description: Standard OIDC scope releasing the buyer's email address claim.\n  standard: true\n- name: customer-account-api:full\n  description: >-\n    Full access to the buyer's Shopify Customer Account API surface — profile, addresses, orders\
  \ and\n    subscriptions for that customer.\n  standard: false\n- name: customer-account-mcp-api:full\n  description: >-\n    Full access to the customer-account MCP surface, the authenticated counterpart of the anonymous\n    UCP commerce endpoint at /api/ucp/mcp.\n  standard: false\nscope_count: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super73/refs/heads/main/scopes/super73-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electric Bikes
- Micromobility
- E-Commerce
- Agentic Commerce
- Consumer Hardware
- Model Context Protocol
- Universal Commerce Protocol
- Shopify
- Direct to Consumer
- Internet of Things
- Transportation
token_urls: []
---
