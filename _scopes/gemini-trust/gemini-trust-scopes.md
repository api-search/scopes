---
api_specs:
- filename: gemini-trust-websocket-asyncapi.yml
  format: yaml
  label: Gemini WebSocket API
  slug: gemini-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/asyncapi/gemini-trust-websocket-asyncapi.yml
- filename: gemini-trust-account-administration-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Account Administration API
  slug: gemini-trust-account-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-account-administration-api-openapi.yml
- filename: gemini-trust-clearing-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Clearing API
  slug: gemini-trust-clearing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-clearing-api-openapi.yml
- filename: gemini-trust-combos-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Combos API
  slug: gemini-trust-combos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-combos-api-openapi.yml
- filename: gemini-trust-derivatives-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Derivatives API
  slug: gemini-trust-derivatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-derivatives-api-openapi.yml
- filename: gemini-trust-fund-management-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Fund Management API
  slug: gemini-trust-fund-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-fund-management-api-openapi.yml
- filename: gemini-trust-instant-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Instant API
  slug: gemini-trust-instant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-instant-api-openapi.yml
- filename: gemini-trust-margin-trading-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Margin Trading API
  slug: gemini-trust-margin-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-margin-trading-api-openapi.yml
- filename: gemini-trust-market-data-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Market Data API
  slug: gemini-trust-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-market-data-api-openapi.yml
- filename: gemini-trust-markets-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Markets API
  slug: gemini-trust-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-markets-api-openapi.yml
- filename: gemini-trust-oauth-api-openapi.yml
  format: yaml
  label: Gemini Trust Company OAuth API
  slug: gemini-trust-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-oauth-api-openapi.yml
- filename: gemini-trust-orders-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Orders API
  slug: gemini-trust-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-orders-api-openapi.yml
- filename: gemini-trust-positions-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Positions API
  slug: gemini-trust-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-positions-api-openapi.yml
- filename: gemini-trust-rewards-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Rewards API
  slug: gemini-trust-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-rewards-api-openapi.yml
- filename: gemini-trust-session-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Session API
  slug: gemini-trust-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-session-api-openapi.yml
- filename: gemini-trust-staking-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Staking API
  slug: gemini-trust-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-staking-api-openapi.yml
- filename: gemini-trust-terms-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Terms API
  slug: gemini-trust-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-terms-api-openapi.yml
- filename: gemini-trust-trading-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Trading API
  slug: gemini-trust-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-trading-api-openapi.yml
- filename: gemini-trust-volume-api-openapi.yml
  format: yaml
  label: Gemini Trust Company Volume API
  slug: gemini-trust-volume-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/openapi/gemini-trust-volume-api-openapi.yml
authorization_urls:
- https://exchange.gemini.com/auth
description: ''
docs: https://developer.gemini.com/authentication/oauth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gemini Trust Scopes
name_suffix: OAuth Scopes
note: These scopes are NOT in either OpenAPI - neither spec declares an oauth2 securityScheme, so the derive-from-spec path returns nothing. They come from the provider's live RFC 8414 authorization-server metadata, which is the authoritative machine-readable source. 33 scopes, resource:action shaped.
overview: 'Gemini Trust Company publishes 32 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gemini Trust Company API on a user''s behalf.


  Tokens are issued from https://exchange.gemini.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gemini Trust Company
provider_slug: gemini-trust
schemes: []
scope_count: 32
scope_names:
- account:read
- addresses:create
- addresses:read
- balances:read
- banks:create
- banks:read
- clearing:create
- clearing:read
- crypto:send
- fdx:accountbasic:read
- fdx:accountdetailed:read
- fdx:customercontact:read
- fdx:rewards:read
- fdx:statements:read
- fdx:transactions:read
- history:read
- orders:create
- orders:read
- payments:create
- payments:read
- payments:send
- positions:read
- predictions:balances:read
- predictions:orders:read
- predictions:orders:write
- predictions:positions:read
- savedAddresses:create
- savedAddresses:read
- settlement:create-update
- settlement:read
- settlement:read-all
- settlement:update
scopes:
- description: ''
  flows: []
  scope: account:read
- description: ''
  flows: []
  scope: addresses:create
- description: ''
  flows: []
  scope: addresses:read
- description: ''
  flows: []
  scope: balances:read
- description: ''
  flows: []
  scope: banks:create
- description: ''
  flows: []
  scope: banks:read
- description: ''
  flows: []
  scope: clearing:create
