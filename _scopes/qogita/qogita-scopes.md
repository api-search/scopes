---
authorization_urls:
- https://api.qogita.com/staff/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Qogita Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Qogita publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Qogita API on a user''s behalf.


  Tokens are issued from https://api.qogita.com/staff/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Qogita
provider_slug: qogita
schemes:
- flows:
  - authorizationUrl: https://api.qogita.com/staff/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.qogita.com/staff/oauth/token
  name: OAuth2
  source: well-known/qogita-oauth-authorization-server.json
scope_count: 1
scope_names:
- staff:mcp
scopes:
- description: Access to the Qogita Staff MCP server (Production).
  flows:
  - authorizationCode
  scope: staff:mcp
slug: qogita-scopes
source_filename: qogita-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.qogita.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/qogita-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.qogita.com/staff/oauth/authorize\n    tokenUrl: https://api.qogita.com/staff/oauth/token\nscopes:\n- scope: staff:mcp\n  description: Access to the Qogita Staff MCP server (Production).\n  flows: [authorizationCode]\n  sources: [well-known/qogita-oauth-authorization-server.json]\nnotes: >-\n  Single scope advertised by the authorization server metadata. This scope\n  governs the hosted MCP resource; Qogita's public REST API does not publish a\n  machine-readable scope reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qogita/refs/heads/main/scopes/qogita-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Ecommerce
- Wholesale
- Marketplace
- Health and Beauty
- B2B
- Retail
- Distribution
token_urls:
- https://api.qogita.com/staff/oauth/token
---
