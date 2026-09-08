---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Accordacff Scopes
name_suffix: OAuth Scopes
note: Read from Accord's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, both served anonymously on api.inaccord.com. These scopes govern the Accord MCP server. The Accord Developer API (GraphQL) does NOT use OAuth — it authenticates with a workspace-scoped bearer API key and has no scope surface; per Accord's authentication page, "the same Row-Level Security rules that apply to in-app sessions apply to API key requests". Accord publishes no separate scopes/permissions reference page; nothing beyond the metadata was found.
overview: 'Accord uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Accord
provider_slug: accordacff
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: accordacff-scopes
source_filename: accordacff-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://api.inaccord.com/.well-known/oauth-authorization-server\nname: Accord OAuth scopes\nnote: >-\n  Read from Accord's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, both served\n  anonymously on api.inaccord.com. These scopes govern the Accord MCP server. The Accord Developer API (GraphQL) does\n  NOT use OAuth — it authenticates with a workspace-scoped bearer API key and has no scope surface; per Accord's\n  authentication page, \"the same Row-Level Security rules that apply to in-app sessions apply to API key requests\".\n  Accord publishes no separate scopes/permissions reference page; nothing beyond the metadata was found.\ndocs: null\nflows:\n  - type: authorization_code\n    authorization_endpoint: https://api.inaccord.com/1/mcp/authorize\n    token_endpoint: https://api.inaccord.com/1/mcp/token\n    pkce_required: true\n    code_challenge_methods:\n      - S256\n  - type: refresh_token\n\
  \    token_endpoint: https://api.inaccord.com/1/mcp/token\nscope_count: 2\nscopes:\n  - name: mcp:read\n    description: >-\n      Read access through the Accord MCP server. Advertised in both the authorization-server and protected-resource\n      metadata. Accord documents the server as read-only in beta, so this is the scope in use today. No per-scope\n      description is published by Accord; this note records what the documentation states, not an inferred meaning.\n  - name: mcp:write\n    description: >-\n      Write access through the Accord MCP server. Advertised in the metadata, but Accord's announcement states the\n      server \"currently reads from your Accord workspace\" with write support planned, so this scope is declared ahead\n      of the capability. No per-scope description is published by Accord.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accordacff/refs/heads/main/scopes/accordacff-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Enablement
- Revenue Operations
- Customer Collaboration
- Sales Engagement
- Customer Onboarding
- Mutual Action Plans
- CRM
- GraphQL
- MCP
- agent-native
- SaaS
- Company
token_urls: []
---
