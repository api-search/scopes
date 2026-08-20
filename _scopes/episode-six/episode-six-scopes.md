---
authorization_urls:
- https://docs.episodesix.com/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Episode Six Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Episode Six publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Episode Six API on a user''s behalf.


  Tokens are issued from https://docs.episodesix.com/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Episode Six
provider_slug: episode-six
schemes:
- applies_to: https://docs.episodesix.com/mcp
  flows:
  - authorizationUrl: https://docs.episodesix.com/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docs.episodesix.com/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docs.episodesix.com/mcp/oauth/token
  issuer: https://docs.episodesix.com/mcp/oauth
  name: MCPOAuth2
  source: well-known/episode-six-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp:search
scopes:
- description: Search the Episode Six TRITIUM developer documentation through the MCP server. This is the single scope advertised in scopes_supported; it bounds the MCP surface to documentation retrieval and grants no access to the payments platform.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:search
slug: episode-six-scopes
source_filename: episode-six-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://docs.episodesix.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  No public scopes or permissions reference exists. The only scope Episode Six publishes\n  anywhere on a public surface is the one advertised in its MCP OAuth authorization-server\n  metadata. The TRITIUM platform API scope model, if it has one, is behind the docs gate.\nschemes:\n- name: MCPOAuth2\n  source: well-known/episode-six-oauth-authorization-server.json\n  issuer: https://docs.episodesix.com/mcp/oauth\n  applies_to: https://docs.episodesix.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs.episodesix.com/mcp/oauth/authorize\n    tokenUrl: https://docs.episodesix.com/mcp/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://docs.episodesix.com/mcp/oauth/token\nscopes:\n- scope: mcp:search\n  description: >-\n    Search the Episode Six TRITIUM developer documentation through the MCP\
  \ server. This is\n    the single scope advertised in scopes_supported; it bounds the MCP surface to\n    documentation retrieval and grants no access to the payments platform.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/episode-six-oauth-authorization-server.json\nscope_count: 1\nx-evidence:\n  fetched: '2026-08-12'\n  url: https://docs.episodesix.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/episode-six/refs/heads/main/scopes/episode-six-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Payments
- Card Issuing
- Issuer Processing
- Ledger
- Banking
- Financial-Services
- Embedded Finance
- Fintech
- Virtual Accounts
- Virtual Cards
- Credit
- Prepaid
- Multi-Currency
token_urls:
- https://docs.episodesix.com/mcp/oauth/token
---
