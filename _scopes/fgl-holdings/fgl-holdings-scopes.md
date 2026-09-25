---
authorization_urls: []
description: Scopes advertised by the F&G Annuities & Life authorization server (auth.fglife.com). These are the OpenID Connect standard and profile-claim scopes the tenant exposes in scopes_supported — read verbatim from the anonymous discovery document. F&G publishes no product API, so there are NO resource/permission scopes of the kind a developer would request against a business API; the list below governs identity and profile claims for portal sign-in only.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Fgl Holdings Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FGL Holdings uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FGL Holdings
provider_slug: fgl-holdings
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fgl-holdings-scopes
source_filename: fgl-holdings-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://auth.fglife.com/.well-known/openid-configuration\nprovider: FGL Holdings\nproviderId: fgl-holdings\ndescription: >-\n  Scopes advertised by the F&G Annuities & Life authorization server (auth.fglife.com). These are the\n  OpenID Connect standard and profile-claim scopes the tenant exposes in scopes_supported — read\n  verbatim from the anonymous discovery document. F&G publishes no product API, so there are NO\n  resource/permission scopes of the kind a developer would request against a business API; the list\n  below governs identity and profile claims for portal sign-in only.\nnotes: >-\n  No scopes/permissions reference page exists on any F&G property — searched www.fglife.com (full\n  sitemap, 88 URLs) and found no developer section. Scope descriptions below are the OIDC Core 1.0 /\n  Auth0 standard meanings for these names, not F&G prose; F&G publishes no per-scope documentation.\nauthorization_server: https://auth.fglife.com/\n\
  observed_request:\n  source: https://saleslink.fglife.com/ (HTTP 302 Location)\n  scope: offline_access openid profile email\nscopes:\n  - name: openid\n    description: Required to obtain an ID token; signals an OpenID Connect authentication request.\n    standard: OIDC Core 1.0\n  - name: profile\n    description: Requests the default profile claims (name, family_name, given_name, nickname, picture, updated_at).\n    standard: OIDC Core 1.0\n  - name: email\n    description: Requests the email and email_verified claims.\n    standard: OIDC Core 1.0\n  - name: address\n    description: Requests the address claim.\n    standard: OIDC Core 1.0\n  - name: phone\n    description: Requests the phone_number and phone_number_verified claims.\n    standard: OIDC Core 1.0\n  - name: offline_access\n    description: Requests a refresh token so the portal session can be renewed without re-prompting.\n    standard: OIDC Core 1.0\n  - name: name\n    description: Individual profile claim scope exposed\
  \ by the Auth0 tenant.\n  - name: given_name\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: family_name\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: nickname\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: picture\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: email_verified\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: created_at\n    description: Individual profile claim scope exposed by the Auth0 tenant.\n  - name: identities\n    description: Individual profile claim scope exposed by the Auth0 tenant (linked identity providers).\nscope_count: 14\nresource_scopes_published: false\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fgl-holdings/refs/heads/main/scopes/fgl-holdings-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Annuities
- Financial Services
- Life Insurance
- Retirement
- Pension-Risk-Transfer
token_urls: []
---
