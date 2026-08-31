---
authorization_urls: []
description: Scopes advertised by the A-Mark Trading Portal's OAuth 2.0 / OIDC discovery document. These are the standard OIDC scope set as emitted by the portal's identity server; A-Mark publishes no scope reference page and no product-specific scopes (no trading, pricing, order or inventory scopes are advertised). Descriptions below are the RFC/OIDC-standard meanings of each scope name, not A-Mark prose — the provider documents none.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: A Mark Precious Metals Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'A-Mark Precious Metals uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: A-Mark Precious Metals
provider_slug: a-mark-precious-metals
schemes:
- name: OAuth2
  source: https://portal.amark.com/.well-known/openid-configuration
  token_url: https://portal.amark.com/connect/token
scope_count: 0
scope_names: []
scopes: []
slug: a-mark-precious-metals-scopes
source_filename: a-mark-precious-metals-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://portal.amark.com/.well-known/openid-configuration\nprovider: A-Mark Precious Metals\nproviderId: a-mark-precious-metals\ndescription: >-\n  Scopes advertised by the A-Mark Trading Portal's OAuth 2.0 / OIDC discovery document.\n  These are the standard OIDC scope set as emitted by the portal's identity server; A-Mark\n  publishes no scope reference page and no product-specific scopes (no trading, pricing,\n  order or inventory scopes are advertised). Descriptions below are the RFC/OIDC-standard\n  meanings of each scope name, not A-Mark prose — the provider documents none.\ndocs: null\ndocs_note: No public scopes/permissions reference page exists on amark.com or gold.com.\nschemes:\n  - name: OAuth2\n    token_url: https://portal.amark.com/connect/token\n    source: https://portal.amark.com/.well-known/openid-configuration\nscope_count: 6\nscopes:\n  - name: openid\n    standard: OpenID Connect Core 1.0\n    description:\
  \ Requests an OpenID Connect authentication response.\n  - name: email\n    standard: OpenID Connect Core 1.0\n    description: Requests the email and email_verified claims.\n  - name: phone\n    standard: OpenID Connect Core 1.0\n    description: Requests the phone_number and phone_number_verified claims.\n  - name: profile\n    standard: OpenID Connect Core 1.0\n    description: Requests the default profile claims.\n  - name: offline_access\n    standard: OpenID Connect Core 1.0\n    description: Requests a refresh token so the client can act without the user present.\n  - name: roles\n    standard: non-standard (identity-server convention)\n    description: >-\n      Requests the caller's portal role assignments. A-Mark does not document what roles\n      exist or what each one authorizes.\nx-evidence:\n  - url: https://portal.amark.com/.well-known/openid-configuration\n    http_status: 200\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/a-mark-precious-metals/refs/heads/main/scopes/a-mark-precious-metals-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Precious Metals
- Trading
- Wholesale
- Gold
- Silver
- Bullion
- Finance
token_urls: []
---
