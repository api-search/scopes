---
authorization_urls: []
description: ''
docs: https://ctd.ai/integrations-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ctd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Connect The Dots uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Connect The Dots
provider_slug: ctd
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ctd-scopes
source_filename: ctd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.ctd.ai/.well-known/oauth-authorization-server + https://ctd.ai/integrations-mcp\ndocs: https://ctd.ai/integrations-mcp\noauth: true\nauthorization_server: https://app.ctd.ai/users-api\nflows:\n- authorization_code\npkce: S256\nscopes:\n- name: read\n  description: >-\n    Read access to your relationship graph — look up people and companies, resolve\n    warm paths to a target, natural-language path search, list ghost emails and the\n    activity feed, and see recent job changes across your network.\n- name: write\n  description: >-\n    Write access — create and send ghost emails, update path stages, run approver\n    actions (share/decline), and add or remove path participants.\nnotes: >-\n  read and write are the only scopes advertised by the OAuth authorization-server\n  metadata (scopes_supported). Scope descriptions are mapped from the documented\n  REST/MCP operation surface (GET operations = read; POST/PATCH\
  \ operations = write).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctd/refs/heads/main/scopes/ctd-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Relationship Intelligence
- Sales
- Warm Introductions
- Network Graph
- CRM
- MCP
- Venture Capital
token_urls: []
---
