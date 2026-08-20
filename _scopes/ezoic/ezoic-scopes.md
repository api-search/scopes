---
api_specs:
- filename: ezoic-access-api-openapi.yml
  format: yaml
  label: ezoic Access API
  slug: ezoic-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-access-api-openapi.yml
- filename: ezoic-products-api-openapi.yml
  format: yaml
  label: ezoic Products API
  slug: ezoic-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-products-api-openapi.yml
- filename: ezoic-purchases-api-openapi.yml
  format: yaml
  label: ezoic Purchases API
  slug: ezoic-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-purchases-api-openapi.yml
- filename: ezoic-big-data-analytics-api-openapi.yml
  format: yaml
  label: ezoic Big Data Analytics API
  slug: ezoic-big-data-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-big-data-analytics-api-openapi.yml
- filename: ezoic-cdn-api-openapi.yml
  format: yaml
  label: ezoic CDN API
  slug: ezoic-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-cdn-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.ezoic.com/docs/analytics-mcp/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ezoic Scopes
name_suffix: OAuth Scopes
note: 'Ezoic runs a real OAuth 2.0 authorization server at token.ezoic.com and publishes RFC 8414 metadata for it, but that metadata omits scopes_supported and Ezoic publishes no scope reference page. The access token issued to an MCP client is described in prose as "a scoped access token", and the gate is an Ezoic ROLE PERMISSION ("Analytics"), not a named OAuth scope a client can request. So there is nothing to enumerate: scope_count is 0 by measurement, not by omission.'
overview: 'ezoic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ezoic
provider_slug: ezoic
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ezoic-scopes
source_filename: ezoic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://token.ezoic.com/.well-known/oauth-authorization-server\ndocs: https://docs.ezoic.com/docs/analytics-mcp/\nnote: >-\n  Ezoic runs a real OAuth 2.0 authorization server at token.ezoic.com and publishes RFC\n  8414 metadata for it, but that metadata omits scopes_supported and Ezoic publishes no\n  scope reference page. The access token issued to an MCP client is described in prose as\n  \"a scoped access token\", and the gate is an Ezoic ROLE PERMISSION (\"Analytics\"), not a\n  named OAuth scope a client can request. So there is nothing to enumerate: scope_count\n  is 0 by measurement, not by omission.\nauthorization_server:\n  issuer: https://token.ezoic.com\n  metadata: https://token.ezoic.com/.well-known/oauth-authorization-server\n  authorization_endpoint: https://token.ezoic.com/authorize\n  token_endpoint: https://token.ezoic.com/token\n  revocation_endpoint: https://token.ezoic.com/token/revoke\n  registration_endpoint:\
  \ https://token.ezoic.com/register\n  device_authorization_endpoint: https://token.ezoic.com/device_authorization\n  jwks_uri: https://token.ezoic.com/.well-known/jwks.json\n  scopes_supported: null\n  scopes_supported_note: Field absent from the published metadata document.\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:device_code\n  - personal_access_token\n  - urn:bidsystem:params:oauth:grant-type:adcp-client-recovery\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none, private_key_jwt]\n  token_endpoint_auth_signing_alg_values_supported: [ES256]\n  id_token_signing_alg_values_supported: [ES256]\n  dpop_signing_alg_values_supported: [ES256]\n  subject_types_supported: [public]\n  client_metadata_document_supported: false\nsecond_authorization_server:\n  issuer: https://token.bidsystem.ai\n\
  \  metadata: https://token.bidsystem.ai/.well-known/oauth-authorization-server\n  applies_to: bidsystem.ai — Ezoic's performance advertising (buy-side) platform\n  ownership: >-\n    Different domain, same company. bidsystem.ai's homepage states \"bidsystem.ai is\n    Ezoic's performance advertising platform\"; ezoic.com's homepage \"Get Started\" CTA\n    links to https://admin.bidsystem.ai/register; and token.ezoic.com itself advertises\n    the vendor grant urn:bidsystem:params:oauth:grant-type:adcp-client-recovery.\n  configuration: >-\n    Identical to token.ezoic.com in every field except issuer and endpoint hostnames —\n    same grants, same S256-only PKCE, same ES256 DPoP, same dynamic client registration,\n    same auth methods. One authorization codebase, two brands.\n  scopes_supported: null\nprotected_resources:\n- resource: https://analytics-mcp.ezoic.com\n  metadata: https://analytics-mcp.ezoic.com/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n\
  \  authorization_servers: [https://token.ezoic.com]\n  scopes_supported: null\n- resource: https://api.bidsystem.ai/mcp\n  metadata: https://api.bidsystem.ai/.well-known/oauth-protected-resource\n  bearer_methods_supported: [header]\n  authorization_servers: [https://token.bidsystem.ai]\n  scopes_supported: [openid, profile]\n  note: >-\n    The only Ezoic-family resource that names any scope — and the two it names are the\n    OIDC identity scopes, not authorization scopes over advertising data. So even here,\n    nothing describes what an access token is permitted to DO.\nscopes:\n- name: openid\n  description: Standard OIDC scope. Published only by the bidsystem.ai MCP protected resource.\n  resource: https://api.bidsystem.ai/mcp\n  source: https://api.bidsystem.ai/.well-known/oauth-protected-resource\n  method: probed\n- name: profile\n  description: Standard OIDC scope. Published only by the bidsystem.ai MCP protected resource.\n  resource: https://api.bidsystem.ai/mcp\n  source:\
  \ https://api.bidsystem.ai/.well-known/oauth-protected-resource\n  method: probed\nscope_count: 2\nscope_count_note: >-\n  Both are generic OIDC identity scopes discovered by probe, not an Ezoic authorization\n  vocabulary. No Ezoic-authored scope exists on any surface, and no scope reference page is\n  published.\npermissions:\n  note: >-\n    Authorization is enforced through Ezoic account roles rather than OAuth scopes.\n    Documented at https://docs.ezoic.com/docs/analytics-mcp/.\n  model:\n  - name: Analytics\n    effect: >-\n      A publisher user (a team member on someone else's Ezoic account) can connect the\n      Analytics MCP only if their Ezoic role includes analytics access — matching what\n      they can already see in the Ezoic dashboard. Account owners manage team permissions\n      under Account -> Privacy & Security -> Manage Users.\n    surface: https://analytics-mcp.ezoic.com/mcp\n  - name: 'API Access (per service)'\n    effect: >-\n      Not OAuth. Each API-gateway\
  \ service (Big Data Analytics, CDN, Subscriptions) is off\n      until a publisher turns it on under Settings -> API Access; the shared developerKey\n      can only call enabled services, and only for domains on its own account.\n    surface: https://api-gateway.ezoic.com\n    docs: https://docs.ezoic.com/docs/api/\nobservations:\n  strong:\n  - PKCE (S256) is the only code challenge method offered — no plain.\n  - DPoP sender-constrained tokens are supported (ES256).\n  - Dynamic client registration (RFC 7591) is available at /register, which is what lets an\n    MCP client connect without a pre-provisioned client_id.\n  - Token revocation (RFC 7009) is published.\n  notable:\n  - >-\n    A vendor-specific grant type is advertised on BOTH authorization servers —\n    urn:bidsystem:params:oauth:grant-type:adcp-client-recovery — indicating Ezoic's token\n    service fronts an Ad Context Protocol (AdCP) bidding client. No AdCP discovery\n    document is published on any host probed (/.well-known/adcp.json\
  \ 404s on both\n    ezoic.com and api.bidsystem.ai), so this is recorded as an observation, not as a\n    catalogued API. It is, however, the thread that led to the third MCP server.\n  - >-\n    The bidsystem.ai advertiser console carries a Chrome WebMCP origin-trial token\n    (feature \"WebMCP\", origin https://admin.bidsystem.ai:443, expiry 2026-11-17) — Ezoic is\n    trialling in-page agent tool exposure alongside its server-side MCP endpoints.\n  - No OIDC. /.well-known/openid-configuration 404s on both token.ezoic.com and\n    login.ezoic.com, yet id_token_signing_alg_values_supported is present in the OAuth\n    metadata — an OIDC-shaped field on a non-OIDC discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/scopes/ezoic-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Reporting
- Subscription
- Paywalls
- Identity
- CDN
- Caching
- MCP
- Authentication
- Agents
token_urls: []
---
