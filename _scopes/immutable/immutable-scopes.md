---
api_specs:
- filename: immutable-zkevm-openapi.json
  format: json
  label: Immutable zkEVM API
  slug: immutable-zkevm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-zkevm-openapi.json
- filename: immutable-audience-openapi.json
  format: json
  label: Immutable Audience API
  slug: immutable-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-audience-openapi.json
authorization_urls: []
description: ''
docs: https://docs.immutable.com/docs/products/passport/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Immutable Scopes
name_suffix: OAuth Scopes
note: 'Neither published OpenAPI declares an oauth2 securityScheme, so derive-oauth-scopes.py found nothing to derive (it reported "providers with oauth2: 0"). The scope surface is real but lives one layer out, in the Passport OpenID Connect provider''s anonymous discovery document at auth.immutable.com. These are OIDC standard claim-scopes, not per-resource API permissions: Immutable''s REST authorisation is API-key based (publishable vs secret), and there is no published per-endpoint permission catalogue.'
overview: 'Immutable uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Immutable
provider_slug: immutable
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: immutable-scopes
source_filename: immutable-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://auth.immutable.com/.well-known/openid-configuration\ndocs: https://docs.immutable.com/docs/products/passport/authentication\nnote: >-\n  Neither published OpenAPI declares an oauth2 securityScheme, so\n  derive-oauth-scopes.py found nothing to derive (it reported \"providers with\n  oauth2: 0\"). The scope surface is real but lives one layer out, in the Passport\n  OpenID Connect provider's anonymous discovery document at auth.immutable.com.\n  These are OIDC standard claim-scopes, not per-resource API permissions:\n  Immutable's REST authorisation is API-key based (publishable vs secret), and\n  there is no published per-endpoint permission catalogue.\nissuer: https://auth.immutable.com/\nauthorization_endpoint: https://auth.immutable.com/authorize\ntoken_endpoint: https://auth.immutable.com/oauth/token\nscope_count: 14\nscopes:\n- name: openid\n  description: Required for OpenID Connect; returns an ID token.\n- name:\
  \ profile\n  description: Basic profile claims for the authenticated Passport user.\n- name: offline_access\n  description: Issues a refresh token so the session survives access-token expiry.\n- name: email\n  description: The user's email address.\n- name: email_verified\n  description: Whether the user's email address has been verified.\n- name: name\n  description: Full name claim.\n- name: given_name\n  description: Given name claim.\n- name: family_name\n  description: Family name claim.\n- name: nickname\n  description: Nickname claim.\n- name: picture\n  description: Profile picture URL claim.\n- name: created_at\n  description: Account creation timestamp claim.\n- name: identities\n  description: Linked external identities for the Passport account.\n- name: phone\n  description: Phone number claim.\n- name: address\n  description: Address claim.\nx-evidence:\n  fetched: '2026-08-23'\n  url: https://auth.immutable.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/scopes/immutable-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Wallets
- Marketplace
- Analytics
- Attribution
- Customer Data Platform
- Authentication
- Developer Platform
token_urls: []
---
