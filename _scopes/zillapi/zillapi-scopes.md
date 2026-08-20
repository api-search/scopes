---
api_specs:
- filename: zillapi-account-api-openapi.yml
  format: yaml
  label: Zillapi Account API
  slug: zillapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-account-api-openapi.yml
- filename: zillapi-buildings-api-openapi.yml
  format: yaml
  label: Zillapi Buildings API
  slug: zillapi-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-buildings-api-openapi.yml
- filename: zillapi-jobs-api-openapi.yml
  format: yaml
  label: Zillapi Jobs API
  slug: zillapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-jobs-api-openapi.yml
- filename: zillapi-listings-api-openapi.yml
  format: yaml
  label: Zillapi Listings API
  slug: zillapi-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-listings-api-openapi.yml
- filename: zillapi-properties-api-openapi.yml
  format: yaml
  label: Zillapi Properties API
  slug: zillapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-properties-api-openapi.yml
- filename: zillapi-search-api-openapi.yml
  format: yaml
  label: Zillapi Search API
  slug: zillapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-search-api-openapi.yml
- filename: zillapi-webhooks-api-openapi.yml
  format: yaml
  label: Zillapi Webhooks API
  slug: zillapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-webhooks-api-openapi.yml
authorization_urls:
- https://api.zillapi.com/oauth/authorize
description: ''
docs: https://zillapi.com/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zillapi Scopes
name_suffix: OAuth Scopes
note: Not derivable from the OpenAPI — openapi/zillapi-openapi-original.json declares only the `bearerAuth` http scheme. The OAuth 2.1 surface and its single scope are published in the RFC 8414 authorization server metadata and the RFC 9728 protected resource metadata, both harvested to well-known/.
overview: 'Zillapi publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zillapi API on a user''s behalf.


  Tokens are issued from https://api.zillapi.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zillapi
provider_slug: zillapi
schemes:
- flows:
  - authorizationUrl: https://api.zillapi.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.zillapi.com/oauth/token
  issuer: https://api.zillapi.com
  name: oauth2
  source: well-known/zillapi-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:access
scopes:
- description: The single scope Zillapi issues. Grants an agent access to the hosted MCP server at https://api.zillapi.com/mcp and the same /v1 REST surface a long-lived API key reaches; both auth paths bill against the same account.
  flows:
  - authorizationCode
  scope: mcp:access
slug: zillapi-scopes
source_filename: zillapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://zillapi.com/.well-known/oauth-authorization-server\ndocs: https://zillapi.com/auth.md\nnote: >-\n  Not derivable from the OpenAPI — openapi/zillapi-openapi-original.json declares only the `bearerAuth`\n  http scheme. The OAuth 2.1 surface and its single scope are published in the RFC 8414 authorization\n  server metadata and the RFC 9728 protected resource metadata, both harvested to well-known/.\nschemes:\n  - name: oauth2\n    source: well-known/zillapi-oauth-authorization-server.json\n    issuer: https://api.zillapi.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.zillapi.com/oauth/authorize\n        tokenUrl: https://api.zillapi.com/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp:access\n    description: >-\n      The single scope Zillapi issues. Grants an agent access to the hosted MCP server at\n      https://api.zillapi.com/mcp and the same /v1 REST surface a long-lived\
  \ API key reaches; both auth\n      paths bill against the same account.\n    flows: [authorizationCode]\n    sources:\n      - well-known/zillapi-oauth-authorization-server.json\n      - well-known/zillapi-oauth-protected-resource.json\n      - well-known/zillapi-mcp-server-card.json\nmodel:\n  granularity: coarse\n  notes: >-\n    A single all-or-nothing scope — there is no read/write split and no per-resource scoping. An agent\n    granted mcp:access can reach every /v1 operation, including webhook creation and revocation.\n    Credit balance and plan, not scope, are what bound what a token can spend.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/scopes/zillapi-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Real-Estate
- PropTech
- Property Data
- Zillow
- Zestimate
- Valuation
- AVM
- Listings
- MCP
- AI Agent
- REST API
token_urls:
- https://api.zillapi.com/oauth/token
---
