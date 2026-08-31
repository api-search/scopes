---
api_specs:
- filename: relevance-ai-openapi.json
  format: json
  label: Relevance AI API
  slug: relevance-ai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/openapi/relevance-ai-openapi.json
authorization_urls: []
description: 'The REST API declares no oauth2 security scheme — it authenticates with a static `Authorization: project:api_key` header and has no scope concept at all. The only OAuth surface is the MCP server, and its scope model is deliberately coarse: one scope, with real authorization carried by the caller''s project role rather than by scope strings.'
docs: https://relevanceai.com/docs/integrations/mcp/mcp-server#access-control
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Relevance Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Relevance AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Relevance AI
provider_slug: relevance-ai
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: relevance-ai-scopes
source_filename: relevance-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: >-\n  https://mcp.relevanceai.com/.well-known/oauth-authorization-server,\n  https://mcp.relevanceai.com/.well-known/oauth-protected-resource,\n  https://relevanceai.com/docs/integrations/mcp/mcp-server\nprovider: Relevance AI\nproviderId: relevance-ai\ndescription: >-\n  The REST API declares no oauth2 security scheme — it authenticates with a static\n  `Authorization: project:api_key` header and has no scope concept at all. The only OAuth\n  surface is the MCP server, and its scope model is deliberately coarse: one scope, with real\n  authorization carried by the caller's project role rather than by scope strings.\nrest_api:\n  oauth2: false\n  scopes: []\n  detail: >-\n    derive-oauth-scopes.py over openapi/relevance-ai-openapi.json found 0 oauth2 flows across\n    566 operations. The single securityScheme is apiKey in header. An API key grants\n    unrestricted access to every resource in its project — the docs say so explicitly\
  \ — so\n    there is no way to issue a least-privilege REST credential.\nmcp:\n  authorization_server: https://mcp.relevanceai.com/\n  scopes_supported:\n    - name: claudeai\n      description: >-\n        The only scope the authorization server advertises, in both the authorization-server\n        and protected-resource metadata. It carries no capability semantics.\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  dynamic_client_registration: true\n  effective_authorization:\n    model: project role, enforced server-side\n    detail: >-\n      Because there is one scope, the real permission boundary is the caller's Relevance AI\n      project role, applied at consent time. Write and destructive tools are REMOVED from the\n      tool list server-side for restricted sessions rather than merely hidden client-side.\n    roles:\n      - role: Admin\n        access: full\n        can_opt_into_run_only: true\n      - role: Editor\n        access: full\n        can_opt_into_run_only:\
  \ true\n      - role: Member\n        access: full\n        can_opt_into_run_only: true\n      - role: Viewer\n        access: run-only\n        can_opt_into_run_only: forced\n      - role: Chat\n        access: chat-only\n        can_opt_into_run_only: forced\n    consent_toggle: >-\n      The OAuth consent screen shows a Run-Only mode toggle for Member, Editor and Admin,\n      defaulting to off (full access).\n    limitation: >-\n      Chat-role users cannot set up dynamic (user-level) OAuth connections via MCP.\n  session_scope: one Relevance AI project per authenticated connection\ndocs: https://relevanceai.com/docs/integrations/mcp/mcp-server#access-control\ngaps:\n  - REST API keys cannot be scoped or least-privileged; they are all-or-nothing per project.\n  - A single OAuth scope means a client cannot request narrower access than its role allows.\n  - No scope reference page is published; the scope name was read from the metadata document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relevance-ai/refs/heads/main/scopes/relevance-ai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- AI Agents
- AI Automation
- Multi-Agent Systems
- Agent Platform
- MCP
- agent-native
- Workflow-Automation
- LLM Orchestration
- Knowledge-Management
- Observability
- Sales Automation
- GTM Engineering
token_urls: []
---
