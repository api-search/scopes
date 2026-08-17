---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Atolls Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from the `scopes_supported` array of the published OIDC discovery documents on the Pepper community hosts. There is no OpenAPI with oauth2 securitySchemes to derive from, and Atolls publishes no scopes/permissions reference page, so descriptions below are the standard OpenID Connect Core 1.0 definitions — marked as such — not text Atolls wrote.
overview: 'Atolls uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Atolls
provider_slug: atolls
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: atolls-scopes
source_filename: atolls-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.mydealz.de/.well-known/openid-configuration\nnote: >-\n  Scopes are taken verbatim from the `scopes_supported` array of the published OIDC\n  discovery documents on the Pepper community hosts. There is no OpenAPI with oauth2\n  securitySchemes to derive from, and Atolls publishes no scopes/permissions reference\n  page, so descriptions below are the standard OpenID Connect Core 1.0 definitions —\n  marked as such — not text Atolls wrote.\ndocs: null\nflows:\n- type: authorization_code\n- type: client_credentials\n- type: refresh_token\nissuers:\n- https://www.mydealz.de\n- https://www.hotukdeals.com\n- https://www.dealabs.com\n- https://www.preisjaeger.at\n- https://www.chollometro.com\n- https://www.pepper.pl\n- https://www.promodescuentos.com\nscope_count: 3\nscopes:\n- name: openid\n  description: Required to make the request an OpenID Connect request and receive an ID token.\n  description_source: OpenID Connect\
  \ Core 1.0 (standard definition — Atolls publishes none)\n- name: profile\n  description: Requests access to the end user's default profile claims.\n  description_source: OpenID Connect Core 1.0 (standard definition — Atolls publishes none)\n- name: email\n  description: Requests access to the email and email_verified claims.\n  description_source: OpenID Connect Core 1.0 (standard definition — Atolls publishes none)\ngaps:\n- >-\n    Only the three baseline OIDC scopes are advertised. No product/resource scopes\n    (deals, threads, cashback, vouchers, user activity) are published, so the discovery\n    document describes identity only — nothing about what an access token may read or\n    write on the Pepper platform.\n- No scopes or permissions reference page exists to enrich these descriptions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atolls/refs/heads/main/scopes/atolls-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- E-Commerce
- Affiliate Marketing
- Cashback
- Coupons
- Shopping
- Retail
- Identity
- OpenID Connect
token_urls: []
---
