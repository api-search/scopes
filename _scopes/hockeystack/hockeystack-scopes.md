---
authorization_urls:
- https://hockeystack.com/api/mcp/oauth/authorize
description: ''
docs: https://app.hockeystack.com/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hockeystack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HockeyStack publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HockeyStack API on a user''s behalf.


  Tokens are issued from https://hockeystack.com/api/mcp/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HockeyStack
provider_slug: hockeystack
schemes:
- flows:
  - authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://hockeystack.com/api/mcp/oauth/token
  name: OmniOAuth2
  source: well-known/hockeystack-oauth-authorization-server.json
scope_count: 1
scope_names:
- omni:tools
scopes:
- description: Grants an OAuth client access to the HockeyStack Omni MCP tool surface (revenue/marketing/account intelligence agent tools) on the protected resource https://hockeystack.com/api/mcp/omni.
  flows:
  - authorizationCode
  scope: omni:tools
slug: hockeystack-scopes
source_filename: hockeystack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://app.hockeystack.com/.well-known/oauth-authorization-server\ndocs: https://app.hockeystack.com/.well-known/oauth-protected-resource\nschemes:\n- name: OmniOAuth2\n  source: well-known/hockeystack-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hockeystack.com/api/mcp/oauth/authorize\n    tokenUrl: https://hockeystack.com/api/mcp/oauth/token\nscopes:\n- scope: omni:tools\n  description: >-\n    Grants an OAuth client access to the HockeyStack Omni MCP tool surface\n    (revenue/marketing/account intelligence agent tools) on the protected\n    resource https://hockeystack.com/api/mcp/omni.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/hockeystack-oauth-authorization-server.json\nnotes: >-\n  Only one scope (omni:tools) is advertised in the authorization-server and\n  protected-resource discovery documents. No finer-grained scope reference is\n  published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hockeystack/refs/heads/main/scopes/hockeystack-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Data
- Marketing Analytics
- Attribution
- Revenue Intelligence
- B2B
- Account Intelligence
- MCP
- AI Agents
token_urls:
- https://hockeystack.com/api/mcp/oauth/token
---
