---
authorization_urls: []
description: ''
docs: https://help.clueso.io/mcp-setup
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Clueso Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by the MCP protected-resource metadata and by the auth.clueso.io authorization-server metadata. These are identity scopes only; the docs publish no per-tool permission scopes. Some tools (video export, advanced branding, record_screen) are gated by Clueso plan, not by OAuth scope.
overview: 'Clueso publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clueso API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clueso
provider_slug: clueso-io
schemes: []
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: OpenID Connect sign-in.
  flows: []
  scope: openid
- description: Access to the user's email address.
  flows: []
  scope: email
- description: Access to the user's basic profile.
  flows: []
  scope: profile
slug: clueso-io-scopes
source_filename: clueso-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Clueso OAuth scopes\ngenerated: '2026-11-04'\nmethod: probed\nsource: https://connect.clueso.io/.well-known/oauth-protected-resource\ndocs: https://help.clueso.io/mcp-setup\nnote: scopes_supported as advertised by the MCP protected-resource metadata and by the auth.clueso.io authorization-server metadata. These are identity scopes only; the docs publish no per-tool permission scopes. Some tools (video export, advanced branding, record_screen) are gated by Clueso plan, not by OAuth scope.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in.\n- name: email\n  description: Access to the user's email address.\n- name: profile\n  description: Access to the user's basic profile.\n"
source_yaml_url: https://artifacts.apis.io/clueso-io/scopes/clueso-io-scopes.yml
summary_line: 3 scopes
tags:
- Company
- AI Video
- Documentation
- Screen Recording
- Video Creation
- Knowledge Base
- Training
- MCP
token_bound: false
token_urls: []
---
