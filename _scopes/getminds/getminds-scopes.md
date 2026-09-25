---
api_specs:
- filename: getminds-openapi.json
  format: json
  label: Minds Public API
  slug: minds-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-openapi.json
authorization_urls: []
description: ''
docs: https://getminds.ai/mcp/setup
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Getminds Scopes
name_suffix: OAuth Scopes
note: OAuth scopes apply to the Minds MCP server (protected resource https://getminds.ai/mcp). The REST v1 API authenticates with a personal API key and declares no oauth2 scopes. Scopes below are read verbatim from the provider's published authorization-server and protected-resource metadata.
overview: 'Minds uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Minds
provider_slug: getminds
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: getminds-scopes
source_filename: getminds-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://getminds.ai/.well-known/oauth-authorization-server\ndocs: https://getminds.ai/mcp/setup\nnote: >-\n  OAuth scopes apply to the Minds MCP server (protected resource\n  https://getminds.ai/mcp). The REST v1 API authenticates with a personal API\n  key and declares no oauth2 scopes. Scopes below are read verbatim from the\n  provider's published authorization-server and protected-resource metadata.\nauthorization_server: https://getminds.ai\nresource: https://getminds.ai/mcp\nscopes:\n- name: openid\n  description: OpenID Connect subject/identity.\n- name: email\n  description: Authenticated account email and verification status.\n- name: profile\n  description: Authenticated account profile claims.\n- name: sparks:read\n  description: Read Minds (\"sparks\") and Audiences.\n- name: sparks:write\n  description: Create and modify Minds (\"sparks\") and Audiences.\n- name: sparks:chat\n  description: Run chat/completion\
  \ and research against Minds and Audiences.\n- name: flows:read\n  description: Read Studies, chats, drafts, runs and research flows.\n- name: flows:write\n  description: Create and run Studies, chats, drafts and research flows.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/scopes/getminds-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Synthetic Research
- Market Research
- Surveys
- User Research
- Marketing Analytics
- ai-personas
- MCP
- Agent-Native
- GDPR
token_urls: []
---
