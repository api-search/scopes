---
authorization_urls: []
description: Colon-separated OAuth 2.0 scope strings verified for the current release, used by the Perk MCP server and OAuth partner integrations. Also confirmed in the MCP protected-resource metadata (scopes_supported).
docs: https://developers.perk.com/docs/perk-mcp-tools-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Perk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Perk uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Perk
provider_slug: perk
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: perk-scopes
source_filename: perk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.perk.com/docs/authenticate-with-the-perk-mcp-server\ndocs: https://developers.perk.com/docs/perk-mcp-tools-reference\nname: Perk OAuth Scopes\ntype: OAuthScopes\ndescription: >-\n  Colon-separated OAuth 2.0 scope strings verified for the current release, used by\n  the Perk MCP server and OAuth partner integrations. Also confirmed in the MCP\n  protected-resource metadata (scopes_supported).\nstyle: colon-separated\nscopes:\n- name: user:read\n  grants: Read user profile and search results.\n  required: true\n- name: trip:read\n  grants: Read trips and trip breakdowns.\n  required: true\n- name: expenses:read\n  grants: Read the signed-in user's expenses.\n- name: report:write\n  grants: Generate, poll, and download travel and spend reports (same scope covers download/poll).\n- name: my-travel-policy:read\n  grants: Read the user's travel and spend policy.\nnotes:\n- Invoice, event, and card tools require\
  \ no additional scope; access follows the user's Perk role/permissions (RBAC).\n- Card and transaction tools additionally require a Spend subscription.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perk/refs/heads/main/scopes/perk-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Corporate Travel
- Expense Management
- Spend Management
- Travel
- Invoices
- Fintech
- SaaS
token_urls: []
---
