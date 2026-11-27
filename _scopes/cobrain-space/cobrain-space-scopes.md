---
authorization_urls: []
description: ''
docs: https://cobrain.space/guides/tools
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cobrain Scopes
name_suffix: OAuth Scopes
note: scopes_supported as published in the RFC 8414 authorization-server metadata (HTTP 200, 2026-11-04). The docs publish no per-scope permissions reference; tool access is governed by the user's own brain permissions ("All of them work with your permissions"), not by scopes.
overview: 'Cobrain publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cobrain API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cobrain
provider_slug: cobrain-space
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in scope (listed in scopes_supported).
  flows: []
  scope: openid
- description: Basic profile claims (listed in scopes_supported).
  flows: []
  scope: profile
- description: Email claim (listed in scopes_supported).
  flows: []
  scope: email
- description: Refresh token issuance; the guide states the grant "expires and renews".
  flows: []
  scope: offline_access
slug: cobrain-space-scopes
source_filename: cobrain-space-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://cobrain.space/.well-known/oauth-authorization-server\ndocs: https://cobrain.space/guides/tools\nnote: scopes_supported as published in the RFC 8414 authorization-server metadata (HTTP 200, 2026-11-04). The docs publish no per-scope permissions reference; tool access is governed by the user's own brain permissions (\"All of them work with your permissions\"), not by scopes.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in scope (listed in scopes_supported).\n- name: profile\n  description: Basic profile claims (listed in scopes_supported).\n- name: email\n  description: Email claim (listed in scopes_supported).\n- name: offline_access\n  description: Refresh token issuance; the guide states the grant \"expires and renews\".\n"
source_yaml_url: https://artifacts.apis.io/cobrain-space/scopes/cobrain-space-scopes.yml
summary_line: 4 scopes
tags:
- Company
- AI Memory
- MCP
- MCP Server
- Knowledge Management
- Markdown
- Note Taking
- Collaboration
- Artificial Intelligence
token_bound: false
token_urls: []
---
