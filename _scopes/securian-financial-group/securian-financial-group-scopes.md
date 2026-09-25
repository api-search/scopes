---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Securian Financial Group Scopes
name_suffix: OAuth Scopes
note: scopes_supported read verbatim from Securian's published OpenID Connect discovery document. There is no public scopes/permissions reference page to enrich these with — the descriptions below for the four standard OIDC scopes are the OpenID Connect Core 1.0 definitions; the two non-standard scopes (edit, admin) are advertised by the server with no published description, and are recorded here without one rather than guessed at.
overview: 'Securian Financial Group uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Securian Financial Group
provider_slug: securian-financial-group
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: securian-financial-group-scopes
source_filename: securian-financial-group-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://sso.securian.com/.well-known/openid-configuration\nnote: >-\n  scopes_supported read verbatim from Securian's published OpenID Connect discovery\n  document. There is no public scopes/permissions reference page to enrich these with —\n  the descriptions below for the four standard OIDC scopes are the OpenID Connect Core 1.0\n  definitions; the two non-standard scopes (edit, admin) are advertised by the server with\n  no published description, and are recorded here without one rather than guessed at.\nissuer: https://sso.securian.com\nauthorization_endpoint: https://sso.securian.com/as/authorization.oauth2\ntoken_endpoint: https://sso.securian.com/as/token.oauth2\ndocs: null\nscope_count: 7\nscopes:\n  - name: openid\n    standard: OpenID Connect Core 1.0\n    description: Required to obtain an ID Token; signals an OpenID Connect authentication request.\n  - name: profile\n    standard: OpenID Connect Core 1.0\n    description:\
  \ Default profile claims (name, family_name, given_name, picture, locale, updated_at, ...).\n  - name: email\n    standard: OpenID Connect Core 1.0\n    description: The email and email_verified claims.\n  - name: address\n    standard: OpenID Connect Core 1.0\n    description: The address claim.\n  - name: phone\n    standard: OpenID Connect Core 1.0\n    description: The phone_number and phone_number_verified claims.\n  - name: edit\n    standard: null\n    description: null\n    note: Provider-specific scope advertised by the authorization server; no published definition.\n  - name: admin\n    standard: null\n    description: null\n    note: Provider-specific scope advertised by the authorization server; no published definition.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securian-financial-group/refs/heads/main/scopes/securian-financial-group-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fortune 1000
- Financial Services
- Insurance
- Life Insurance
- Annuities
- Retirement
- Group Benefits
- Employee Benefits
token_urls: []
---
