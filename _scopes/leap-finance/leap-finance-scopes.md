---
authorization_urls: []
description: The scopes advertised by Leap Finance Inc.'s Auth0 identity tenant. These are the standard OpenID Connect scopes and standard-claim scopes emitted by an Auth0 tenant with no custom API registered for public use — there is not a single Leap-Finance-specific or resource-specific scope among them.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Leap Finance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Leap Finance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leap Finance
provider_slug: leap-finance
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leap-finance-scopes
source_filename: leap-finance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: >-\n  scopes_supported from https://auth.leapfinance.com/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-08-25) — saved verbatim to\n  well-known/leap-finance-openid-configuration.json\nname: Leap Finance OAuth scopes\ndescription: >-\n  The scopes advertised by Leap Finance Inc.'s Auth0 identity tenant. These are the\n  standard OpenID Connect scopes and standard-claim scopes emitted by an Auth0 tenant\n  with no custom API registered for public use — there is not a single\n  Leap-Finance-specific or resource-specific scope among them.\n\ncaveat: >-\n  No scopes-and-permissions reference page exists on the company's site to enrich\n  this from; Leap Finance publishes no developer documentation of any kind. Every\n  entry below is read directly from the live discovery document, and descriptions are\n  the meanings defined by OpenID Connect Core 1.0 §5.4 / RFC 6749, not text the\n  provider wrote.\n\ndocs: null\ndocs_note:\
  \ >-\n  Searched leapfinance.com and leapscholar.com for a scopes, permissions or API\n  reference page. None exists — leapfinance.com/docs, /api-docs and /redoc all return\n  the site's soft-404 shell, and no docs.* or developer.* subdomain resolves for\n  either domain.\n\nauthorization_server: https://auth.leapfinance.com/\nscope_count: 14\ncustom_scopes: 0\n\nscopes:\n  - name: openid\n    standard: OpenID Connect Core 1.0\n    description: Requests an ID Token and identifies the request as an OIDC request.\n  - name: profile\n    standard: OpenID Connect Core 1.0\n    description: >-\n      Requests the default profile claims (name, family_name, given_name, nickname,\n      picture, updated_at and related).\n  - name: email\n    standard: OpenID Connect Core 1.0\n    description: Requests the email and email_verified claims.\n  - name: address\n    standard: OpenID Connect Core 1.0\n    description: Requests the address claim.\n  - name: phone\n    standard: OpenID Connect Core 1.0\n\
  \    description: Requests the phone_number and phone_number_verified claims.\n  - name: offline_access\n    standard: OpenID Connect Core 1.0\n    description: Requests a refresh token so the client can obtain tokens without the user present.\n  - name: name\n    standard: OIDC standard claim exposed as a scope by Auth0\n    description: Requests the name claim.\n  - name: given_name\n    standard: OIDC standard claim exposed as a scope by Auth0\n    description: Requests the given_name claim.\n  - name: family_name\n    standard: OIDC standard claim exposed as a scope by Auth0\n    description: Requests the family_name claim.\n  - name: nickname\n    standard: OIDC standard claim exposed as a scope by Auth0\n    description: Requests the nickname claim.\n  - name: email_verified\n    standard: OIDC standard claim exposed as a scope by Auth0\n    description: Requests the email_verified boolean claim.\n  - name: picture\n    standard: OIDC standard claim exposed as a scope by Auth0\n\
  \    description: Requests the picture claim.\n  - name: created_at\n    standard: Auth0 profile claim\n    description: Requests the account creation timestamp claim.\n  - name: identities\n    standard: Auth0 profile claim\n    description: >-\n      Requests the identities array describing linked identity-provider accounts.\n\nfindings:\n  resource_scopes: 0\n  note: >-\n    The absence of any resource-specific scope is itself the finding. A provider that\n    exposed a programmatic API through this tenant would register an Auth0 API and\n    advertise its permissions here. Leap Finance advertises only identity scopes,\n    which is consistent with the tenant existing solely to log borrowers and staff\n    into first-party web applications.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leap-finance/refs/heads/main/scopes/leap-finance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Financial-Services
- Lending
- Student Loans
- Education Finance
- Fintech
- Consumer Finance
- Study Abroad
- India
token_urls: []
---
