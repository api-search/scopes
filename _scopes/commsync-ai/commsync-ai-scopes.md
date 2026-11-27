---
authorization_urls: []
description: The OAuth 2.1 authorization server issues a single scope. Finer-grained access is not expressed as scopes but as the user's org role (OWNER, ADMIN, MEMBER), channel memberships, and a per-credential channel allowlist chosen on the consent screen or on the API key.
docs: https://commsync.ai/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CommSync Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CommSync publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CommSync API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CommSync
provider_slug: commsync-ai
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to the CommSync MCP server (https://server.commsync.ai/api/mcp) as the signed-in user, limited to the lines chosen on the consent screen.
  flows: []
  scope: mcp
slug: commsync-ai-scopes
source_filename: commsync-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commsync.ai/docs/mcp.txt\ndocs: https://commsync.ai/auth.md\ndescription: The OAuth 2.1 authorization server issues a single scope. Finer-grained access is not expressed as scopes but as the user's org role (OWNER, ADMIN, MEMBER), channel memberships, and a per-credential channel allowlist chosen on the consent screen or on the API key.\nscopes:\n- name: mcp\n  description: Access to the CommSync MCP server (https://server.commsync.ai/api/mcp) as the signed-in user, limited to the lines chosen on the consent screen.\n  source: https://commsync.ai/docs/mcp.txt\npermission_model:\n  roles: [OWNER, ADMIN, MEMBER]\n  docs: https://commsync.ai/docs/roles-and-permissions\n  channel_scoping: Every request is executed as the credential's owner, gated by their org role and channel access; an API key or connected OAuth app may additionally be channel-scoped to specific lines.\n"
source_yaml_url: https://artifacts.apis.io/commsync-ai/scopes/commsync-ai-scopes.yml
summary_line: 1 scope
tags:
- Company
- Unified Inbox
- SMS
- Email
- Messaging
- Artificial Intelligence
- AI Agents
- MCP
- Webhook
- Communications
token_bound: false
token_urls: []
---
