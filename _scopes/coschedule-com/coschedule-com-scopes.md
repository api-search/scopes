---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CoSchedule Scopes
name_suffix: OAuth Scopes
note: Read from the MCP server's published OAuth protected-resource metadata (HTTP 200). No scopes reference page in the docs; access mirrors the signing-in user's calendar permissions and is read-only per https://coschedule.com/support/integrations/ai-chat-apps/use-claude-and-chatgpt-with-coschedule.
overview: 'CoSchedule publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoSchedule API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoSchedule
provider_slug: coschedule-com
schemes: []
scope_count: 1
scope_names:
- openid
scopes:
- description: OpenID Connect sign-in scope, the only value in scopes_supported.
  flows: []
  scope: openid
slug: coschedule-com-scopes
source_filename: coschedule-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://platform.coschedule.com/.well-known/oauth-protected-resource/mcp\nnote: Read from the MCP server's published OAuth protected-resource metadata (HTTP 200). No scopes reference page in the docs; access mirrors the signing-in user's calendar permissions and is read-only per https://coschedule.com/support/integrations/ai-chat-apps/use-claude-and-chatgpt-with-coschedule.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in scope, the only value in scopes_supported.\n"
source_yaml_url: https://artifacts.apis.io/coschedule-com/scopes/coschedule-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- Marketing
- Social Media Management
- Content Calendar
- Marketing Automation
- Scheduling
- MCP
token_bound: false
token_urls: []
---
