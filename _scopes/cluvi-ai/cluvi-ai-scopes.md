---
authorization_urls: []
description: ''
docs: https://cluvi.ai/mcp.md
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cluvi AI Scopes
name_suffix: OAuth Scopes
note: Both scopes are read from the published discovery metadata (HTTP 200). The docs publish no scope reference page.
overview: 'Cluvi AI publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cluvi AI API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cluvi AI
provider_slug: cluvi-ai
schemes: []
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access to the MCP server's tools. Listed in scopes_supported in both the authorization-server and protected-resource metadata. The docs do not describe what it covers.
  flows: []
  scope: mcp:read
- description: Write access through the MCP server. Listed in scopes_supported. The docs say the person chooses "whether it can make changes" when connecting, which matches this scope; the scope itself is not described.
  flows: []
  scope: mcp:write
slug: cluvi-ai-scopes
source_filename: cluvi-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://cluvi.ai/.well-known/oauth-protected-resource/mcp\ndocs: https://cluvi.ai/mcp.md\nscopes:\n- name: mcp:read\n  description: Read access to the MCP server's tools. Listed in scopes_supported in both the authorization-server and protected-resource metadata. The docs do not describe what it covers.\n- name: mcp:write\n  description: Write access through the MCP server. Listed in scopes_supported. The docs say the person chooses \"whether it can make changes\" when connecting, which matches this scope; the scope itself is not described.\nnote: Both scopes are read from the published discovery metadata (HTTP 200). The docs publish no scope reference page.\n"
source_yaml_url: https://artifacts.apis.io/cluvi-ai/scopes/cluvi-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Restaurant
- Hospitality
- Reservations
- WhatsApp
- Messaging
- AI Receptionist
- MCP
token_bound: false
token_urls: []
---
