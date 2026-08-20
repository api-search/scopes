---
api_specs:
- filename: ibotta-product-api-openapi.yml
  format: yaml
  label: Ibotta Product API
  slug: ibotta-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibotta/refs/heads/main/openapi/ibotta-product-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ibotta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ibotta uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ibotta
provider_slug: ibotta
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ibotta-scopes
source_filename: ibotta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.dashboard.ibotta.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  Ibotta's public Product API declares no OAuth 2.0 security scheme — it uses a single service\n  bearer token with no scopes. The only scope surface Ibotta publishes anonymously is the\n  scopes_supported list from the Auth0 tenant that fronts the IPN partner portal\n  (auth.dashboard.ibotta.com). These are stock OIDC identity scopes for portal sign-in, NOT\n  API authorization scopes for the Ibotta Performance Network partner APIs — those are not\n  publicly documented. Recorded here as measured, not as an API permission model.\nauthorization_servers:\n- issuer: https://auth.dashboard.ibotta.com/\n  applies_to: Ibotta Performance Network partner portal (portal.ipn.ibotta.com)\n  discovery: https://auth.dashboard.ibotta.com/.well-known/openid-configuration\n  status: 200\n  scope_kind: oidc-identity\n  scopes:\n  - name: openid\n   \
  \ description: Standard OIDC scope requesting an ID token.\n  - name: profile\n    description: Basic profile claims for the signed-in partner user.\n  - name: offline_access\n    description: Issues a refresh token for long-lived portal sessions.\n  - name: name\n    description: name claim.\n  - name: given_name\n    description: given_name claim.\n  - name: family_name\n    description: family_name claim.\n  - name: nickname\n    description: nickname claim.\n  - name: email\n    description: email claim.\n  - name: email_verified\n    description: email_verified claim.\n  - name: picture\n    description: picture claim.\n  - name: created_at\n    description: created_at claim (Auth0 extension).\n  - name: identities\n    description: Linked identity providers for the account (Auth0 extension).\n  - name: phone\n    description: phone_number claim.\n  - name: address\n    description: address claim.\n  claims_supported:\n  - aud\n  - auth_time\n  - created_at\n  - email\n  - email_verified\n\
  \  - exp\n  - family_name\n  - given_name\n  - iat\n  - identities\n  - iss\n  - name\n  - nickname\n  - phone_number\n  - picture\n  - sub\napi_scopes:\n  documented: false\n  note: >-\n    No API authorization scopes are published for either the Ibotta Product API (bearer token,\n    no scopes) or the IPN partner APIs (documentation is behind the partner portal login).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibotta/refs/heads/main/scopes/ibotta-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Cashback
- Rewards
- Retail Media
- Coupons
- Loyalty
- Shopping
- Advertising
- Promotions
- Product Search
- Retail
- Affiliates
- CPG
token_urls: []
---
