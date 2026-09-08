---
authorization_urls:
- https://mcp.1up.ai/authorize
description: ''
docs: https://help.1up.ai/en/articles/14304740-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 1Up Scopes
name_suffix: OAuth Scopes
note: 1up publishes no OpenAPI, so derive-oauth-scopes.py has nothing to read. The scope list below is the one the provider actually advertises, taken verbatim from both RFC 8414 and RFC 9728 discovery documents on mcp.1up.ai. It is an OpenID Connect-shaped identity scope set only — there is no resource-level or per-tool permission scope. Authorization inside a workspace is enforced by 1up's own RBAC and workspace isolation, not by OAuth scope, so an agent holding a token has whatever the signed-in user has. Nothing more granular is published.
overview: '1up publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 1up API on a user''s behalf.


  Tokens are issued from https://mcp.1up.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 1up
provider_slug: 1up
schemes:
- flows:
  - authorizationUrl: https://mcp.1up.ai/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.1up.ai/token
  name: 1up MCP OAuth 2.1
  source: well-known/1up-oauth-protected-resource.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect identity — issue an ID token for the signed-in 1up user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the signed-in 1up user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the signed-in 1up user.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the MCP client can keep working without re-prompting; the 1up-mcp CLI caches and auto-refreshes credentials in ~/.1up/credentials.json.
  flows:
  - authorizationCode
  scope: offline_access
slug: 1up-scopes
source_filename: 1up-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://mcp.1up.ai/.well-known/oauth-protected-resource\ndocs: https://help.1up.ai/en/articles/14304740-mcp\nnote: >-\n  1up publishes no OpenAPI, so derive-oauth-scopes.py has nothing to read. The scope list\n  below is the one the provider actually advertises, taken verbatim from both RFC 8414 and\n  RFC 9728 discovery documents on mcp.1up.ai. It is an OpenID Connect-shaped identity scope\n  set only — there is no resource-level or per-tool permission scope. Authorization inside\n  a workspace is enforced by 1up's own RBAC and workspace isolation, not by OAuth scope, so\n  an agent holding a token has whatever the signed-in user has. Nothing more granular is\n  published.\nschemes:\n- name: 1up MCP OAuth 2.1\n  source: well-known/1up-oauth-protected-resource.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.1up.ai/authorize\n    tokenUrl: https://mcp.1up.ai/token\nscope_count: 4\nscopes:\n- scope:\
  \ openid\n  description: OpenID Connect identity — issue an ID token for the signed-in 1up user.\n  flows: [authorizationCode]\n  sources: [well-known/1up-oauth-authorization-server.json, well-known/1up-oauth-protected-resource.json]\n- scope: profile\n  description: Basic profile claims for the signed-in 1up user.\n  flows: [authorizationCode]\n  sources: [well-known/1up-oauth-authorization-server.json, well-known/1up-oauth-protected-resource.json]\n- scope: email\n  description: Email address claim for the signed-in 1up user.\n  flows: [authorizationCode]\n  sources: [well-known/1up-oauth-authorization-server.json, well-known/1up-oauth-protected-resource.json]\n- scope: offline_access\n  description: >-\n    Issue a refresh token so the MCP client can keep working without re-prompting; the\n    1up-mcp CLI caches and auto-refreshes credentials in ~/.1up/credentials.json.\n  flows: [authorizationCode]\n  sources: [well-known/1up-oauth-authorization-server.json, well-known/1up-oauth-protected-resource.json]\n\
  gaps:\n- >-\n  No read/write separation. An agent that can call ask_question can equally call\n  delete_qa_pair, delete_kb_item and delete_knowledge_group — the token does not\n  distinguish them.\n- >-\n  No per-workspace scope. switch_workspace lets a token move between every workspace the\n  user can reach; scope does not pin an agent to one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1up/refs/heads/main/scopes/1up-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Sales Enablement
- Knowledge Management
- RFP Automation
- Security Questionnaires
- Model Context Protocol
- Agents
- SaaS
- Revenue Operations
token_urls:
- https://mcp.1up.ai/token
---