- description: ''
  flows: []
  scope: clearing:read
- description: ''
  flows: []
  scope: crypto:send
- description: ''
  flows: []
  scope: fdx:accountbasic:read
- description: ''
  flows: []
  scope: fdx:accountdetailed:read
- description: ''
  flows: []
  scope: fdx:customercontact:read
- description: ''
  flows: []
  scope: fdx:rewards:read
- description: ''
  flows: []
  scope: fdx:statements:read
- description: ''
  flows: []
  scope: fdx:transactions:read
- description: ''
  flows: []
  scope: history:read
- description: ''
  flows: []
  scope: orders:create
- description: ''
  flows: []
  scope: orders:read
- description: ''
  flows: []
  scope: payments:create
- description: ''
  flows: []
  scope: payments:read
- description: ''
  flows: []
  scope: payments:send
- description: ''
  flows: []
  scope: positions:read
- description: ''
  flows: []
  scope: predictions:balances:read
- description: ''
  flows: []
  scope: predictions:orders:read
- description: ''
  flows: []
  scope: predictions:orders:write
- description: ''
  flows: []
  scope: predictions:positions:read
- description: ''
  flows: []
  scope: savedAddresses:create
- description: ''
  flows: []
  scope: savedAddresses:read
- description: ''
  flows: []
  scope: settlement:create-update
- description: ''
  flows: []
  scope: settlement:read
- description: ''
  flows: []
  scope: settlement:read-all
- description: ''
  flows: []
  scope: settlement:update
slug: gemini-trust-scopes
source_filename: gemini-trust-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: https://api.gemini.com/.well-known/oauth-authorization-server\ndocs: https://developer.gemini.com/authentication/oauth\nnote: These scopes are NOT in either OpenAPI - neither spec declares an oauth2 securityScheme, so the derive-from-spec\n  path returns nothing. They come from the provider's live RFC 8414 authorization-server metadata, which is the authoritative\n  machine-readable source. 33 scopes, resource:action shaped.\nissuer: https://exchange.gemini.com\nauthorization_endpoint: https://exchange.gemini.com/auth\ntoken_endpoint: https://exchange.gemini.com/auth/token\nrevocation_endpoint: https://exchange.gemini.com/auth/token/revoke\nintrospection_endpoint: https://exchange.gemini.com/auth/token/introspect\nuserinfo_endpoint: https://exchange.gemini.com/userinfo\ngrant_types:\n- authorization_code\n- refresh_token\npkce:\n  supported: true\n  methods:\n  - S256\n  required_for: public clients (SPA, mobile, desktop)\ntoken_lifetime:\n\
  \  access_token: 24 hours\n  refresh_token: non-expiring\nscope_count: 32\nscopes:\n- name: account:read\n- name: addresses:create\n- name: addresses:read\n- name: balances:read\n- name: banks:create\n- name: banks:read\n- name: clearing:create\n- name: clearing:read\n- name: crypto:send\n- name: fdx:accountbasic:read\n- name: fdx:accountdetailed:read\n- name: fdx:customercontact:read\n- name: fdx:rewards:read\n- name: fdx:statements:read\n- name: fdx:transactions:read\n- name: history:read\n- name: orders:create\n- name: orders:read\n- name: payments:create\n- name: payments:read\n- name: payments:send\n- name: positions:read\n- name: predictions:balances:read\n- name: predictions:orders:read\n- name: predictions:orders:write\n- name: predictions:positions:read\n- name: savedAddresses:create\n- name: savedAddresses:read\n- name: settlement:create-update\n- name: settlement:read\n- name: settlement:read-all\n- name: settlement:update\nscope_families:\n  fdx:\n    count: 6\n    note: 'Financial\
  \ Data Exchange (FDX) namespaced scopes - fdx:accountbasic:read, fdx:accountdetailed:read, fdx:customercontact:read,\n      fdx:rewards:read, fdx:statements:read, fdx:transactions:read. See conformance/gemini-trust-conformance.yml:\n      this is a real domain-standard signature carried in the contract, not a marketing claim.'\n  predictions:\n    count: 4\n  settlement:\n    count: 4\nsandbox:\n  issuer: https://exchange.sandbox.gemini.com\n  source: https://api.sandbox.gemini.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemini-trust/refs/heads/main/scopes/gemini-trust-scopes.yml
summary_line: 32 scopes
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
token_bound: false
token_urls:
- https://exchange.gemini.com/auth/token
---
