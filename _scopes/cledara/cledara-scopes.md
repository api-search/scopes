---
api_specs:
- filename: cledara-api-openapi.json
  format: json
  label: Cledara API
  slug: cledara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-api-openapi.json
authorization_urls: []
description: OAuth scopes Cledara publishes. Exactly one, and it belongs to the market-data MCP endpoint, not to the workspace REST API — that surface authenticates with an unscoped Bearer API key that inherits the creating user's full permissions and therefore has no scope vocabulary at all.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cledara Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cledara uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cledara
provider_slug: cledara
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cledara-scopes
source_filename: cledara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://data.cledara.com/.well-known/oauth-authorization-server\nprovider: Cledara\nproviderId: cledara\ndescription: >-\n  OAuth scopes Cledara publishes. Exactly one, and it belongs to the market-data MCP\n  endpoint, not to the workspace REST API — that surface authenticates with an unscoped\n  Bearer API key that inherits the creating user's full permissions and therefore has no\n  scope vocabulary at all.\napi: Cledara SaaS Market Data Hub MCP Server\nauthorization_server: https://data.cledara.com\nflows:\n  - type: authorization_code\n    authorizationUrl: https://data.cledara.com/authorize\n    tokenUrl: https://data.cledara.com/oauth/token\n    pkce: S256\n  - type: client_credentials\n    tokenUrl: https://data.cledara.com/oauth/token\nscopes:\n  - name: 'mcp:read'\n    description: >-\n      Read access to the Cledara SaaS Market Data Hub through the MCP endpoint at\n      https://data.cledara.com/mcp. Declared in scopes_supported\
  \ of the RFC 8414\n      authorization-server metadata; Cledara publishes no prose scope reference, so the\n      description here is derived from the scope name plus the endpoint it guards.\n    grants: read\n    surface: https://data.cledara.com/mcp\nscope_count: 1\ndocs: null\nnotes:\n  - No write scope is published, which is consistent with a read-only public dataset.\n  - No scope reference page exists on the provider's site; the authorization-server\n    metadata document is the only published source.\n  - The REST API at api.cledara.com declares only an http/bearer securityScheme and\n    therefore contributes no scopes.\nmaintainers:\n  - FN: Kin Lane\n    email: kinlane@gmail.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/scopes/cledara-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Finance
- SaaS Management
- Software Spending
- Spend Management
- Subscription Management
- Virtual Cards
- Expense Management
- FinOps
- MCP
- Market Data
token_urls: []
---
