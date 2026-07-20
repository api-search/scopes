---
authorization_urls:
- https://forge.era.app/oauth/authorize
description: ''
docs: https://era.app/help/mcp-server-era-context
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Era Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Era publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Era API on a user''s behalf.


  Tokens are issued from https://forge.era.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Era
provider_slug: era
schemes:
- flows:
  - authorizationUrl: https://forge.era.app/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://forge.era.app/oauth/register
    tokenUrl: https://forge.era.app/oauth/token
  name: OAuth2
  source: https://context.era.app/.well-known/oauth-authorization-server
scope_count: 10
scope_names:
- mcp:discovery
- mcp:tools-basic
- mcp:tools-write
- mcp:billing-write
- mcp:resources-read
- offline_access
- banking:read
- banking:write
- social:read
- social:write
scopes:
- description: Discover the Era Context MCP server and its tool catalog
  flows: []
  scope: mcp:discovery
- description: Invoke read-oriented (basic) MCP tools
  flows: []
  scope: mcp:tools-basic
- description: Invoke write-capable MCP tools (account/transaction modifications)
  flows: []
  scope: mcp:tools-write
- description: Perform billing changes (subscription upgrade/cancel/manage); required separately from other write scopes and gated by extra consent
  flows: []
  scope: mcp:billing-write
- description: Read MCP resources exposed by the server
  flows: []
  scope: mcp:resources-read
- description: Obtain a refresh token for long-lived, offline agent access
  flows: []
  scope: offline_access
- description: Read connected banking data (balances, accounts, transactions)
  flows: []
  scope: banking:read
- description: Modify banking-related data (rules, categories, transaction fields, transfer links)
  flows: []
  scope: banking:write
- description: Read social/referral program data
  flows: []
  scope: social:read
- description: Modify social/referral program data
  flows: []
  scope: social:write
slug: era-scopes
source_filename: era-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://context.era.app/.well-known/oauth-protected-resource\ndocs: https://era.app/help/mcp-server-era-context\nauthorization_server: https://forge.era.app\nschemes:\n- name: OAuth2\n  source: https://context.era.app/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://forge.era.app/oauth/authorize\n    tokenUrl: https://forge.era.app/oauth/token\n    registrationUrl: https://forge.era.app/oauth/register\n    pkce: S256\nscopes:\n- scope: mcp:discovery\n  description: Discover the Era Context MCP server and its tool catalog\n- scope: mcp:tools-basic\n  description: Invoke read-oriented (basic) MCP tools\n- scope: mcp:tools-write\n  description: Invoke write-capable MCP tools (account/transaction modifications)\n- scope: mcp:billing-write\n  description: Perform billing changes (subscription upgrade/cancel/manage); required\n    separately from other write scopes and gated\
  \ by extra consent\n- scope: mcp:resources-read\n  description: Read MCP resources exposed by the server\n- scope: offline_access\n  description: Obtain a refresh token for long-lived, offline agent access\n- scope: banking:read\n  description: Read connected banking data (balances, accounts, transactions)\n- scope: banking:write\n  description: Modify banking-related data (rules, categories, transaction fields, transfer links)\n- scope: social:read\n  description: Read social/referral program data\n- scope: social:write\n  description: Modify social/referral program data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/era/refs/heads/main/scopes/era-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Company
- Fintech
- Artificial Intelligence
- Personal Finance
- Wealth Management
- Model Context Protocol
- MCP
- Agent Native
- Open Banking
- OAuth
token_urls:
- https://forge.era.app/oauth/token
---
