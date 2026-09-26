---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the GoGift authorization server. These were read from the live `scopes_supported` array in the provider's own OpenID Connect discovery document on both the production (auth.gogift.io) and sandbox (auth-pre.gogift.io) issuers — the two arrays are identical. GoGift publishes no scope-reference page in its API docs, so the descriptions below are the standard OIDC meanings where the scope is a standard one and are marked `undocumented` where GoGift defines the scope itself.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gogift Scopes
name_suffix: OAuth Scopes
note: The API reference at docs.gogift.io never names a scope. Which of AuthApi / finance_api / retail_api a given client is granted is decided by GoGift when it provisions the client id and secret. Treat the non-standard scopes below as observed-from-discovery, not as a provider-published permissions reference.
overview: 'GoGift uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: GoGift
provider_slug: gogift
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: gogift-scopes
source_filename: gogift-scopes.yml
source_heading: OAuth Scopes
source_url: https://auth.gogift.io/.well-known/openid-configuration
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://auth.gogift.io/.well-known/openid-configuration\nsources:\n  - https://auth.gogift.io/.well-known/openid-configuration\n  - https://auth-pre.gogift.io/.well-known/openid-configuration\n  - well-known/gogift-openid-configuration.json\nprovider: GoGift\nproviderId: gogift\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the GoGift authorization server. These were\n  read from the live `scopes_supported` array in the provider's own OpenID Connect discovery\n  document on both the production (auth.gogift.io) and sandbox (auth-pre.gogift.io) issuers —\n  the two arrays are identical. GoGift publishes no scope-reference page in its API docs, so\n  the descriptions below are the standard OIDC meanings where the scope is a standard one and\n  are marked `undocumented` where GoGift defines the scope itself.\nnote: >-\n  The API reference at docs.gogift.io never names a scope. Which of AuthApi / finance_api /\n\
  \  retail_api a given client is granted is decided by GoGift when it provisions the client id\n  and secret. Treat the non-standard scopes below as observed-from-discovery, not as a\n  provider-published permissions reference.\ndocs: null\ndocs_note: No scopes/permissions reference page is published by GoGift.\nscope_count: 11\nscopes:\n  - name: openid\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Requests an ID token; required for any OpenID Connect authentication request.\n  - name: profile\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Basic profile claims (name, family_name, given_name, preferred_username, locale, updated_at, picture, website, gender, birthdate, zoneinfo).\n  - name: email\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: The email and email_verified claims.\n  - name: address\n    standard: true\n    spec: OpenID Connect Core 1.0\n    description: The address claim.\n  - name: offline_access\n\
  \    standard: true\n    spec: OpenID Connect Core 1.0\n    description: Issues a refresh token so the client can renew the access token without re-authenticating.\n  - name: Permissions\n    standard: false\n    description: GoGift-defined scope releasing the `Permissions` claim, which carries the caller's platform permission set.\n    documented: false\n  - name: PhoneNumber\n    standard: false\n    description: GoGift-defined scope releasing the `PhoneNumber` claim.\n    documented: false\n  - name: Country\n    standard: false\n    description: GoGift-defined scope releasing the `Country` claim, used for locale/currency resolution.\n    documented: false\n  - name: AuthApi\n    standard: false\n    description: >-\n      Access to the GoGift authorization server's own administrative API surface\n      (auth.gogift.io/api/user, /api/group, /api/permission, /api/client, /api/apiresource and\n      the other endpoints advertised as *_endpoint in the discovery document).\n    documented:\
  \ false\n  - name: retail_api\n    standard: false\n    description: >-\n      Access to the retail/commerce surface on api.gogift.io — the product catalogue, basket\n      and order endpoints (POST|GET /products/filter, GET /products/{id}, POST /baskets,\n      PUT /baskets, POST /baskets/finalize).\n    documented: false\n    inferred: true\n    inference_basis: scope name matched against the documented endpoint families; GoGift does not state the mapping.\n  - name: finance_api\n    standard: false\n    description: >-\n      Access to the finance surface, consistent with the `InvoiceByFinance` payment method the\n      basket finalisation endpoint accepts.\n    documented: false\n    inferred: true\n    inference_basis: scope name matched against the documented `InvoiceByFinance` payment method; GoGift does not state the mapping.\nclaims_supported:\n  - sub\n  - name\n  - family_name\n  - given_name\n  - middle_name\n  - nickname\n  - zoneinfo\n  - locale\n  - updated_at\n  - birthdate\n\
  \  - gender\n  - preferred_username\n  - profile\n  - picture\n  - website\n  - email\n  - email_verified\n  - Permissions\n  - PhoneNumber\n  - Country\n  - address\n  - openid\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gogift/refs/heads/main/scopes/gogift-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Gift Cards
- Rewards
- Incentives
- Loyalty
- Commerce
- Payments
- Employee Recognition
- Loyalty & Incentives
token_urls: []
---
