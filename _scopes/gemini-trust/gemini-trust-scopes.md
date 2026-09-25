---
api_specs:
- filename: gemini-trust-rest-openapi.yml
  format: yaml
  label: Gemini Crypto Trading REST API
  slug: gemini-crypto-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-rest-openapi.yml
- filename: gemini-trust-prediction-markets-openapi.yml
  format: yaml
  label: Gemini Prediction Markets REST API
  slug: gemini-prediction-markets-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-prediction-markets-openapi.yml
- filename: gemini-trust-websocket-asyncapi.yml
  format: yaml
  label: Gemini WebSocket API
  slug: gemini-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/asyncapi/gemini-trust-websocket-asyncapi.yml
authorization_urls: []
description: ''
docs: https://developer.gemini.com/authentication/oauth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gemini Trust Scopes
name_suffix: OAuth Scopes
note: These scopes are NOT in either OpenAPI - neither spec declares an oauth2 securityScheme, so the derive-from-spec path returns nothing. They come from the provider's live RFC 8414 authorization-server metadata, which is the authoritative machine-readable source. 33 scopes, resource:action shaped.
overview: 'Gemini Trust Company uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gemini Trust Company
provider_slug: gemini-trust
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: gemini-trust-scopes
source_filename: gemini-trust-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: https://api.gemini.com/.well-known/oauth-authorization-server\ndocs: https://developer.gemini.com/authentication/oauth\nnote: These scopes are NOT in either OpenAPI - neither spec declares an oauth2 securityScheme, so the derive-from-spec\n  path returns nothing. They come from the provider's live RFC 8414 authorization-server metadata, which is the authoritative\n  machine-readable source. 33 scopes, resource:action shaped.\nissuer: https://exchange.gemini.com\nauthorization_endpoint: https://exchange.gemini.com/auth\ntoken_endpoint: https://exchange.gemini.com/auth/token\nrevocation_endpoint: https://exchange.gemini.com/auth/token/revoke\nintrospection_endpoint: https://exchange.gemini.com/auth/token/introspect\nuserinfo_endpoint: https://exchange.gemini.com/userinfo\ngrant_types:\n- authorization_code\n- refresh_token\npkce:\n  supported: true\n  methods:\n  - S256\n  required_for: public clients (SPA, mobile, desktop)\ntoken_lifetime:\n\
  \  access_token: 24 hours\n  refresh_token: non-expiring\nscope_count: 32\nscopes:\n- name: account:read\n- name: addresses:create\n- name: addresses:read\n- name: balances:read\n- name: banks:create\n- name: banks:read\n- name: clearing:create\n- name: clearing:read\n- name: crypto:send\n- name: fdx:accountbasic:read\n- name: fdx:accountdetailed:read\n- name: fdx:customercontact:read\n- name: fdx:rewards:read\n- name: fdx:statements:read\n- name: fdx:transactions:read\n- name: history:read\n- name: orders:create\n- name: orders:read\n- name: payments:create\n- name: payments:read\n- name: payments:send\n- name: positions:read\n- name: predictions:balances:read\n- name: predictions:orders:read\n- name: predictions:orders:write\n- name: predictions:positions:read\n- name: savedAddresses:create\n- name: savedAddresses:read\n- name: settlement:create-update\n- name: settlement:read\n- name: settlement:read-all\n- name: settlement:update\nscope_families:\n  fdx:\n    count: 6\n    note: 'Financial\
  \ Data Exchange (FDX) namespaced scopes - fdx:accountbasic:read, fdx:accountdetailed:read, fdx:customercontact:read,\n      fdx:rewards:read, fdx:statements:read, fdx:transactions:read. See conformance/gemini-trust-conformance.yml:\n      this is a real domain-standard signature carried in the contract, not a marketing claim.'\n  predictions:\n    count: 4\n  settlement:\n    count: 4\nsandbox:\n  issuer: https://exchange.sandbox.gemini.com\n  source: https://api.sandbox.gemini.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/scopes/gemini-trust-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Order Management
- Clearing
- Custody
- Financial Services
- Prediction Markets
- Staking
- Derivatives
- WebSocket
- FIX
- Real-Time
- A2A
token_urls: []
---
