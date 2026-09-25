---
api_specs:
- filename: lvlltd-com-openapi.yml
  format: yaml
  label: LVL LTD Agent Skill Market API
  slug: lvl-ltd-agent-skill-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lvlltd-com/refs/heads/main/openapi/lvlltd-com-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Lvlltd Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LVL LTD CO publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the LVL LTD CO API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LVL LTD CO
provider_slug: lvlltd-com
schemes:
- authorization_server_metadata: absent (RFC 8414 404; OIDC discovery 404) — verified 2026-09-19
  authorization_servers:
  - https://lvlltd.com
  bearer_methods_supported:
  - header
  flows: []
  name: declared-by-protected-resource-metadata
  resource: https://lvlltd.com
  source: well-known/lvlltd-com-oauth-protected-resource.json
scope_count: 4
scope_names:
- agent:read
- agent:execute
- x402:pay
- openid
scopes:
- description: ''
  flows: []
  scope: agent:read
- description: ''
  flows: []
  scope: agent:execute
- description: ''
  flows: []
  scope: x402:pay
- description: ''
  flows: []
  scope: openid
slug: lvlltd-com-scopes
source_filename: lvlltd-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://lvlltd.com/.well-known/oauth-protected-resource (RFC 9728 document, saved as well-known/lvlltd-com-oauth-protected-resource.json)\ndocs: null\nsummary: >-\n  LVL LTD publishes an OAuth scope LIST but no OAuth server. The RFC 9728 protected-resource document on\n  the apex declares four scopes_supported and names https://lvlltd.com as its authorization server, yet\n  that host serves neither /.well-known/oauth-authorization-server (404) nor\n  /.well-known/openid-configuration (404), the OpenAPI declares no oauth2 securityScheme, and no docs page\n  explains how a token would be obtained or which operation would accept one. derive-oauth-scopes.py\n  therefore found nothing in the spec. The scopes are recorded here because the provider published them;\n  they are, today, unobtainable.\nschemes:\n- name: declared-by-protected-resource-metadata\n  source: well-known/lvlltd-com-oauth-protected-resource.json\n  resource:\
  \ https://lvlltd.com\n  authorization_servers: [https://lvlltd.com]\n  authorization_server_metadata: absent (RFC 8414 404; OIDC discovery 404) — verified 2026-09-19\n  bearer_methods_supported: [header]\n  flows: []\nscopes:\n- scope: agent:read\n  description: null\n  flows: []\n  sources: [well-known/lvlltd-com-oauth-protected-resource.json]\n  obtainable: false\n- scope: agent:execute\n  description: null\n  flows: []\n  sources: [well-known/lvlltd-com-oauth-protected-resource.json]\n  obtainable: false\n- scope: x402:pay\n  description: null\n  flows: []\n  sources: [well-known/lvlltd-com-oauth-protected-resource.json]\n  obtainable: false\n  note: The capability this scope names is in fact exercised without any token — by the X-PAYMENT / PAYMENT-SIGNATURE payment proof on POST /api/pay (see authentication/).\n- scope: openid\n  description: null\n  flows: []\n  sources: [well-known/lvlltd-com-oauth-protected-resource.json]\n  obtainable: false\nfinding: >-\n  A dangling delegated-identity\
  \ declaration: the resource document is the half of RFC 9728 a resource\n  server publishes, and it is well-formed, but the authorization-server half it points at does not\n  exist. An MCP client following the 2025-06-18 authorization flow would fetch this document, follow\n  authorization_servers[0], and fail at the metadata step.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lvlltd-com/refs/heads/main/scopes/lvlltd-com-scopes.yml
summary_line: 4 scopes
tags:
- Agents
- Agentic Commerce
- Agent Skills
- A2A
- MCP
- x402
- Micropayments
- Stablecoins
- Marketplace
- Agent-Native
- United States
token_urls: []
---
