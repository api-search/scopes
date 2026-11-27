---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Comuna Scopes
name_suffix: OAuth Scopes
note: These are the only scopes the protected-resource metadata advertises; they are identity scopes, not resource permissions. The docs state access is bounded by the user's row-level-security permissions rather than by fine-grained OAuth scopes. No scopes reference page is published.
overview: 'Comuna publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Comuna API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Comuna
provider_slug: comuna-work
schemes: []
scope_count: 4
scope_names:
- openid
- email
- profile
- offline_access
scopes:
- description: OpenID Connect sign-in (advertised in scopes_supported).
  flows: []
  scope: openid
- description: User email claim (advertised in scopes_supported).
  flows: []
  scope: email
- description: User profile claims (advertised in scopes_supported).
  flows: []
  scope: profile
- description: Refresh token issuance (advertised in scopes_supported).
  flows: []
  scope: offline_access
slug: comuna-work-scopes
source_filename: comuna-work-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://api.comuna.work/.well-known/oauth-protected-resource\nhttp_status: 200\nscopes:\n- name: openid\n  description: OpenID Connect sign-in (advertised in scopes_supported).\n- name: email\n  description: User email claim (advertised in scopes_supported).\n- name: profile\n  description: User profile claims (advertised in scopes_supported).\n- name: offline_access\n  description: Refresh token issuance (advertised in scopes_supported).\nnote: These are the only scopes the protected-resource metadata advertises; they are identity scopes, not resource permissions. The docs state access is bounded by the user's row-level-security permissions rather than by fine-grained OAuth scopes. No scopes reference page is published.\n"
source_yaml_url: https://artifacts.apis.io/comuna-work/scopes/comuna-work-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Project Management
- Kanban
- Collaboration
- AI Agents
- MCP
- Productivity
token_bound: false
token_urls: []
---
