---
authorization_urls: []
description: The complete set of OAuth 2.0 scopes EatStreet advertises, read verbatim from the scopes_supported array of its RFC 8414 Authorization Server Metadata document. EatStreet publishes no scope reference page — the developer portal is gone — so no description text is available for any scope and none has been invented here. The names are the entire published record.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Eatstreet Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EatStreet uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EatStreet
provider_slug: eatstreet
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: eatstreet-scopes
source_filename: eatstreet-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://eatstreet.com/.well-known/oauth-authorization-server\nname: EatStreet OAuth scopes\ndescription: >-\n  The complete set of OAuth 2.0 scopes EatStreet advertises, read verbatim from\n  the scopes_supported array of its RFC 8414 Authorization Server Metadata\n  document. EatStreet publishes no scope reference page — the developer portal\n  is gone — so no description text is available for any scope and none has been\n  invented here. The names are the entire published record.\nauthorization_server: https://eatstreet.com\nscope_count: 3\nscopes:\n- name: merchant_integration\n  description: null\n  note: >-\n    Name implies the restaurant/merchant-side integration surface (menus,\n    orders inbound to a merchant). No published definition exists.\n- name: customer\n  description: null\n  note: >-\n    Name implies the consumer-side surface (accounts, addresses, order\n    placement and tracking). No published definition\
  \ exists.\n- name: example\n  description: null\n  note: >-\n    Advertised in scopes_supported alongside the two real scopes. Reads as a\n    placeholder or sample scope left in production metadata rather than a\n    functional grant.\ngaps:\n- No scope reference page is published; scopes_supported carries names only.\n- No per-scope operation mapping is possible — EatStreet publishes no OpenAPI.\ndocs: null\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://eatstreet.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eatstreet/refs/heads/main/scopes/eatstreet-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Food Delivery
- Restaurant
- Online Ordering
- Marketplace
- Local Commerce
- Consumer
- Point-of-Sale
- Authentication
token_urls: []
---
