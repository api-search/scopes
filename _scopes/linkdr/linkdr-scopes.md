---
api_specs:
- filename: linkdr-admin-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP Admin MCP API
  slug: linkdr-admin-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-admin-mcp-api-openapi.yml
- filename: linkdr-agent-resources-api-openapi.yml
  format: yaml
  label: LinkDR MCP Agent resources API
  slug: linkdr-agent-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-agent-resources-api-openapi.yml
- filename: linkdr-mcp-api-openapi.yml
  format: yaml
  label: LinkDR MCP MCP API
  slug: linkdr-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-mcp-api-openapi.yml
- filename: linkdr-public-data-api-openapi.yml
  format: yaml
  label: LinkDR MCP Public data API
  slug: linkdr-public-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-public-data-api-openapi.yml
- filename: linkdr-system-api-openapi.yml
  format: yaml
  label: LinkDR MCP System API
  slug: linkdr-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkdr/openapi/linkdr-system-api-openapi.yml
authorization_urls:
- /api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: LinkDR MCP Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LinkDR MCP publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LinkDR MCP API on a user''s behalf.


  Tokens are issued from /api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LinkDR MCP
provider_slug: linkdr
schemes:
- description: 'OAuth 2.1 authorization-code flow with PKCE (required) for both MCP servers. Authorization server metadata: https://linkdr.com/.well-known/oauth-authorization-server. Dynamic client registration is accepted. Each server is its own protected resource (https://linkdr.com/mcp and https://linkdr.com/mcp/admin), so a token is audience-bound to one of them. The admin server also requires the admin role on the LinkDR account.'
  flows:
  - authorizationUrl: /api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /api/auth/oauth2/token
  name: McpOAuth
  source: openapi/linkdr-openapi.json
scope_count: 4
scope_names:
- email
- offline_access
- openid
- profile
scopes:
- description: Identify the account by email address during sign-in
  flows:
  - authorizationCode
  scope: email
- description: Receive a refresh token so long-running agent sessions stay connected until revoked
  flows:
  - authorizationCode
  scope: offline_access
- description: Sign in with a LinkDR account
  flows:
  - authorizationCode
  scope: openid
- description: Read the account display name
  flows:
  - authorizationCode
  scope: profile
slug: linkdr-scopes
source_filename: linkdr-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/linkdr-openapi.json\nschemes:\n- name: McpOAuth\n  source: openapi/linkdr-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /api/auth/oauth2/authorize\n    tokenUrl: /api/auth/oauth2/token\n  description: 'OAuth 2.1 authorization-code flow with PKCE (required) for both MCP servers.\n    Authorization server metadata: https://linkdr.com/.well-known/oauth-authorization-server.\n    Dynamic client registration is accepted. Each server is its own protected resource (https://linkdr.com/mcp\n    and https://linkdr.com/mcp/admin), so a token is audience-bound to one of them. The admin\n    server also requires the admin role on the LinkDR account.'\nscopes:\n- scope: email\n  description: Identify the account by email address during sign-in\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkdr-openapi.json\n- scope: offline_access\n  description: Receive a refresh token so long-running agent\
  \ sessions stay connected until revoked\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkdr-openapi.json\n- scope: openid\n  description: Sign in with a LinkDR account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkdr-openapi.json\n- scope: profile\n  description: Read the account display name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/linkdr-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/linkdr/scopes/linkdr-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- SEO
- Backlink
- Artificial Intelligence
- Software-as-a-Service
token_bound: false
token_urls:
- /api/auth/oauth2/token
---
