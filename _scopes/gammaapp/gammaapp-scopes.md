---
authorization_urls: []
description: ''
docs: https://developers.gamma.app/mcp/mcp-tools-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gammaapp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gamma.app publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gamma.app API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gamma.app
provider_slug: gammaapp
schemes:
- authorization_server: https://auth.gamma.app
  name: OAuth2
  source: https://mcp.gamma.app/.well-known/oauth-protected-resource
scope_count: 2
scope_names:
- generate
- gamma:read
scopes:
- description: Create gammas (presentations, documents, webpages, social posts) in the user's workspace.
  flows: []
  scope: generate
- description: Read gammas, list folders, and list themes from the user's workspace.
  flows: []
  scope: gamma:read
slug: gammaapp-scopes
source_filename: gammaapp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.gamma.app/.well-known/oauth-protected-resource\ndocs: https://developers.gamma.app/mcp/mcp-tools-reference\nnotes: >-\n  OAuth scopes apply to the Gamma MCP server / connector OAuth flow (auth server\n  https://auth.gamma.app), not to the API-key-authenticated REST API. Scope list\n  taken verbatim from the RFC 9728 protected-resource metadata; the human-facing\n  consent permissions are documented in the MCP tools reference.\nschemes:\n- name: OAuth2\n  authorization_server: https://auth.gamma.app\n  source: https://mcp.gamma.app/.well-known/oauth-protected-resource\nscopes:\n- scope: generate\n  description: Create gammas (presentations, documents, webpages, social posts) in the user's workspace.\n  sources: [well-known/gammaapp-oauth-protected-resource.json]\n- scope: 'gamma:read'\n  description: Read gammas, list folders, and list themes from the user's workspace.\n  sources: [well-known/gammaapp-oauth-protected-resource.json]\n\
  consent_permissions:\n- Create gammas in your workspace\n- Read gammas in your workspace\n- List folders from your workspace\n- List themes from your workspace\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gammaapp/refs/heads/main/scopes/gammaapp-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Artificial Intelligence
- Presentations
- Documents
- Content Generation
- Generative AI
- Productivity
- MCP
- Websites
- Social Media
token_urls: []
---
