---
api_specs:
- filename: brand-api-brands-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Brands API
  slug: brand-api-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-brands-api-openapi.yml
- filename: brand-api-context-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Context API
  slug: brand-api-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-context-api-openapi.yml
- filename: brand-api-search-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Search API
  slug: brand-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-search-api-openapi.yml
- filename: brand-api-viewer-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Viewer API
  slug: brand-api-viewer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-viewer-api-openapi.yml
authorization_urls:
- https://developers.brandfetch.com/oauth/authorize
description: ''
docs: https://docs.brandfetch.com/mcp/overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Brand Api Scopes
name_suffix: OAuth Scopes
note: 'Brandfetch''s OpenAPI declares no oauth2 security scheme — the REST API is bearer API-key only — so derive-oauth-scopes.py correctly found nothing. The OAuth surface exists solely for the MCP server, and its scope model is published anonymously in the RFC 8414 authorization-server metadata. Exactly one scope is advertised. Read-only is the whole authorization model: there is no write scope because the public product has no write surface.'
overview: 'Brand API (Brandfetch) publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brand API (Brandfetch) API on a user''s behalf.


  Tokens are issued from https://developers.brandfetch.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brand API (Brandfetch)
provider_slug: brand-api
schemes:
- applies_to: https://mcp.brandfetch.io/mcp
  flows:
  - authorizationUrl: https://developers.brandfetch.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://developers.brandfetch.com/api/oauth/register
    response_types:
    - code
    tokenUrl: https://developers.brandfetch.com/api/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://developers.brandfetch.com
  name: brandfetch-mcp-oauth
  source: https://developers.brandfetch.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 1
scope_names:
- read
scopes:
- description: Read access to Brandfetch brand data through the MCP server. The only scope advertised in scopes_supported; it covers every MCP tool (brand_search, get_brand, get_brand_context, enrich_transaction, build_logo_urls, get_asset_base64, send_feedback).
  flows:
  - authorizationCode
  scope: read
slug: brand-api-scopes
source_filename: brand-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://developers.brandfetch.com/.well-known/oauth-authorization-server\ndocs: https://docs.brandfetch.com/mcp/overview\nnote: >-\n  Brandfetch's OpenAPI declares no oauth2 security scheme — the REST API is bearer\n  API-key only — so derive-oauth-scopes.py correctly found nothing. The OAuth surface\n  exists solely for the MCP server, and its scope model is published anonymously in the\n  RFC 8414 authorization-server metadata. Exactly one scope is advertised. Read-only is\n  the whole authorization model: there is no write scope because the public product has\n  no write surface.\nschemes:\n  - name: brandfetch-mcp-oauth\n    type: oauth2\n    source: https://developers.brandfetch.com/.well-known/oauth-authorization-server\n    issuer: https://developers.brandfetch.com\n    applies_to: https://mcp.brandfetch.io/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://developers.brandfetch.com/oauth/authorize\n\
  \        tokenUrl: https://developers.brandfetch.com/api/oauth/token\n        registrationUrl: https://developers.brandfetch.com/api/oauth/register\n        pkce: [S256]\n        token_endpoint_auth_methods: [none]\n        response_types: [code]\nscopes:\n  - scope: read\n    description: >-\n      Read access to Brandfetch brand data through the MCP server. The only scope\n      advertised in scopes_supported; it covers every MCP tool (brand_search, get_brand,\n      get_brand_context, enrich_transaction, build_logo_urls, get_asset_base64,\n      send_feedback).\n    flows: [authorizationCode]\n    sources: [https://developers.brandfetch.com/.well-known/oauth-authorization-server]\nnon_oauth_credentials:\n  - {name: API key, transport: 'Authorization: Bearer <key>', scoped: false,\n     applies_to: [Brand API, Brand Context API, Transaction API, Viewer API]}\n  - {name: MCP token, prefix: 'bf1.', transport: 'Authorization: Bearer <token>', scoped: false,\n     applies_to: [MCP server],\
  \ note: 'Non-interactive alternative to the OAuth flow.'}\n  - {name: Client ID, transport: '?c=<client_id> query parameter', scoped: false,\n     applies_to: [Logo API, Brand Search API], note: 'Public, embeddable, not a secret.'}\nx-evidence:\n  fetched: '2026-08-14'\n  url: https://developers.brandfetch.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  file: ../well-known/brand-api-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/scopes/brand-api-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Brands
- Logos
- Brand Assets
- Company Data
- Firmographics
- Brand Context
- Merchant Enrichment
- Agent Tools
token_urls:
- https://developers.brandfetch.com/api/oauth/token
---
