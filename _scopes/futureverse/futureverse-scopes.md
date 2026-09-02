---
api_specs:
- filename: futureverse-campaigns-api-openapi.yml
  format: yaml
  label: Futureverse Campaigns API
  slug: futureverse-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/openapi/futureverse-campaigns-api-openapi.yml
- filename: futureverse-quests-api-openapi.yml
  format: yaml
  label: Futureverse Quests API
  slug: futureverse-quests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/openapi/futureverse-quests-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.therootnetwork.com/learn/features/identity-protocol
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Futureverse Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 securityScheme to derive from — the only OpenAPI in this repo is the generated RootRewards description, which uses an API key. These scopes are read directly from the live FuturePass OIDC discovery document instead, and saved verbatim to well-known/futureverse-openid-configuration.json.
overview: 'Futureverse uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Futureverse
provider_slug: futureverse
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: futureverse-scopes
source_filename: futureverse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: https://login.futureverse.app/.well-known/openid-configuration\nsource_status: 200\ndocs: https://docs.therootnetwork.com/learn/features/identity-protocol\nnote: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme to derive from — the only OpenAPI in this\n  repo is the generated RootRewards description, which uses an API key. These scopes are read\n  directly from the live FuturePass OIDC discovery document instead, and saved verbatim to\n  well-known/futureverse-openid-configuration.json.\n\nprovider: FuturePass Identity (OpenID Connect)\nissuer: https://login.futureverse.app\nauthorization_endpoint: https://login.futureverse.app/auth\ntoken_endpoint: https://login.futureverse.app/token\n\nscope_count: 2\nscopes:\n  - name: openid\n    description: >-\n      Required OIDC scope. Requests an ID token identifying the FuturePass subject.\n    standard: true\n  - name: offline_access\n    description: >-\n      Requests\
  \ a refresh token so the client can obtain new access tokens without user interaction.\n    standard: true\n\nfinding: >-\n  FuturePass publishes exactly the two baseline OIDC scopes and nothing else. There is no\n  product-level authorization vocabulary — no read/write split, no per-resource scope, no\n  consent-visible permission a user could reason about. Everything an integrating application is\n  permitted to do is decided outside the token. What FuturePass DOES carry is unusually rich\n  identity: the discovery document advertises custom claims (eoa, custodian, chainId, futurepass,\n  connectorId, passName) that bind the OIDC subject to an on-chain smart wallet. So the token is\n  strong on WHO and silent on WHAT.\n\nclaims_supported:\n  - sub\n  - iss\n  - sid\n  - auth_time\n  - email\n  - profile\n  - eoa\n  - custodian\n  - chainId\n  - futurepass\n  - connectorId\n  - passName\n\nother_surfaces:\n  - api: Futureverse Asset Register API\n    model: >-\n      No OAuth scopes.\
  \ Authorization is either a SIWE bearer token (admin operations) or a\n      wallet-signed ARTM transaction (state changes). Permission is proven by key ownership, not\n      granted by scope.\n  - api: RootRewards Quest API\n    model: >-\n      No OAuth. An `sk_`-prefixed API key bound to the quest owner account; authorization is\n      ownership of the quest, checked server-side.\n  - api: The Root Network Documentation MCP Server\n    model: >-\n      Unauthenticated. Neither /.well-known/oauth-protected-resource nor\n      /.well-known/oauth-authorization-server is served on the MCP host (both 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/scopes/futureverse-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Blockchain
- Web3
- Metaverse
- Digital Assets
- NFT
- GraphQL
- Identity
- OpenID Connect
- asset-registry
- Layer 1
- EVM
- Gaming
- agent-native
- MCP
token_urls: []
---
