---
api_specs:
- filename: cledara-applications-api-openapi.yml
  format: yaml
  label: Cledara Applications API
  slug: cledara-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-applications-api-openapi.yml
- filename: cledara-transactions-api-openapi.yml
  format: yaml
  label: Cledara Transactions API
  slug: cledara-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-transactions-api-openapi.yml
authorization_urls:
- https://data.cledara.com/authorize
description: OAuth scopes Cledara publishes. Exactly one, and it belongs to the market-data MCP endpoint, not to the workspace REST API — that surface authenticates with an unscoped Bearer API key that inherits the creating user's full permissions and therefore has no scope vocabulary at all.
docs: ''
flows:
- authorization_code
- client_credentials
kind: oauth-scopes
layout: scope
method: probed
name: Cledara Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cledara publishes 1 OAuth 2.0 scope via the authorization_code and client_credentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cledara API on a user''s behalf.


  Tokens are issued from https://data.cledara.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cledara
provider_slug: cledara
schemes: []
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read access to the Cledara SaaS Market Data Hub through the MCP endpoint at https://data.cledara.com/mcp. Declared in scopes_supported of the RFC 8414 authorization-server metadata; Cledara publishes no prose scope reference, so the description here is derived from the scope name plus the endpoint it guards.
  flows: []
  scope: mcp:read
slug: cledara-scopes
source_filename: cledara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://data.cledara.com/.well-known/oauth-authorization-server\nprovider: Cledara\nproviderId: cledara\ndescription: >-\n  OAuth scopes Cledara publishes. Exactly one, and it belongs to the market-data MCP\n  endpoint, not to the workspace REST API — that surface authenticates with an unscoped\n  Bearer API key that inherits the creating user's full permissions and therefore has no\n  scope vocabulary at all.\napi: Cledara SaaS Market Data Hub MCP Server\nauthorization_server: https://data.cledara.com\nflows:\n  - type: authorization_code\n    authorizationUrl: https://data.cledara.com/authorize\n    tokenUrl: https://data.cledara.com/oauth/token\n    pkce: S256\n  - type: client_credentials\n    tokenUrl: https://data.cledara.com/oauth/token\nscopes:\n  - name: 'mcp:read'\n    description: >-\n      Read access to the Cledara SaaS Market Data Hub through the MCP endpoint at\n      https://data.cledara.com/mcp. Declared in scopes_supported\
  \ of the RFC 8414\n      authorization-server metadata; Cledara publishes no prose scope reference, so the\n      description here is derived from the scope name plus the endpoint it guards.\n    grants: read\n    surface: https://data.cledara.com/mcp\nscope_count: 1\ndocs: null\nnotes:\n  - No write scope is published, which is consistent with a read-only public dataset.\n  - No scope reference page exists on the provider's site; the authorization-server\n    metadata document is the only published source.\n  - The REST API at api.cledara.com declares only an http/bearer securityScheme and\n    therefore contributes no scopes.\nmaintainers:\n  - FN: Kin Lane\n    email: kinlane@gmail.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/scopes/cledara-scopes.yml
summary_line: 1 scope · authorization_code/client_credentials
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
token_bound: false
token_urls:
- https://data.cledara.com/oauth/token
---
