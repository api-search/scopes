---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Agentsmyth Scopes
name_suffix: OAuth Scopes
note: Read from the provider's live OIDC discovery document, not from an OpenAPI - no OpenAPI is published. These are the only scopes the authorization server advertises. They are the standard OIDC identity set; no resource- or product-specific scopes (no read/write, no per-agent scopes) are published, so an agent cannot request least-privilege access to a named capability. If finer-grained scopes exist they are not in the public metadata.
overview: 'AgentSmyth uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AgentSmyth
provider_slug: agentsmyth
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: agentsmyth-scopes
source_filename: agentsmyth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://app.auth.agentsmyth.com/.well-known/openid-configuration\nnote: >-\n  Read from the provider's live OIDC discovery document, not from an OpenAPI - no OpenAPI is\n  published. These are the only scopes the authorization server advertises. They are the standard\n  OIDC identity set; no resource- or product-specific scopes (no read/write, no per-agent scopes)\n  are published, so an agent cannot request least-privilege access to a named capability. If\n  finer-grained scopes exist they are not in the public metadata.\ndocs: null\ndocs_note: No public scopes or permissions reference page exists.\nauthorization_server: https://app.auth.agentsmyth.com\nscope_count: 4\nscopes:\n- name: openid\n  description: Standard OIDC scope requesting an ID token for the authenticated subject.\n  category: identity\n- name: profile\n  description: Standard OIDC scope granting access to basic profile claims.\n  category: identity\n- name:\
  \ email\n  description: Standard OIDC scope granting access to the subject's email address claim.\n  category: identity\n- name: offline_access\n  description: >-\n    Standard OAuth scope requesting a refresh token for long-lived, unattended access - the scope an\n    agent needs to keep working without a human re-authorizing.\n  category: session\nresource_scopes:\n- resource: https://api.agentsmyth.com/mcp\n  scopes_supported:\n  - openid\n  - offline_access\n  - email\n  - profile\n  source: https://api.agentsmyth.com/.well-known/oauth-protected-resource/mcp\nx-evidence:\n  fetched: '2026-09-12'\n  probes:\n  - url: https://app.auth.agentsmyth.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://api.agentsmyth.com/.well-known/oauth-protected-resource/mcp\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentsmyth/refs/heads/main/scopes/agentsmyth-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Financial-Services
- Capital Markets
- Artificial Intelligence
- AI Agents
- Trading
- Investment Research
- Market Intelligence
- MCP
- agent-native
- Fintech
token_urls: []
---
