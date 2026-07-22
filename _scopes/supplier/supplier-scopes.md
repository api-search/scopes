---
authorization_urls:
- https://supplier.io/authorize
description: ''
docs: https://royalplugins.com/support/royal-mcp/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Supplier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Supplier publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Supplier API on a user''s behalf.


  Tokens are issued from https://supplier.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Supplier
provider_slug: supplier
schemes:
- flows:
  - authorizationUrl: https://supplier.io/authorize
    flow: authorizationCode
    tokenUrl: https://supplier.io/token
  name: OAuth2
  source: well-known/supplier-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:full
scopes:
- description: Full access to the Royal MCP server tools exposed at supplier.io/wp-json/royal-mcp/v1
  flows:
  - authorizationCode
  scope: mcp:full
slug: supplier-scopes
source_filename: supplier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://supplier.io/.well-known/oauth-authorization-server\ndocs: https://royalplugins.com/support/royal-mcp/\nschemes:\n- name: OAuth2\n  source: well-known/supplier-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://supplier.io/authorize\n    tokenUrl: https://supplier.io/token\nscopes:\n- scope: 'mcp:full'\n  description: Full access to the Royal MCP server tools exposed at supplier.io/wp-json/royal-mcp/v1\n  flows: [authorizationCode]\n  sources: ['well-known/supplier-oauth-authorization-server.json']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supplier/refs/heads/main/scopes/supplier-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Procurement
- Supply Chain
- Supplier Diversity
- Spend Analytics
- Sourcing
- ESG
- Sustainability
- MCP
token_urls:
- https://supplier.io/token
---
