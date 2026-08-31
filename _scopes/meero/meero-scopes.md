---
api_specs:
- filename: meero-asynchronous-api-openapi.yml
  format: yaml
  label: Meero Asynchronous API
  slug: meero-asynchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-asynchronous-api-openapi.yml
- filename: meero-feature-api-openapi.yml
  format: yaml
  label: Meero Feature API
  slug: meero-feature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-feature-api-openapi.yml
- filename: meero-synchronous-api-openapi.yml
  format: yaml
  label: Meero Synchronous API
  slug: meero-synchronous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-synchronous-api-openapi.yml
- filename: meero-vehicle-api-openapi.yml
  format: yaml
  label: Meero Vehicle API
  slug: meero-vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/openapi/meero-vehicle-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.carcutter.com/.well-known/oauth-protected-resource
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Meero Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Meero uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Meero
provider_slug: meero
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: meero-scopes
source_filename: meero-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://www.carcutter.com/.well-known/oauth-authorization-server\ndocs: https://www.carcutter.com/.well-known/oauth-protected-resource\nsummary: 'The Car-Cutter REST API declares no oauth2 security scheme — it is HTTP bearer only, with\n  no scope surface. The one OAuth 2.0 authorization server CarCutter operates belongs to its remote\n  MCP endpoint, and it advertises exactly one scope.'\nauthorization_servers:\n- issuer: https://www.carcutter.com\n  authorization_endpoint: https://www.carcutter.com/oauth/authorize\n  token_endpoint: https://www.carcutter.com/oauth/token\n  revocation_endpoint: https://www.carcutter.com/oauth/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  protects: https://www.carcutter.com/wp-json/mcp/mcp-oauth-server\n\
  - issuer: https://auth.eu.car-cutter.com/\n  kind: openid-connect\n  provider: Auth0\n  authorization_endpoint: https://auth.eu.car-cutter.com/authorize\n  token_endpoint: https://auth.eu.car-cutter.com/oauth/token\n  device_authorization_endpoint: https://auth.eu.car-cutter.com/oauth/device/code\n  userinfo_endpoint: https://auth.eu.car-cutter.com/userinfo\n  jwks_uri: https://auth.eu.car-cutter.com/.well-known/jwks.json\n  registration_endpoint: https://auth.eu.car-cutter.com/oidc/register\n  revocation_endpoint: https://auth.eu.car-cutter.com/oauth/revoke\n  code_challenge_methods_supported: [S256, plain]\n  protects: 'CarCutter Hub (hub.car-cutter.com) and the gated audience https://api2.car-cutter.com'\n  discovered_via: 'The Hub login redirect chain: https://hub.car-cutter.com/ -> /auth/login/ -> auth.eu.car-cutter.com/login?...&audience=https%3A%2F%2Fapi2.car-cutter.com'\n  scopes_note: 'scopes_supported is the stock Auth0 OIDC claim set (openid, profile, offline_access,\n    name,\
  \ given_name, family_name, nickname, email, email_verified, picture, created_at, identities,\n    phone, address). These are identity claims, not CarCutter API permissions — no product-scoped\n    values are published. The login request itself asks for only \"openid offline_access\".'\nscopes:\n- name: mcp\n  description: 'Access to the CarCutter MCP server resource. The authorization server publishes no\n    finer-grained scopes and no per-scope descriptions; this is the only value in scopes_supported\n    on both the authorization-server and the protected-resource metadata documents.'\n  source: /.well-known/oauth-authorization-server + /.well-known/oauth-protected-resource\nscope_count: 1\ngaps:\n- No scope decomposition (read vs write, per-tool) is published for the MCP resource.\n- The REST API has no scopes at all; a bearer token is all-or-nothing per account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meero/refs/heads/main/scopes/meero-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automotive
- Images
- Artificial Intelligence
- Computer Vision
- Photography
- Media Processing
- E-Commerce
- Vehicle Merchandising
- Company
token_urls: []
---
