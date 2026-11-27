---
authorization_urls: []
description: ''
docs: https://clerkchat.co/docs/guides/connect-assistant
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: ClerkChat Scopes
name_suffix: OAuth Scopes
note: Scope names are read from scopes_supported in the protected-resource and authorization-server metadata (HTTP 200). The docs do not describe them individually; they say "Review the requested permissions and approve the connection" and that access is further limited to approved workspaces and the user's role and plan. Descriptions below are left empty rather than inferred.
overview: 'ClerkChat publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClerkChat API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClerkChat
provider_slug: clerkchat-co
schemes: []
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: ''
  flows: []
  scope: mcp:read
- description: ''
  flows: []
  scope: mcp:write
- description: ''
  flows: []
  scope: offline_access
slug: clerkchat-co-scopes
source_filename: clerkchat-co-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.clerkchat.co/.well-known/oauth-protected-resource\ndocs: https://clerkchat.co/docs/guides/connect-assistant\nnote: Scope names are read from scopes_supported in the protected-resource and authorization-server metadata (HTTP 200). The docs do not describe them individually; they say \"Review the requested permissions and approve the connection\" and that access is further limited to approved workspaces and the user's role and plan. Descriptions below are left empty rather than inferred.\nscopes:\n- name: mcp:read\n  description: null\n- name: mcp:write\n  description: null\n- name: offline_access\n  description: null\n"
source_yaml_url: https://artifacts.apis.io/clerkchat-co/scopes/clerkchat-co-scopes.yml
summary_line: 3 scopes
tags:
- Company
- AI Agents
- Customer Service
- Chatbots
- Messaging
- WhatsApp
- MCP
- Conversational AI
token_bound: false
token_urls: []
---
