---
api_specs:
- filename: recurrency-openapi.yml
  format: yaml
  label: Recurrency API
  slug: recurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/openapi/recurrency-openapi.yml
authorization_urls:
- https://login.recurrency.ai/authorize
description: ''
docs: https://recurrency.gitbook.io/recurrency/authentication/getting-an-access-token
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Recurrency Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Recurrency publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Recurrency API on a user''s behalf.


  Tokens are issued from https://api.recurrency.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Recurrency
provider_slug: recurrency
schemes:
- description: 'OAuth 2.0 client-credentials for the e-procurement REST API. POST to the token endpoint with grant_type=client_credentials plus client_id/client_secret to receive a Bearer access token, valid for 7 days (604800 seconds). Send it as `authorization: Bearer {token}`.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.recurrency.com/oauth/token
  name: oauth2-api
  source: openapi/recurrency-openapi.yml
- description: Auth0-backed authorization-code + PKCE (S256) flow securing the hosted MCP server (api.recurrency.com/mcp, protected resource core-api.recurrency.ai).
  flows:
  - authorizationUrl: https://login.recurrency.ai/authorize
    flow: authorizationCode
    tokenUrl: https://login.recurrency.ai/oauth/token
  name: oauth2-mcp
  source: well-known/recurrency-oauth-authorization-server.json
scope_count: 4
scope_names:
- recurrency:api:tenant
- recurrency:mcp:tenant:read
- recurrency:mcp:tenant:write
- recurrency:mcp:admin
scopes:
- description: Tenant-scoped access to the Recurrency e-procurement REST API.
  flows:
  - clientCredentials
  scope: recurrency:api:tenant
- description: Read access to tenant data via the Recurrency MCP server.
  flows:
  - authorizationCode
  scope: recurrency:mcp:tenant:read
- description: Write access to tenant data via the Recurrency MCP server.
  flows:
  - authorizationCode
  scope: recurrency:mcp:tenant:write
- description: Administrative access via the Recurrency MCP server.
  flows:
  - authorizationCode
  scope: recurrency:mcp:admin
slug: recurrency-scopes
source_filename: recurrency-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/recurrency-openapi.yml\ndocs: https://recurrency.gitbook.io/recurrency/authentication/getting-an-access-token\nschemes:\n  - name: oauth2-api\n    source: openapi/recurrency-openapi.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.recurrency.com/oauth/token\n    description: >-\n      OAuth 2.0 client-credentials for the e-procurement REST API. POST to the\n      token endpoint with grant_type=client_credentials plus\n      client_id/client_secret to receive a Bearer access token, valid for 7 days\n      (604800 seconds). Send it as `authorization: Bearer {token}`.\n  - name: oauth2-mcp\n    source: well-known/recurrency-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.recurrency.ai/authorize\n        tokenUrl: https://login.recurrency.ai/oauth/token\n    description: >-\n      Auth0-backed authorization-code + PKCE (S256)\
  \ flow securing the hosted MCP\n      server (api.recurrency.com/mcp, protected resource core-api.recurrency.ai).\nscopes:\n  - scope: recurrency:api:tenant\n    description: Tenant-scoped access to the Recurrency e-procurement REST API.\n    flows: [clientCredentials]\n    sources: [openapi/recurrency-openapi.yml]\n  - scope: recurrency:mcp:tenant:read\n    description: Read access to tenant data via the Recurrency MCP server.\n    flows: [authorizationCode]\n    sources: [well-known/recurrency-oauth-authorization-server.json]\n  - scope: recurrency:mcp:tenant:write\n    description: Write access to tenant data via the Recurrency MCP server.\n    flows: [authorizationCode]\n    sources: [well-known/recurrency-oauth-authorization-server.json]\n  - scope: recurrency:mcp:admin\n    description: Administrative access via the Recurrency MCP server.\n    flows: [authorizationCode]\n    sources: [well-known/recurrency-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/scopes/recurrency-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Company
- Ai Ml
- ERP
- Distribution
- Wholesale
- E-Procurement
- Supply Chain
- Orders
token_urls:
- https://api.recurrency.com/oauth/token
- https://login.recurrency.ai/oauth/token
---
