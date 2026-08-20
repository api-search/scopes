---
authorization_urls: []
description: ''
docs: https://docs.chord.co/chord-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Chord Commerce Scopes
name_suffix: OAuth Scopes
note: Chord publishes no OpenAPI, so derive-oauth-scopes.py had no securitySchemes to read. These scopes are taken verbatim from the two live OAuth discovery documents Chord's MCP host serves. They are OIDC identity scopes only — Chord publishes NO resource/permission scopes (nothing like read:orders or write:audiences). Authorization inside the MCP server is decided by the authenticated user's Chord organization membership and by the server's own read-only constraint, not by scope.
overview: 'Chord uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chord
provider_slug: chord-commerce
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: chord-commerce-scopes
source_filename: chord-commerce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.chord.co/.well-known/oauth-protected-resource and\n  https://mcp.chord.co/.well-known/oauth-authorization-server\ndocs: https://docs.chord.co/chord-mcp\nnote: >-\n  Chord publishes no OpenAPI, so derive-oauth-scopes.py had no securitySchemes to\n  read. These scopes are taken verbatim from the two live OAuth discovery\n  documents Chord's MCP host serves. They are OIDC identity scopes only — Chord\n  publishes NO resource/permission scopes (nothing like read:orders or\n  write:audiences). Authorization inside the MCP server is decided by the\n  authenticated user's Chord organization membership and by the server's own\n  read-only constraint, not by scope.\napi: Chord MCP\nresource: https://mcp.chord.co/mcp\nauthorization_server: https://api.stytch.chord.co\nscopes:\n  - name: openid\n    description: OIDC — issue an ID token for the authenticated Chord user.\n    advertised_by:\n      - oauth-protected-resource\n\
  \      - oauth-authorization-server\n  - name: profile\n    description: OIDC — basic profile claims for the Chord user.\n    advertised_by:\n      - oauth-protected-resource\n      - oauth-authorization-server\n  - name: email\n    description: OIDC — the Chord user's email address.\n    advertised_by:\n      - oauth-protected-resource\n      - oauth-authorization-server\n  - name: offline_access\n    description: Issue a refresh token so the MCP client can reconnect without re-consent.\n    advertised_by:\n      - oauth-protected-resource\n      - oauth-authorization-server\n  - name: phone\n    description: OIDC — phone claim.\n    advertised_by:\n      - oauth-authorization-server\n    note: >-\n      Advertised by the authorization server but NOT listed in the MCP\n      protected-resource metadata, so it is not requestable for the MCP resource.\neffective_authorization:\n  model: tenant-membership\n  description: >-\n    Every MCP tool targets the CURRENT tenant's warehouse. The\
  \ set of tenants a\n    token can reach is the set of Chord organizations the authenticated user\n    belongs to; switch_tenant is rejected for any org the user is not a member of.\n  enforcement:\n    - read-only — execute_sql accepts SELECT/UNION/INTERSECT/EXCEPT only\n    - execute_sql capped at 10000 rows; preview_table capped at 100 rows\n  source: https://github.com/chordcommerce/chord-copilot/blob/main/plugin/skills/copilot/SKILL.md\nother_surfaces:\n  - api: Chord Audiences API\n    scopes: none\n    note: Flat bearer token; no scope model documented.\n  - api: Chord CDP Ingest API\n    scopes: none\n    note: Per-source write key; no scope model documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chord-commerce/refs/heads/main/scopes/chord-commerce-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Commerce
- Composable Commerce
- Headless Commerce
- Order Management
- OMS
- Customer Data Platform
- CDP
- Event Tracking
- Commerce Analytics
- Customer Lifetime Value
- AI Agents
- Commerce Copilot
- Solidus
- Spree
- Ruby on Rails
- Shopify
- Direct to Consumer
token_urls: []
---
