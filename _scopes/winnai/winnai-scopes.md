---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Winnai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Winn.ai publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Winn.ai API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Winn.ai
provider_slug: winnai
schemes: []
scope_count: 2
scope_names:
- sessions:read
- mcp
scopes:
- description: 'Read access to call sessions. Provider publishes no description; the name is recorded verbatim from scopes_supported. It is consistent with the Enterprise plan''s stated "API access: Get conversation data and AI insights, in any tool".'
  flows: []
  scope: sessions:read
- description: Single coarse scope for the WordPress MCP Adapter surface on the marketing site's CMS. Provider publishes no description. Not a product API scope.
  flows: []
  scope: mcp
slug: winnai-scopes
source_filename: winnai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  scopes_supported in https://app.winn.ai/.well-known/oauth-authorization-server\n  and https://winn.ai/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  WINN.AI publishes no scopes or permissions reference page. Every scope below was\n  read verbatim from RFC 8414 authorization server metadata. No description text\n  is published by the provider for any of them, so the description fields record\n  what the scope name plainly denotes and say so.\n\nscope_count: 2\nscopes:\n- name: sessions:read\n  authorization_server: https://app.winn.ai\n  resource: https://app.winn.ai/mcp\n  description: >-\n    Read access to call sessions. Provider publishes no description; the name is\n    recorded verbatim from scopes_supported. It is consistent with the Enterprise\n    plan's stated \"API access: Get conversation data and AI insights, in any\n    tool\".\n  read_write: read\n  provider_described: false\n- name:\
  \ mcp\n  authorization_server: https://winn.ai\n  resource: https://winn.ai/wp-json/mcp/mcp-oauth-server\n  description: >-\n    Single coarse scope for the WordPress MCP Adapter surface on the marketing\n    site's CMS. Provider publishes no description. Not a product API scope.\n  read_write: unknown\n  provider_described: false\n  product_surface: false\n\nobservations:\n- The product authorization server advertises exactly one scope, and it is\n  read-only. No write scope is published, which is consistent with a\n  conversation-data export surface rather than a full CRUD API.\n- Scope granularity is coarse-to-nonexistent on the WordPress server (a single\n  \"mcp\" scope covers the whole surface).\n\nrelated:\n- authentication/winnai-authentication.yml\n- mcp/winnai-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/winnai/refs/heads/main/scopes/winnai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Sales
- Artificial Intelligence
- Revenue
- CRM
- Sales Enablement
- Conversation Intelligence
- Productivity
token_bound: false
token_urls: []
---
