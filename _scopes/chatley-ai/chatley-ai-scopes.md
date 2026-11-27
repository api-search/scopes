---
api_specs:
- filename: chatley-ai-openapi-generated.yml
  format: yaml
  label: Chatley Developer API
  slug: developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatley-ai/openapi/_ae-authored/chatley-ai-openapi-generated.yml
authorization_urls: []
description: ''
docs: https://docs.chatley.ai/mcp/connecting
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Chatley AI Scopes
name_suffix: OAuth Scopes
note: OAuth applies only to the MCP server. Its protected-resource metadata (HTTP 200) lists only OIDC housekeeping scopes; the docs publish no per-tool permission scopes - tool visibility follows the user's Chatley role instead ("The tool list reflects what you are allowed to do").
overview: 'Chatley AI publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chatley AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chatley AI
provider_slug: chatley-ai
schemes: []
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect sign-in (listed in scopes_supported).
  flows: []
  scope: openid
- description: Refresh-token access (listed in scopes_supported).
  flows: []
  scope: offline_access
slug: chatley-ai-scopes
source_filename: chatley-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://mcp.chatley.ai/.well-known/oauth-protected-resource\ndocs: https://docs.chatley.ai/mcp/connecting\nnote: OAuth applies only to the MCP server. Its protected-resource metadata (HTTP 200) lists only OIDC housekeeping scopes;\n  the docs publish no per-tool permission scopes - tool visibility follows the user's Chatley role instead (\"The tool list\n  reflects what you are allowed to do\").\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (listed in scopes_supported).\n- name: offline_access\n  description: Refresh-token access (listed in scopes_supported).\n"
source_yaml_url: https://artifacts.apis.io/chatley-ai/scopes/chatley-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Artificial Intelligence
- Voice Agents
- Conversational AI
- AI Receptionist
- Telephony
- SMS
- White Label
- MCP
- Lead Generation
token_bound: false
token_urls: []
---
