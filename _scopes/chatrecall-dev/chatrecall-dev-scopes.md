---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: chat-recall Scopes
name_suffix: OAuth Scopes
note: scopes_supported as advertised by the authorization server metadata; descriptions are the standard OIDC meanings. No product-specific scopes (e.g. read-only vs write tool access) are published.
overview: 'chat-recall publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the chat-recall API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: chat-recall
provider_slug: chatrecall-dev
schemes: []
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Email claim
  flows: []
  scope: email
- description: Refresh token issuance; the connectors doc says "The assistant refreshes its access with a refresh token, and you do not sign in again."
  flows: []
  scope: offline_access
slug: chatrecall-dev-scopes
source_filename: chatrecall-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://chatrecall.dev/.well-known/oauth-authorization-server\nname: chat-recall OAuth scopes\nscopes:\n- name: openid\n  description: OpenID Connect sign-in\n- name: profile\n  description: Basic profile claims\n- name: email\n  description: Email claim\n- name: offline_access\n  description: Refresh token issuance; the connectors doc says \"The assistant refreshes its access with a refresh token, and you do not sign in again.\"\nnote: scopes_supported as advertised by the authorization server metadata; descriptions are the standard OIDC meanings. No product-specific scopes (e.g. read-only vs write tool access) are published.\n"
source_yaml_url: https://artifacts.apis.io/chatrecall-dev/scopes/chatrecall-dev-scopes.yml
summary_line: 4 scopes
tags:
- Company
- AI Coding Assistants
- Developer Tools
- MCP
- Memory
- Search
- Secret Scanning
- Self-Hosted
- Open Source
token_bound: false
token_urls: []
---
