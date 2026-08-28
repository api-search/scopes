---
authorization_urls: []
description: ''
docs: https://docs.simetrik.com/mcp/connect
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Simetrik Scopes
name_suffix: OAuth Scopes
note: These are the scopes the running authorization server advertises, not a scope reference page - Simetrik publishes no scopes/permissions reference, and the docs actively tell users to leave the client's OAuth advanced settings closed. The three scopes are identity scopes only; they carry no Simetrik-resource authorization. Actual authorization is the signed-in user's own workspace role and permissions, enforced server-side on every call, plus two independent gates (the workspace must be enabled for CLI/agent access and the role must hold the "Use CLI" permission). That means the OAuth scope set does NOT describe what an agent can reach - see authentication/simetrik-authentication.yml.
overview: 'Simetrik uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Simetrik
provider_slug: simetrik
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: simetrik-scopes
source_filename: simetrik-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  https://mcp.us.simetrik.com/.well-known/oauth-authorization-server (HTTP 200) and\n  https://mcp.us.simetrik.com/.well-known/oauth-protected-resource/mcp (HTTP 200), both fetched\n  anonymously 2026-08-27.\ndocs: https://docs.simetrik.com/mcp/connect\nnote: >-\n  These are the scopes the running authorization server advertises, not a scope reference page -\n  Simetrik publishes no scopes/permissions reference, and the docs actively tell users to leave the\n  client's OAuth advanced settings closed. The three scopes are identity scopes only; they carry no\n  Simetrik-resource authorization. Actual authorization is the signed-in user's own workspace role and\n  permissions, enforced server-side on every call, plus two independent gates (the workspace must be\n  enabled for CLI/agent access and the role must hold the \"Use CLI\" permission). That means the OAuth\n  scope set does NOT describe what an agent can reach - see\
  \ authentication/simetrik-authentication.yml.\nauthorization_server: https://mcp.us.simetrik.com/\nprotected_resource: https://mcp.us.simetrik.com/mcp\nscope_count: 3\nscopes:\n- name: openid\n  description: OpenID Connect authentication of the Simetrik user.\n  kind: identity\n- name: profile\n  description: Basic profile claims for the signed-in Simetrik user.\n  kind: identity\n- name: email\n  description: Email address of the signed-in Simetrik user.\n  kind: identity\npermission_model:\n  granularity: workspace role\n  documented_permissions:\n  - name: Use CLI\n    description: >-\n      Role-level permission required for both the CLI and the MCP server. Without it the workspace\n      does not appear on the connect picker and tools return permission errors.\n    granted_in: app.simetrik.com\n  note: >-\n    Simetrik does not publish a full permission catalog. Only the \"Use CLI\" permission is named in the\n    public docs; the rest are referred to generically as \"the corresponding\
  \ access for your role\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simetrik/refs/heads/main/scopes/simetrik-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Reconciliation
- Financial Operations
- Payments
- Accounting
- FinTech
- Financial Close
- Data Integration
- Agents
- MCP
- Latin America
token_urls: []
---
