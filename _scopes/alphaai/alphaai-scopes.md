---
api_specs:
- filename: alphaai-calendar-api-openapi.yml
  format: yaml
  label: AlphaAI Calendar API
  slug: alphaai-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-calendar-api-openapi.yml
- filename: alphaai-news-api-openapi.yml
  format: yaml
  label: AlphaAI News API
  slug: alphaai-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-news-api-openapi.yml
- filename: alphaai-symbols-api-openapi.yml
  format: yaml
  label: AlphaAI Symbols API
  slug: alphaai-symbols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/openapi/alphaai-symbols-api-openapi.yml
authorization_urls:
- https://mcp.alphai.io/oauth/authorize
description: AlphaAI's OAuth surface belongs to the MCP server, not the REST API. The REST OpenAPI declares only a bearer API key and no oauth2 scheme, so the mechanical derive pass (derive-oauth-scopes.py) correctly found nothing. The scopes below were read from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata on the MCP host — both anonymous, both 200.
docs: https://alphai.io/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Alphaai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AlphaAI publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AlphaAI API on a user''s behalf.


  Tokens are issued from https://mcp.alphai.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AlphaAI
provider_slug: alphaai
schemes:
- dynamic_client_registration:
    note: Public clients with no pre-registration — the shape MCP clients need to connect from a browser without the user ever creating an OAuth app.
    registration_endpoint: https://mcp.alphai.io/oauth/register
    spec: RFC 7591
    supported: true
    token_endpoint_auth_methods_supported:
    - none
  flows:
  - authorizationUrl: https://mcp.alphai.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refresh: true
    tokenUrl: https://mcp.alphai.io/oauth/token
  introspection_endpoint: https://mcp.alphai.io/oauth/introspect
  issuer: https://mcp.alphai.io
  name: MCP OAuth 2.1
  revocation_endpoint: https://mcp.alphai.io/oauth/revoke
  source: well-known/alphaai-oauth-authorization-server.json
scope_count: 2
scope_names:
- tools.read
- tools.bulk
scopes:
- description: Read access to the MCP tool surface. Advertised by both the authorization server and the protected-resource metadata. The provider publishes no per-scope reference page, so this description is inferred from the scope name and the read-only character of every tool except the alerts pair.
  flows:
  - authorizationCode
  scope: tools.read
- description: Advertised alongside tools.read on both metadata documents. Its exact semantics are not documented anywhere on the provider's public surface — the name suggests higher-volume or batched tool invocation, but that is not asserted here. Determining it would require authenticated introspection.
  flows:
  - authorizationCode
  scope: tools.bulk
slug: alphaai-scopes
source_filename: alphaai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://mcp.alphai.io/.well-known/oauth-authorization-server\ndocs: https://alphai.io/mcp\ndescription: >-\n  AlphaAI's OAuth surface belongs to the MCP server, not the REST API. The REST\n  OpenAPI declares only a bearer API key and no oauth2 scheme, so the mechanical\n  derive pass (derive-oauth-scopes.py) correctly found nothing. The scopes below\n  were read from the live RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata on the MCP host — both anonymous, both 200.\n\napplies_to: https://mcp.alphai.io/mcp\nnot_applicable_to: >-\n  https://api.alphai.io — the REST API authenticates with a static\n  `ak_live_` bearer key and has no scope model at all.\n\nschemes:\n  - name: MCP OAuth 2.1\n    source: well-known/alphaai-oauth-authorization-server.json\n    issuer: https://mcp.alphai.io\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.alphai.io/oauth/authorize\n\
  \        tokenUrl: https://mcp.alphai.io/oauth/token\n        pkce: S256\n        refresh: true\n    dynamic_client_registration:\n      supported: true\n      spec: RFC 7591\n      registration_endpoint: https://mcp.alphai.io/oauth/register\n      token_endpoint_auth_methods_supported: [none]\n      note: >-\n        Public clients with no pre-registration — the shape MCP clients need to\n        connect from a browser without the user ever creating an OAuth app.\n    revocation_endpoint: https://mcp.alphai.io/oauth/revoke\n    introspection_endpoint: https://mcp.alphai.io/oauth/introspect\n\nscopes:\n  - scope: tools.read\n    description: >-\n      Read access to the MCP tool surface. Advertised by both the authorization\n      server and the protected-resource metadata. The provider publishes no\n      per-scope reference page, so this description is inferred from the scope\n      name and the read-only character of every tool except the alerts pair.\n    flows: [authorizationCode]\n\
  \    sources: [well-known/alphaai-oauth-authorization-server.json, well-known/alphaai-oauth-protected-resource.json]\n  - scope: tools.bulk\n    description: >-\n      Advertised alongside tools.read on both metadata documents. Its exact\n      semantics are not documented anywhere on the provider's public surface —\n      the name suggests higher-volume or batched tool invocation, but that is not\n      asserted here. Determining it would require authenticated introspection.\n    flows: [authorizationCode]\n    sources: [well-known/alphaai-oauth-authorization-server.json, well-known/alphaai-oauth-protected-resource.json]\n\nscope_count: 2\n\ngaps:\n  - >-\n    No scopes reference page exists. The scopes are discoverable only by reading\n    the .well-known metadata directly, which means a human integrator following\n    the docs never learns they exist.\n  - >-\n    The alert-mutating tools (alphai_alerts_subscribe / _unsubscribe) are the\n    only writes in the product, but no write-shaped\
  \ scope is advertised. Either\n    tools.read covers them — which would be a scope-naming problem — or the\n    authorization decision is made on plan tier rather than scope. The docs say\n    the alert tools are gated on a Basic/Pro plan, which points at the latter.\n\nrelated:\n  authentication: authentication/alphaai-authentication.yml\n  mcp: mcp/alphaai-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaai/refs/heads/main/scopes/alphaai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Financial News
- Stock Market
- SEC Filings
- Insider Trading
- Fintech
- Market Data
- Sentiment
- AI Agents
- MCP
- LLM
- Trading
token_urls:
- https://mcp.alphai.io/oauth/token
---
