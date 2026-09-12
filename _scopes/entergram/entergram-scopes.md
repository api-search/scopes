---
api_specs:
- filename: entergram-openapi.json
  format: json
  label: Entergram API
  slug: entergram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-openapi.json
authorization_urls: []
description: ''
docs: https://www.entergram.com/help-center/security-developers/claude-mcp-connector
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Entergram Scopes
name_suffix: OAuth Scopes
note: Entergram's REST API authenticates with a workspace-scoped X-API-Key header and declares no OAuth flow in its OpenAPI. OAuth2 (authorization_code + PKCE) is used by the hosted MCP server; the scope set below is served verbatim in the RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata at mcp.entergram.com, and echoed in the 401 WWW-Authenticate challenge from the MCP endpoint. Scopes are workspace-granular read/write pairs plus OIDC scopes.
overview: 'Entergram uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Entergram
provider_slug: entergram
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: entergram-scopes
source_filename: entergram-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: https://mcp.entergram.com/.well-known/oauth-protected-resource\ndocs: https://www.entergram.com/help-center/security-developers/claude-mcp-connector\nnote: >-\n  Entergram's REST API authenticates with a workspace-scoped X-API-Key header and declares no OAuth\n  flow in its OpenAPI. OAuth2 (authorization_code + PKCE) is used by the hosted MCP server; the scope\n  set below is served verbatim in the RFC 8414 authorization-server metadata and RFC 9728\n  protected-resource metadata at mcp.entergram.com, and echoed in the 401 WWW-Authenticate challenge\n  from the MCP endpoint. Scopes are workspace-granular read/write pairs plus OIDC scopes.\nauthorization_server: https://app.entergram.com\nresource: https://mcp.entergram.com/mcp\nscopes:\n- name: workspace.read\n  description: Read workspace metadata.\n- name: members.read\n  description: Read workspace members.\n- name: accounts.read\n  description: Read connected Telegram accounts.\n\
  - name: contacts.read\n  description: Read workspace contacts.\n- name: chats.read\n  description: Read chats and chat metadata.\n- name: chats.write\n  description: Write to chats (e.g. internal comments).\n- name: chat_custom_fields.read\n  description: Read workspace-shared and actor-scoped chat custom field values.\n- name: chat_custom_fields.write\n  description: Write chat custom field values.\n- name: messages.read\n  description: Read Telegram message history.\n- name: messages.write\n  description: Send Telegram messages and fire broadcasts.\n- name: custom_fields.read\n  description: Read custom-column definitions and options.\n- name: custom_fields.write\n  description: Manage custom-column definitions, options and values.\n- name: tickets.read\n  description: Read tickets and ticket comments.\n- name: tickets.write\n  description: Create and update tickets and ticket comments.\n- name: events.read\n  description: Read resumable workspace events.\n- name: offline_access\n  description:\
  \ Issue refresh tokens for long-lived access (authorization-server metadata only).\n- name: openid\n  description: OIDC authentication.\n- name: profile\n  description: OIDC profile claims.\n- name: email\n  description: OIDC email claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/scopes/entergram-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Messaging
- Notifications
- Communications
- CRM
- Telegram
- Customer Support
- Ticketing
- Sales
- MCP
- Webhooks
token_urls: []
---
