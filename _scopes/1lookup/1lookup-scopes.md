---
authorization_urls:
- https://app.1lookup.io/api/mcp/oauth/authorize
description: 1Lookup's only OAuth surface is the hosted MCP connector. Its authorization-server metadata (RFC 8414) and protected-resource metadata (RFC 9728) both advertise a single scope. The REST API at /api/v1 uses static API keys and has no scope model at all — do not read this file as covering it.
docs: https://www.1lookup.io/products/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 1Lookup Scopes
name_suffix: OAuth Scopes
note: ''
overview: '1Lookup publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1Lookup API on a user''s behalf.


  Tokens are issued from https://app.1lookup.io/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1Lookup
provider_slug: 1lookup
schemes:
- flows:
  - authorizationUrl: https://app.1lookup.io/api/mcp/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://app.1lookup.io/api/mcp/oauth/token
  issuer: https://app.1lookup.io
  name: mcpOAuth21
  resource: https://app.1lookup.io/api/mcp
  source: well-known/1lookup-oauth-authorization-server.json
scope_count: 1
scope_names:
- lookup
scopes:
- description: Grants an MCP client the five 1Lookup tools (validate_phone, verify_email, ip_lookup, bulk_verify, get_account). Provider describes the grant as read-only; calls bill against the authorizing account's plan credits.
  flows:
  - authorizationCode
  scope: lookup
slug: 1lookup-scopes
source_filename: 1lookup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://app.1lookup.io/.well-known/oauth-authorization-server\ndocs: https://www.1lookup.io/products/mcp\ndescription: >-\n  1Lookup's only OAuth surface is the hosted MCP connector. Its authorization-server metadata (RFC 8414)\n  and protected-resource metadata (RFC 9728) both advertise a single scope. The REST API at\n  /api/v1 uses static API keys and has no scope model at all — do not read this file as covering it.\nschemes:\n  - name: mcpOAuth21\n    source: well-known/1lookup-oauth-authorization-server.json\n    issuer: https://app.1lookup.io\n    resource: https://app.1lookup.io/api/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.1lookup.io/api/mcp/oauth/authorize\n        tokenUrl: https://app.1lookup.io/api/mcp/oauth/token\n        pkce: [S256]\nscopes:\n  - scope: lookup\n    description: >-\n      Grants an MCP client the five 1Lookup tools (validate_phone, verify_email, ip_lookup,\
  \ bulk_verify,\n      get_account). Provider describes the grant as read-only; calls bill against the authorizing\n      account's plan credits.\n    flows: [authorizationCode]\n    sources:\n      - well-known/1lookup-oauth-authorization-server.json\n      - well-known/1lookup-oauth-protected-resource.json\ngaps:\n  - >-\n    A single coarse `lookup` scope covers all five tools; there is no separation between the\n    credit-spending validation tools and the read-only get_account tool, so an agent cannot be granted\n    balance visibility without also being granted the ability to spend credits.\n  - No published scopes/permissions reference page beyond the MCP product page.\nx-evidence:\n  - url: https://app.1lookup.io/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-09'\n  - url: https://app.1lookup.io/.well-known/oauth-protected-resource\n    http_status: 200\n    fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1lookup/refs/heads/main/scopes/1lookup-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Phone Validation
- Email Validation
- IP Intelligence
- Fraud and Risk
- Data Enrichment
- B2B contact & company data
- SEO / web analytics
- Audio Transcription
- MCP / agent-native
- REST API
token_urls:
- https://app.1lookup.io/api/mcp/oauth/token
---
