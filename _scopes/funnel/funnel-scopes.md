---
authorization_urls: []
description: ''
docs: https://help.funnel.io/en/articles/15014203-quick-start-guide-using-funnel-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Funnel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Funnel uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Funnel
provider_slug: funnel
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: funnel-scopes
source_filename: funnel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://mcp.ai.funnel.io/.well-known/oauth-protected-resource/mcp +\n  https://mcp.eu.ai.funnel.io/.well-known/oauth-protected-resource/mcp +\n  https://login.funnel.io/.well-known/openid-configuration\ndocs: https://help.funnel.io/en/articles/15014203-quick-start-guide-using-funnel-mcp\nauthorization_server: https://login.funnel.io\nidentity_provider: Auth0\nsurfaces:\n- api: Funnel MCP\n  resource: https://mcp.ai.funnel.io/mcp\n  flow: authorization_code\n  metadata: well-known/funnel-mcp-oauth-protected-resource.json\n  http_status: 200\n  scopes:\n  - name: openid\n    required: true\n    description: OIDC subject identity. Issues an ID token identifying the Funnel user.\n  - name: profile\n    required: false\n    description: Standard OIDC profile claims (name, given_name, family_name, nickname, picture).\n  - name: email\n    required: false\n    description: Standard OIDC email claims (email, email_verified).\n\
  \  - name: offline_access\n    required: false\n    description: >-\n      Issues a refresh token so the MCP client can keep the connection alive without a fresh\n      browser sign-in. Its absence is what surfaces as the \"Connection has expired\" reconnect\n      prompt Funnel documents for Claude.\n- api: Funnel MCP (EU)\n  resource: https://mcp.eu.ai.funnel.io/mcp\n  flow: authorization_code\n  metadata: well-known/funnel-mcp-eu-oauth-protected-resource.json\n  http_status: 200\n  scopes:\n  - name: openid\n  - name: profile\n  - name: email\n  - name: offline_access\n- api: Funnel Control Plane API\n  resource: https://controlplane.setup.us.funnel.io\n  flow: client_credentials\n  scopes: []\n  scopes_note: >-\n    No OAuth scopes are used. The system-user client-credentials grant is authorized by audience\n    (https://controlplane.setup.{us,eu}.funnel.io) and scoped by subscription_id, not by scope\n    strings. See authentication/funnel-authentication.yml.\nauthorization_server_scopes_supported:\n\
  - openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\nauthorization_server_note: >-\n  The list above is what the Auth0 tenant advertises in scopes_supported; only the four scopes in\n  the MCP protected-resource metadata are actually requested for the Funnel MCP resource.\nauthorization_model:\n  granularity: identity-only\n  detail: >-\n    Funnel does not publish any resource- or action-scoped OAuth scopes. Authorization for MCP is\n    entirely delegated to the signed-in Funnel user's own workspace permissions, and the whole MCP\n    surface is read-only by construction. There is therefore no way for a consumer to request a\n    narrower grant than \"everything this user can read\".\nnotes: >-\n  Probed anonymously from the RFC 9728 Protected Resource Metadata documents Funnel serves on both\n  regional MCP hosts. Nothing here is derived from an OpenAPI spec — Funnel\
  \ publishes none.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funnel/refs/heads/main/scopes/funnel-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Data
- Analytics
- Advertising
- Data Integration
- ETL
- Data Warehouse
- Attribution
- Reporting
- Business Intelligence
- MCP
- AI Agents
- Marketing Mix Modeling
token_urls: []
---
