---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tarx Com Scopes
name_suffix: OAuth Scopes
note: The scope names come verbatim from the provider's RFC 8414 / RFC 9728 metadata. No scopes reference page was found on docs.tarx.com or howdy.tarx.com, so descriptions are recorded only where a provider document states the meaning; the rest are null rather than guessed. ai-plugin.json requests scope "user" for the ChatGPT connector.
overview: 'TARXAN uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TARXAN
provider_slug: tarx-com
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tarx-com-scopes
source_filename: tarx-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp.tarx.com/.well-known/oauth-authorization-server (scopes_supported) + https://mcp.tarx.com/.well-known/oauth-protected-resource\ndocs: null\nissuer: https://mcp.tarx.com\nresource: https://mcp.tarx.com/mcp\nnote: >-\n  The scope names come verbatim from the provider's RFC 8414 / RFC 9728 metadata. No scopes reference\n  page was found on docs.tarx.com or howdy.tarx.com, so descriptions are recorded only where a\n  provider document states the meaning; the rest are null rather than guessed. ai-plugin.json\n  requests scope \"user\" for the ChatGPT connector.\nscope_count: 3\nscopes:\n- name: public\n  description: null\n  evidence: Named in scopes_supported. The anonymous MCP surface (public-safe tools, tarx://system resources) is what the provider calls \"public context\" in mcp.json.\n- name: user\n  description: null\n  evidence: Named in scopes_supported; requested by /.well-known/ai-plugin.json (auth.scope \"user\"\
  ) for the ChatGPT connector.\n- name: chatgpt_private_memory\n  description: null\n  evidence: Named in scopes_supported. mcp.json describes \"private memory reads and writes require OAuth/Bearer auth\" and names ChatGPT as a target client; the scope name pairs the two, but no document defines it.\ntool_gating_observed:\n- {tool: tarx_memory_search, anonymous: denied, message: Authentication required for private memory reads. Provide a Bearer token.}\n- {tool: tarx_status, anonymous: allowed}\n- {tool: tarx_skills_list, anonymous: allowed}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tarx-com/refs/heads/main/scopes/tarx-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AI Agents
- Agent Runtime
- Local-First AI
- Private AI
- MCP
- A2A
- LLM
- Inference
- Developer Tools
- Hardware
- Robotics
token_urls: []
---
