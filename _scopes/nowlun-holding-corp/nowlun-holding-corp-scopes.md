---
authorization_urls:
- https://nowlun.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nowlun Holding Corp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nowlun Holding Corp. publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nowlun Holding Corp. API on a user''s behalf.


  Tokens are issued from https://nowlun.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nowlun Holding Corp.
provider_slug: nowlun-holding-corp
schemes:
- flows:
  - authorizationUrl: https://nowlun.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://nowlun.com/oauth/token
  name: OAuth2
  source: well-known/nowlun-holding-corp-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp
- excel
- mind
scopes:
- description: 'Access to Nowlun''s MCP (Model Context Protocol) server at https://nowlun.com/mcp. Verified: the protected-resource metadata lists "mcp" as the required scope for that resource.'
  flows:
  - authorizationCode
  scope: mcp
- description: Scope advertised in scopes_supported. Purpose not documented publicly (no scope reference page published).
  flows:
  - authorizationCode
  scope: excel
- description: Scope advertised in scopes_supported. Purpose not documented publicly (no scope reference page published).
  flows:
  - authorizationCode
  scope: mind
slug: nowlun-holding-corp-scopes
source_filename: nowlun-holding-corp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://nowlun.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/nowlun-holding-corp-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://nowlun.com/oauth/authorize\n    tokenUrl: https://nowlun.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Access to Nowlun's MCP (Model Context Protocol) server at https://nowlun.com/mcp.\n    Verified: the protected-resource metadata lists \"mcp\" as the required scope for that resource.\n  flows: [authorizationCode]\n  sources: [well-known/nowlun-holding-corp-oauth-authorization-server.json]\n- scope: excel\n  description: >-\n    Scope advertised in scopes_supported. Purpose not documented publicly (no scope reference page published).\n  flows: [authorizationCode]\n  sources: [well-known/nowlun-holding-corp-oauth-authorization-server.json]\n- scope: mind\n  description: >-\n    Scope\
  \ advertised in scopes_supported. Purpose not documented publicly (no scope reference page published).\n  flows: [authorizationCode]\n  sources: [well-known/nowlun-holding-corp-oauth-authorization-server.json]\nnotes: >-\n  Scopes captured verbatim from published scopes_supported. Nowlun does not publish a\n  human-readable scope/permission reference page, so descriptions beyond the verified\n  \"mcp\" resource binding are left honestly undocumented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowlun-holding-corp/refs/heads/main/scopes/nowlun-holding-corp-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Logistics
- Freight Forwarding
- Shipping
- Supply Chain
- Sea Freight
- Customs
- MENA
- MCP
token_urls:
- https://nowlun.com/oauth/token
---
