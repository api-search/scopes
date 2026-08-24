---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Globacap Scopes
name_suffix: OAuth Scopes
note: These are the scopes the Globacap identity provider advertises in its anonymous OpenID Connect discovery document. They are the standard OIDC scope set — Globacap publishes no API-specific or product-specific permission reference, and no scopes/permissions documentation page exists to enrich this from. Do not read this as an API authorization model; it is the login surface only.
overview: 'Globacap uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Globacap
provider_slug: globacap
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: globacap-scopes
source_filename: globacap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://login.globacap.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes the Globacap identity provider advertises in its anonymous\n  OpenID Connect discovery document. They are the standard OIDC scope set — Globacap\n  publishes no API-specific or product-specific permission reference, and no\n  scopes/permissions documentation page exists to enrich this from. Do not read this\n  as an API authorization model; it is the login surface only.\nissuer: https://login.globacap.com\nflows:\n- type: authorization_code\n  authorization_url: https://login.globacap.com/oauth2/auth\n  token_url: https://login.globacap.com/oauth2/token\n  pkce_required_methods:\n  - S256\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token.\n  standard: true\n- name: profile\n  description: Standard OIDC scope for basic profile claims.\n  standard: true\n- name: email\n  description: Standard\
  \ OIDC scope for the email claim.\n  standard: true\n- name: phone\n  description: Standard OIDC scope for the phone_number claim.\n  standard: true\n- name: address\n  description: Standard OIDC scope for the address claim.\n  standard: true\n- name: offline\n  description: Requests a refresh token for offline access.\n  standard: true\nscope_count: 6\nproduct_specific_scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globacap/refs/heads/main/scopes/globacap-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Private Capital Markets
- Capital Markets
- Securities
- Financial Services
- Fintech
- Tokenization
- Share Register
- Secondary Markets
- United Kingdom
token_urls: []
---
