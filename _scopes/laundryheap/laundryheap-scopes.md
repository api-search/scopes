---
authorization_urls: []
description: 'The complete OAuth 2.0 scope surface Laundryheap''s authorization server advertises. There are two scopes and no published scope reference page: this list is the authorization server''s own machine-readable declaration, which is the only place either scope is named anywhere on Laundryheap''s public surface.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Laundryheap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Laundryheap uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Laundryheap
provider_slug: laundryheap
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: laundryheap-scopes
source_filename: laundryheap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://www.laundryheap.com/.well-known/openid-configuration — scopes_supported,\n  fetched live 2026-08-23 (HTTP 200).\ndescription: >-\n  The complete OAuth 2.0 scope surface Laundryheap's authorization server\n  advertises. There are two scopes and no published scope reference page: this\n  list is the authorization server's own machine-readable declaration, which is\n  the only place either scope is named anywhere on Laundryheap's public surface.\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page exists. Searched the website, the help\n  centre (help.laundryheap.com) and the partner/hotel pages; none mention OAuth,\n  scopes, API access or client credentials.\n\nauthorization_server: https://www.laundryheap.com\nauthorization_url: https://www.laundryheap.com/oauth/authorize\ntoken_url: https://www.laundryheap.com/oauth/token\ngrant_types: [authorization_code, client_credentials]\n\nscope_count: 2\nscopes:\n\
  \  - name: openid\n    description: >-\n      Standard OpenID Connect scope. Requests an ID token (RS256) identifying the\n      end user; enables the /oauth/userinfo endpoint.\n    standard: true\n    spec: OpenID Connect Core 1.0\n  - name: orders.create\n    description: >-\n      Create orders on behalf of the account. Laundryheap's only business scope.\n      Its dotted resource.action naming implies a wider intended scheme\n      (orders.read, orders.cancel and so on) of which only this one is currently\n      advertised.\n    standard: false\n    resource: orders\n    action: create\n    write: true\n\nobservations:\n  - >-\n    The scope set is write-only in business terms: a partner can create an order\n    but the authorization server advertises no scope for reading, modifying or\n    cancelling one. Every read and every cancellation observed on the GraphQL\n    surface is gated behind the first-party session instead.\n  - >-\n    Dynamic client registration (RFC 7591) is open\
  \ at /oauth/registration, so\n    scopes can be requested by a self-registered client.\n\nx-evidence:\n  fetched: '2026-08-23'\n  url: https://www.laundryheap.com/.well-known/openid-configuration\n  http_status: 200\n  scopes_supported: [openid, orders.create]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laundryheap/refs/heads/main/scopes/laundryheap-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Laundry
- Dry Cleaning
- On-Demand Services
- Logistics
- Last Mile Delivery
- Consumer Services
- Hospitality
- Ordering
- GraphQL
- Authentication
token_urls: []
---
