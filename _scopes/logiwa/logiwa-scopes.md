---
authorization_urls: []
description: The Logiwa API gateway advertises three OAuth scopes in its anonymously-served OIDC discovery document. NONE of them is documented anywhere in the Logiwa developer reference, and the only documented authentication flow — the password grant against /token — does not take a scope parameter. Authorization on the Integration API is carried by the provisioned user's Roles, Warehouses and Clients, not by token scopes.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Logiwa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Logiwa uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Logiwa
provider_slug: logiwa
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: logiwa-scopes
source_filename: logiwa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://appapi.logiwa.com/.well-known/openid-configuration\nname: Logiwa OAuth scopes\ndescription: >-\n  The Logiwa API gateway advertises three OAuth scopes in its anonymously-served OIDC discovery\n  document. NONE of them is documented anywhere in the Logiwa developer reference, and the only\n  documented authentication flow — the password grant against /token — does not take a scope\n  parameter. Authorization on the Integration API is carried by the provisioned user's Roles,\n  Warehouses and Clients, not by token scopes.\nscope_count: 3\nscopes:\n- name: admin\n  description: null\n  documented_by_provider: false\n  note: >-\n    Advertised in scopes_supported. No description, no grant path and no reference page exists\n    for it in the public documentation. Description is left null rather than guessed.\n- name: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  documented_by_provider: false\n\
  - name: offline_access\n  description: Standard OAuth 2.0 scope requesting a refresh token.\n  documented_by_provider: false\n  note: Appears twice in the served scopes_supported array — a duplicate in Logiwa's own document.\ndocumented_authorization_model: >-\n  \"The data this API user can access is based on the permissions given to them in Logiwa, such as\n  the Roles, Warehouses, and Clients they're affiliated with.\"\n  — https://developer.logiwa.com/?id=5df0da39e6466c2eec992f3f\nfindings:\n- id: scopes-not-documented\n  severity: medium\n  detail: >-\n    The gateway advertises an \"admin\" scope with no published definition and no documented way to\n    request it. An integrator has no way to know what it grants or to scope a credential down.\n- id: no-least-privilege-path\n  severity: medium\n  detail: >-\n    Because the documented flow is a password grant with no scope parameter, every integration\n    token carries the full permission set of the human user account behind it.\
  \ There is no\n    published way to issue a read-only or warehouse-limited API credential.\nx-evidence:\n  fetched: '2026-08-25'\n  probes:\n  - url: https://appapi.logiwa.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://wmsapi.logiwa.com/.well-known/openid-configuration\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logiwa/refs/heads/main/scopes/logiwa-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Warehouse Management
- Fulfillment
- Logistics
- Supply Chain
- Inventory Management
- Order Management
- Third Party Logistics
- Ecommerce
- Shipping
- Webhooks
- SaaS
token_urls: []
---
