---
authorization_urls: []
description: OAuth scopes advertised by machine0's authorization server metadata (scopes_supported). These are OIDC-standard identity scopes gating the OAuth authorization-code flow used by the CLI and MCP clients; machine0 does not publish granular per-resource (VM/image) scopes — infrastructure authorization is bound to the authenticated account rather than fine-grained scopes.
docs: https://docs.machine0.io/mcp/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Machine0 Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Machine0 publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Machine0 API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Machine0
provider_slug: machine0
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OIDC authentication; issue an ID token identifying the account.
  flows: []
  scope: openid
- description: Access to the account's basic profile claims (name).
  flows: []
  scope: profile
- description: Access to the account's email and email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived, non-interactive access.
  flows: []
  scope: offline_access
slug: machine0-scopes
source_filename: machine0-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.machine0.io/.well-known/oauth-authorization-server\ndescription: >-\n  OAuth scopes advertised by machine0's authorization server metadata\n  (scopes_supported). These are OIDC-standard identity scopes gating the OAuth\n  authorization-code flow used by the CLI and MCP clients; machine0 does not\n  publish granular per-resource (VM/image) scopes — infrastructure authorization\n  is bound to the authenticated account rather than fine-grained scopes.\ndocs: https://docs.machine0.io/mcp/overview\nscopes:\n  - name: openid\n    description: OIDC authentication; issue an ID token identifying the account.\n  - name: profile\n    description: Access to the account's basic profile claims (name).\n  - name: email\n    description: Access to the account's email and email_verified claims.\n  - name: offline_access\n    description: Issue a refresh token for long-lived, non-interactive access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machine0/refs/heads/main/scopes/machine0-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Cloud
- Infrastructure
- Virtual Machines
- AI Agents
- Developer Tools
- CLI
- MCP
token_bound: false
token_urls: []
---
