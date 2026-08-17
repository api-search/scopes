---
authorization_urls: []
description: OAuth scopes advertised by Actively's authorization server (https://auth.actively.ai), which fronts the hosted MCP server at https://api.actively.ai/mcp. The advertised set is the standard OpenID Connect quartet only — there are NO product-specific or resource-scoped permissions published. Whatever authorization Actively applies to per-account agent data is enforced server-side and is not expressed as OAuth scopes a client can request or a reviewer can inspect.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Actively Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Actively uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Actively
provider_slug: actively
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: actively-scopes
source_filename: actively-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.actively.ai/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Actively publishes no scopes/permissions reference page. The scope list below\n  is read verbatim from the authorization server's own scopes_supported array,\n  which is the only published source.\ndescription: >-\n  OAuth scopes advertised by Actively's authorization server\n  (https://auth.actively.ai), which fronts the hosted MCP server at\n  https://api.actively.ai/mcp. The advertised set is the standard OpenID\n  Connect quartet only — there are NO product-specific or resource-scoped\n  permissions published. Whatever authorization Actively applies to\n  per-account agent data is enforced server-side and is not expressed as\n  OAuth scopes a client can request or a reviewer can inspect.\nauthorization_server: https://auth.actively.ai\nresource: https://api.actively.ai/mcp\nscope_count: 4\nscopes:\n- name: openid\n  type: openid-connect\n\
  \  description: >-\n    Standard OIDC scope. Requests an ID token identifying the authenticated\n    Actively user.\n  source: scopes_supported\n- name: profile\n  type: openid-connect\n  description: >-\n    Standard OIDC scope. Grants access to basic profile claims via\n    https://auth.actively.ai/oauth2/userinfo.\n  source: scopes_supported\n- name: email\n  type: openid-connect\n  description: >-\n    Standard OIDC scope. Grants access to the user's email address claim.\n  source: scopes_supported\n- name: offline_access\n  type: openid-connect\n  description: >-\n    Standard OIDC scope. Requests a refresh token so an agent can maintain a\n    long-lived session against the MCP server without re-consent.\n  source: scopes_supported\nfindings:\n- >-\n  NO RESOURCE SCOPES. The MCP resource https://api.actively.ai/mcp is\n  protected, but no scope in the published set names it or any Actively data\n  object (accounts, agents, memory, strategy, research). A client cannot\n  request least-privilege\
  \ access, and a security reviewer cannot tell from the\n  token what an agent is permitted to read or write.\n- >-\n  This matters more than usual for this provider: the product connects\n  autonomous per-account agents to CRM-derived revenue data in third-party AI\n  clients (ChatGPT, Claude, Cowork). Scope granularity is the control surface\n  a customer would use to bound that, and it is not published.\n- >-\n  Publishing resource-specific scopes (e.g. accounts:read, strategy:read,\n  memory:write) in scopes_supported would be a low-cost, high-value addition\n  and is the single clearest gap in an otherwise spec-clean OAuth\n  implementation.\nevidence:\n- fetched: '2026-08-13'\n  url: https://auth.actively.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  quote: '\"scopes_supported\": [\"email\", \"offline_access\", \"openid\", \"profile\"]'\n- fetched: '2026-08-13'\n  url: https://auth.actively.ai/.well-known/openid-configuration\n  http_status: 200\n  quote: '\"scopes_supported\"\
  : [\"email\", \"offline_access\", \"openid\", \"profile\"]'\n- fetched: '2026-08-13'\n  url: https://api.actively.ai/.well-known/oauth-authorization-server\n  http_status: 200\n  note: >-\n    The api-host mirror omits scopes_supported entirely, so the auth host is\n    the authoritative source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actively/refs/heads/main/scopes/actively-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ai Apps
- AI Agents
- Revenue Intelligence
- Sales
- Go To Market
- MCP
- OAuth
- Model Context Protocol
- Sales Intelligence
- Enterprise Software
token_urls: []
---
