---
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by the point.me identity tenant. All fourteen are standard OIDC scopes and OIDC claim-shorthand scopes; none are product scopes. No API-resource scopes (audience-specific permissions for api.point.me) are anonymously discoverable, because api.point.me returns 401 on every path including /.well-known/oauth-protected-resource.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Point Me Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'POINT.ME uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: POINT.ME
provider_slug: point-me
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: point-me-scopes
source_filename: point-me-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  scopes_supported in https://auth.point.me/.well-known/openid-configuration\n  (HTTP 200, fetched 2026-08-26). point.me publishes no scopes or permissions\n  reference page — these are the scopes its Auth0 identity tenant advertises,\n  not an API authorization model the company documents.\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the point.me identity tenant.\n  All fourteen are standard OIDC scopes and OIDC claim-shorthand scopes; none are\n  product scopes. No API-resource scopes (audience-specific permissions for\n  api.point.me) are anonymously discoverable, because api.point.me returns 401 on\n  every path including /.well-known/oauth-protected-resource.\napi: point-me-flight-search-api\nissuer: https://auth.point.me/\nauthorization_endpoint: https://auth.point.me/authorize\ntoken_endpoint: https://auth.point.me/oauth/token\ndocs: null\ndocs_note: no published scopes/permissions reference\
  \ page was found on any point.me host\nscope_count: 14\nscopes:\n  - name: openid\n    description: Standard OIDC scope; requests an ID token.\n    standard: true\n  - name: profile\n    description: Standard OIDC scope; basic profile claims.\n    standard: true\n  - name: offline_access\n    description: Standard OIDC scope; requests a refresh token.\n    standard: true\n  - name: email\n    description: Standard OIDC scope; the end user's email address.\n    standard: true\n  - name: address\n    description: Standard OIDC scope; the end user's postal address.\n    standard: true\n  - name: phone\n    description: Standard OIDC scope; the end user's phone number.\n    standard: true\n  - name: name\n    description: OIDC claim-shorthand scope (Auth0); full name claim.\n    standard: true\n  - name: given_name\n    description: OIDC claim-shorthand scope (Auth0); given name claim.\n    standard: true\n  - name: family_name\n    description: OIDC claim-shorthand scope (Auth0); family name\
  \ claim.\n    standard: true\n  - name: nickname\n    description: OIDC claim-shorthand scope (Auth0); nickname claim.\n    standard: true\n  - name: email_verified\n    description: OIDC claim-shorthand scope (Auth0); email verification status.\n    standard: true\n  - name: picture\n    description: OIDC claim-shorthand scope (Auth0); profile picture claim.\n    standard: true\n  - name: created_at\n    description: Auth0 claim-shorthand scope; account creation timestamp.\n    standard: false\n  - name: identities\n    description: Auth0 claim-shorthand scope; linked identity providers.\n    standard: false\nx-evidence:\n  checked: '2026-08-26'\n  probes:\n    - url: https://auth.point.me/.well-known/openid-configuration\n      status: 200\n    - url: https://api.point.me/.well-known/oauth-protected-resource\n      status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/point-me/refs/heads/main/scopes/point-me-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Travel
- Award Travel
- Loyalty
- Points and Miles
- Flights
- Rewards
- Embedded Finance
- Banking
- Search
- Company
token_urls: []
---
