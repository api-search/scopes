---
authorization_urls:
- https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Arphie Scopes
name_suffix: OAuth Scopes
note: Arphie publishes no OpenAPI and no human-readable scopes/permissions reference, so derive-oauth-scopes.py had nothing to read. Every scope below comes from live, anonymous OAuth discovery metadata. The Arphie MCP server's protected-resource document declares exactly ONE supported scope (`email`); the Supabase authorization server behind it advertises the standard OIDC scope set. Nothing here is inferred.
overview: 'Arphie publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arphie API on a user''s behalf.


  Tokens are issued from https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arphie
provider_slug: arphie
schemes:
- flows:
  - authorizationUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token
  name: ArphieMCPOAuth
  resource: https://app.arphie.ai/api/mcp
  source: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp
scope_count: 1
scope_names:
- email
scopes:
- description: The only scope the Arphie MCP protected-resource metadata declares as supported for https://app.arphie.ai/api/mcp.
  flows:
  - authorizationCode
  scope: email
slug: arphie-scopes
source_filename: arphie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp\nnote: >-\n  Arphie publishes no OpenAPI and no human-readable scopes/permissions reference, so\n  derive-oauth-scopes.py had nothing to read. Every scope below comes from live,\n  anonymous OAuth discovery metadata. The Arphie MCP server's protected-resource\n  document declares exactly ONE supported scope (`email`); the Supabase authorization\n  server behind it advertises the standard OIDC scope set. Nothing here is inferred.\nschemes:\n- name: ArphieMCPOAuth\n  source: https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp\n  resource: https://app.arphie.ai/api/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token\nscopes:\n- scope: email\n  description: >-\n    The only scope the Arphie MCP protected-resource\
  \ metadata declares as supported for\n    https://app.arphie.ai/api/mcp.\n  flows: [authorizationCode]\n  declared_by: resource\n  sources: [https://app.arphie.ai/.well-known/oauth-protected-resource/api/mcp]\nauthorization_server_scopes:\n- scope: openid\n  declared_by: authorization-server\n- scope: profile\n  declared_by: authorization-server\n- scope: email\n  declared_by: authorization-server\n- scope: phone\n  declared_by: authorization-server\n- scope: offline_access\n  declared_by: authorization-server\nauthorization_server_scopes_source: https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/.well-known/oauth-authorization-server\ngaps:\n- >-\n  There is no Arphie-authored permission model in the OAuth layer — no read/write scopes,\n  no per-resource scopes. Authorization inside the product is handled by Arphie's\n  role-based access controls after identity is established, not by OAuth scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arphie/refs/heads/main/scopes/arphie-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Enterprise
- Artificial Intelligence
- Sales Enablement
- RFP Automation
- Security Questionnaires
- Knowledge-Management
- Go-To-Market
- MCP
- Agents
token_urls:
- https://ogxxofxbnksprbjqojnc.supabase.co/auth/v1/oauth/token
---
