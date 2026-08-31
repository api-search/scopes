---
authorization_urls: []
description: ''
docs: https://ec-force.com/information/20260804
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Super Studio Scopes
name_suffix: OAuth Scopes
note: 'Read directly from the ecforce AI MCP authorization server''s RFC 8414 metadata, which is served anonymously. The server advertises exactly one scope. No scopes/permissions reference page is published — the ecforce v2 REST API uses a member-permission model configured per API connection user in the admin screens rather than OAuth scopes, and that configuration is behind the tenant login. derive-oauth-scopes.py was not applicable: there is no OpenAPI in this repo to derive from.'
overview: 'SUPER STUDIO uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SUPER STUDIO
provider_slug: super-studio
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: super-studio-scopes
source_filename: super-studio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://agent.ec-force.com/.well-known/oauth-authorization-server\ndocs: https://ec-force.com/information/20260804\nnote: >-\n  Read directly from the ecforce AI MCP authorization server's RFC 8414 metadata, which is served\n  anonymously. The server advertises exactly one scope. No scopes/permissions reference page is\n  published — the ecforce v2 REST API uses a member-permission model configured per API connection\n  user in the admin screens rather than OAuth scopes, and that configuration is behind the tenant\n  login. derive-oauth-scopes.py was not applicable: there is no OpenAPI in this repo to derive from.\nauthorization_server: https://agent.ec-force.com\nflows:\n- type: authorization_code\n  authorization_url: https://agent.ec-force.com/mcp/oauth/authorize\n  token_url: https://agent.ec-force.com/mcp/oauth/token\n  refresh_supported: true\n  pkce: S256\n  dynamic_client_registration: https://agent.ec-force.com/mcp/oauth/register\n\
  scopes:\n- name: mcp\n  description: >-\n    The single scope advertised by the ecforce AI MCP authorization server. Effective authority is\n    not carried in the scope string: the provider states access is bounded by the ecforce services\n    the tenant has contracted and by the signed-in ecforce account's own permission scope, so two\n    tokens carrying \"mcp\" can reach different data.\n  source: oauth-authorization-server metadata\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-studio/refs/heads/main/scopes/super-studio-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- E-Commerce
- Commerce
- Subscription Commerce
- Order Management
- Marketing Automation
- Business Intelligence
- SaaS
- Artificial Intelligence
- Agents
- MCP
- Japan
token_urls: []
---
