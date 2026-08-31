---
api_specs:
- filename: public
  format: yaml
  label: Yahoo DSP Traffic API
  slug: dsp-traffic-api
  spec_type: Postman
  url: https://www.postman.com/yahoodsp/workspace/public
authorization_urls: []
description: OAuth scope surface for the Yahoo identity service at api.login.yahoo.com. The four scopes below are the ones the provider advertises in its own OpenID Connect discovery document; they cover sign-in and profile/email claims. Per-API data permissions (for example Fantasy Sports read/write) are granted as API Permissions selected when an app is registered at developer.yahoo.com/apps/create/, not as discovery-published scope strings, and Yahoo does not publish a machine-readable list of those permission identifiers.
docs: https://developer.yahoo.com/oauth2/guide/openid_connect/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Yahoo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yahoo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yahoo
provider_slug: yahoo
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: yahoo-scopes
source_filename: yahoo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Yahoo\nproviderId: yahoo\ngenerated: '2026-08-28'\nmethod: searched\nsource: >-\n  https://api.login.yahoo.com/.well-known/openid-configuration ,\n  https://developer.yahoo.com/oauth2/guide/openid_connect/ ,\n  https://developer.yahoo.com/apps/create/\ndocs: https://developer.yahoo.com/oauth2/guide/openid_connect/\ndescription: >-\n  OAuth scope surface for the Yahoo identity service at api.login.yahoo.com. The four scopes\n  below are the ones the provider advertises in its own OpenID Connect discovery document; they\n  cover sign-in and profile/email claims. Per-API data permissions (for example Fantasy Sports\n  read/write) are granted as API Permissions selected when an app is registered at\n  developer.yahoo.com/apps/create/, not as discovery-published scope strings, and Yahoo does not\n  publish a machine-readable list of those permission identifiers.\nauthorization_server: https://api.login.yahoo.com\n\
  discovery: https://api.login.yahoo.com/.well-known/openid-configuration\nscopes:\n  - name: openid\n    description: Requests an OpenID Connect ID token identifying the signed-in Yahoo user.\n    source: discovery scopes_supported\n  - name: openid2\n    description: >-\n      Yahoo's legacy OpenID 2.0 compatibility scope, returned alongside openid for callers\n      migrating from the retired OpenID 2.0 endpoints.\n    source: discovery scopes_supported\n  - name: profile\n    description: >-\n      Basic profile claims - name, given_name, family_name, birthdate, locale.\n    source: discovery scopes_supported\n  - name: email\n    description: The user's email address and its verification state (email, email_verified).\n    source: discovery scopes_supported\nscope_count: 4\nnot_scope_based:\n  - api: Yahoo DSP Traffic API\n    reason: >-\n      Two-legged client_credentials with a JWT client assertion; access is bounded by the seat and\n      user role assigned in the DSP UI, not by\
  \ OAuth scope strings.\n  - api: Yahoo DSP Reporting API\n    reason: Same client_credentials model as the Traffic API; no scope parameter is documented.\n  - api: Yahoo Ad Tech DataX API\n    reason: >-\n      Access is provisioned per partner during onboarding via an exchanged RSA public key; no\n      scopes are published.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yahoo/refs/heads/main/scopes/yahoo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Advertising
- Programmatic Advertising
- Demand-Side Platform
- Fantasy Sports
- Sports Data
- Identity
- OpenID Connect
- Authentication
- Audience Data
- Media
- Reporting
- Conversion Tracking
token_urls: []
---
