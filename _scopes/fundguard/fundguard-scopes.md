---
authorization_urls:
- https://www.fundguard.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Fundguard Scopes
name_suffix: OAuth Scopes
note: Derived from published OAuth metadata rather than an OpenAPI (FundGuard publishes no spec). The authorization server advertises exactly one scope. No scopes/permissions reference page exists on any public FundGuard host; nothing beyond the advertised value is recorded.
overview: 'FundGuard publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FundGuard API on a user''s behalf.


  Tokens are issued from https://www.fundguard.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FundGuard
provider_slug: fundguard
schemes:
- flows:
  - authorizationUrl: https://www.fundguard.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.fundguard.com/oauth/token
  name: mcp-oauth
  source: well-known/fundguard-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the MCP server exposed at https://www.fundguard.com/wp-json/mcp/mcp-oauth-server. The scope is advertised in both scopes_supported of the authorization-server metadata and scopes_supported of the protected-resource metadata. No finer-grained scope decomposition is published.
  flows:
  - authorizationCode
  scope: mcp
slug: fundguard-scopes
source_filename: fundguard-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://www.fundguard.com/.well-known/oauth-authorization-server\nnote: >-\n  Derived from published OAuth metadata rather than an OpenAPI (FundGuard publishes no spec). The\n  authorization server advertises exactly one scope. No scopes/permissions reference page exists on any\n  public FundGuard host; nothing beyond the advertised value is recorded.\nschemes:\n- name: mcp-oauth\n  source: well-known/fundguard-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fundguard.com/oauth/authorize\n    tokenUrl: https://www.fundguard.com/oauth/token\nscopes:\n- scope: mcp\n  description: >-\n    Access the MCP server exposed at https://www.fundguard.com/wp-json/mcp/mcp-oauth-server. The scope is\n    advertised in both scopes_supported of the authorization-server metadata and scopes_supported of the\n    protected-resource metadata. No finer-grained scope decomposition is published.\n\
  \  flows: [authorizationCode]\n  sources:\n  - well-known/fundguard-oauth-authorization-server.json\n  - well-known/fundguard-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://www.fundguard.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundguard/refs/heads/main/scopes/fundguard-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- investment-accounting
- Fund Accounting
- ibor
- abor
- NAV
- Asset Management
- portfolio-accounting
- Private Markets
- Financial-Services
- Fintech
- Software-as-a-Service
- Artificial Intelligence
- MCP
token_urls:
- https://www.fundguard.com/oauth/token
---
