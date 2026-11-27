---
authorization_urls: []
description: ''
docs: https://cloziq.com/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cloziq Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by the MCP server's OAuth authorization-server and protected-resource metadata (both HTTP 200). They are identity scopes only; the docs say access is scoped to the user's own workspace and the consent screen lists write, publish and delete, but no finer-grained API scopes are published.
overview: 'Cloziq publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloziq API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloziq
provider_slug: cloziq-com
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in.
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Refresh token issuance (refresh_token grant is advertised).
  flows: []
  scope: offline_access
slug: cloziq-com-scopes
source_filename: cloziq-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.cloziq.com/.well-known/oauth-authorization-server\ndocs: https://cloziq.com/mcp\nname: Cloziq OAuth scopes\nnote: scopes_supported as advertised by the MCP server's OAuth authorization-server and protected-resource metadata (both HTTP 200). They are identity scopes only; the docs say access is scoped to the user's own workspace and the consent screen lists write, publish and delete, but no finer-grained API scopes are published.\nscopes:\n- name: openid\n  description: OpenID Connect sign-in.\n- name: profile\n  description: Basic profile claims.\n- name: email\n  description: Email address claim.\n- name: offline_access\n  description: Refresh token issuance (refresh_token grant is advertised).\n"
source_yaml_url: https://artifacts.apis.io/cloziq-com/scopes/cloziq-com-scopes.yml
summary_line: 4 scopes
tags:
- Company
- AI Sales Agent
- Instagram
- Facebook Messenger
- Direct Messaging
- Appointment-Setting
- Sales Automation
- MCP
token_bound: false
token_urls: []
---
