---
authorization_urls:
- https://www.spocket.dev/oauth/authorize
description: ''
docs: https://www.spocket.dev/documentation/platform-api
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Spocket Scopes
name_suffix: OAuth Scopes
note: Two independent OAuth surfaces with two independent scope vocabularies. The MCP scope set comes from the live RFC 8414 authorization-server metadata; the Platform API scope set comes from the provider's published scope table. Spocket publishes no OpenAPI, so derive-oauth-scopes.py has no securitySchemes to read - these are searched, not derived.
overview: 'Spocket publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spocket API on a user''s behalf.


  Tokens are issued from https://www.spocket.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spocket
provider_slug: spocket
schemes:
- flows:
  - authorizationUrl: https://www.spocket.dev/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    tokenUrl: https://www.spocket.dev/oauth/token
  name: MCPOAuth21
  source: well-known/spocket-oauth-authorization-server.json
  surface: https://www.spocket.dev/api/mcp
- flows:
  - flow: clientCredentials
    tokenUrl: https://www.spocket.dev/api/v1/token
  name: PlatformClientCredentials
  source: https://www.spocket.dev/documentation/platform-api
  surface: https://www.spocket.dev/api/v1
scope_count: 5
scope_names:
- spocket
- apps:read
- apps:write
- apps:delete
- domains:write
scopes:
- description: The single coarse scope advertised by the MCP authorization server. All 20 MCP tools are covered by it - the provider states no plan or tier gates a tool, and no per-tool or read-only variant is published.
  flows:
  - authorizationCode
  scope: spocket
- description: List apps, read status and logs.
  flows:
  - clientCredentials
  scope: apps:read
- description: Provision, deploy, start, stop, restart.
  flows:
  - clientCredentials
  scope: apps:write
- description: Delete apps.
  flows:
  - clientCredentials
  scope: apps:delete
- description: Attach and verify custom domains.
  flows:
  - clientCredentials
  scope: domains:write
slug: spocket-scopes
source_filename: spocket-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.spocket.dev/documentation/platform-api\ndocs: https://www.spocket.dev/documentation/platform-api\nnote: >-\n  Two independent OAuth surfaces with two independent scope vocabularies. The MCP scope\n  set comes from the live RFC 8414 authorization-server metadata; the Platform API scope\n  set comes from the provider's published scope table. Spocket publishes no OpenAPI, so\n  derive-oauth-scopes.py has no securitySchemes to read - these are searched, not derived.\nschemes:\n  - name: MCPOAuth21\n    source: well-known/spocket-oauth-authorization-server.json\n    surface: https://www.spocket.dev/api/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.spocket.dev/oauth/authorize\n        tokenUrl: https://www.spocket.dev/oauth/token\n        code_challenge_methods_supported: [S256]\n  - name: PlatformClientCredentials\n    source: 'https://www.spocket.dev/documentation/platform-api'\n\
  \    surface: https://www.spocket.dev/api/v1\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://www.spocket.dev/api/v1/token\nscopes:\n  - scope: spocket\n    description: >-\n      The single coarse scope advertised by the MCP authorization server. All 20 MCP tools\n      are covered by it - the provider states no plan or tier gates a tool, and no\n      per-tool or read-only variant is published.\n    flows: [authorizationCode]\n    surface: mcp\n    sources: [well-known/spocket-oauth-authorization-server.json]\n  - scope: apps:read\n    description: List apps, read status and logs.\n    flows: [clientCredentials]\n    surface: platform-rest\n    sources: ['https://www.spocket.dev/documentation/platform-api']\n  - scope: apps:write\n    description: Provision, deploy, start, stop, restart.\n    flows: [clientCredentials]\n    surface: platform-rest\n    sources: ['https://www.spocket.dev/documentation/platform-api']\n  - scope: apps:delete\n    description: Delete\
  \ apps.\n    flows: [clientCredentials]\n    surface: platform-rest\n    sources: ['https://www.spocket.dev/documentation/platform-api']\n  - scope: domains:write\n    description: Attach and verify custom domains.\n    flows: [clientCredentials]\n    surface: platform-rest\n    sources: ['https://www.spocket.dev/documentation/platform-api']\nobservations:\n  - >-\n    domains:write is a published scope with no corresponding endpoint in the published\n    Platform API endpoint table - the capability is scoped but not documented.\n  - >-\n    The MCP surface has one scope covering every tool including the destructive\n    spocket_delete, so an MCP consent grant cannot be narrowed the way a Platform API key\n    can be at creation.\nx-evidence:\n  fetched: '2026-08-09'\n  probed:\n    - url: https://www.spocket.dev/.well-known/oauth-authorization-server\n      status: 200\n    - url: https://www.spocket.dev/documentation/platform-api\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spocket/refs/heads/main/scopes/spocket-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- PaaS
- application-hosting
- bot-hosting
- developer-tools
- agent-infrastructure
- MCP
- deployment
- serverless
- always-on
token_urls:
- https://www.spocket.dev/oauth/token
- https://www.spocket.dev/api/v1/token
---
