---
api_specs:
- filename: agent-ready-dev-openapi.yml
  format: yaml
  label: Agent Ready API
  slug: agent-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/openapi/agent-ready-dev-openapi.yml
authorization_urls: []
description: ''
docs: https://agent-ready.dev/auth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Agent Ready Dev Scopes
name_suffix: OAuth Scopes
note: 'The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py found zero), so this file is built from the provider''s own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, which both advertise scopes_supported. IMPORTANT: the scopes are ADVERTISED, NOT ENFORCED — /auth states there is no OAuth flow, keys are long-lived ar_live_ Bearer secrets issued from the dashboard, and access is decided by plan tier (Free vs Pro) rather than by scope. A token never carries a scope, and a 403 for a plan mismatch is reported as insufficient_scope. Recorded as the provider''s declared permission vocabulary.'
overview: 'Agent Ready publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agent Ready API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agent Ready
provider_slug: agent-ready-dev
schemes:
- authorization_server_metadata: well-known/agent-ready-dev-oauth-authorization-server.json
  bearerFormat: ar_live_<prefix>_<secret>
  bearer_methods_supported:
  - header
  dynamic_client_registration: false
  grant_types_supported:
  - urn:ietf:params:oauth:grant-type:api-key
  issuance: human-mediated at https://agent-ready.dev/dashboard/api-keys (Pro plan)
  name: ApiKey (Bearer)
  protected_resource_metadata: well-known/agent-ready-dev-oauth-protected-resource.json
  response_types_supported:
  - none
  revocation: dashboard only (no RFC 7009 endpoint)
  scheme: bearer
  source: openapi/agent-ready-dev-openapi.yml
  token_endpoint_auth_methods_supported:
  - none
  type: http
scope_count: 4
scope_names:
- scan:read
- scan:write
- ask:read
- mcp
scopes:
- description: Read scans — GET /api/v1/scans/{id}, GET /api/v1/scans, the get_scan MCP tool and A2A tasks/get. (Description inferred from the operation surface; the metadata publishes names only.)
  flows: []
  scope: scan:read
- description: Start scans — POST /api/v1/scans and the scan_site MCP tool / A2A skill.
  flows: []
  scope: scan:write
- description: The NLWeb /api/v1/ask endpoint and the ask tool/skill — public today, no key required.
  flows: []
  scope: ask:read
- description: Access to the hosted MCP endpoint https://agent-ready.dev/api/v1/mcp (the resource named in the protected-resource metadata).
  flows: []
  scope: mcp
slug: agent-ready-dev-scopes
source_filename: agent-ready-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://agent-ready.dev/.well-known/oauth-authorization-server\ndocs: https://agent-ready.dev/auth\nnote: >-\n  The OpenAPI declares no oauth2 securityScheme (derive-oauth-scopes.py found zero), so this file is built from\n  the provider's own RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata, which\n  both advertise scopes_supported. IMPORTANT: the scopes are ADVERTISED, NOT ENFORCED — /auth states there is\n  no OAuth flow, keys are long-lived ar_live_ Bearer secrets issued from the dashboard, and access is decided\n  by plan tier (Free vs Pro) rather than by scope. A token never carries a scope, and a 403 for a plan mismatch\n  is reported as insufficient_scope. Recorded as the provider's declared permission vocabulary.\nschemes:\n- name: ApiKey (Bearer)\n  type: http\n  scheme: bearer\n  bearerFormat: ar_live_<prefix>_<secret>\n  source: openapi/agent-ready-dev-openapi.yml\n  issuance: human-mediated\
  \ at https://agent-ready.dev/dashboard/api-keys (Pro plan)\n  authorization_server_metadata: well-known/agent-ready-dev-oauth-authorization-server.json\n  protected_resource_metadata: well-known/agent-ready-dev-oauth-protected-resource.json\n  grant_types_supported: [urn:ietf:params:oauth:grant-type:api-key]\n  token_endpoint_auth_methods_supported: [none]\n  response_types_supported: [none]\n  bearer_methods_supported: [header]\n  dynamic_client_registration: false\n  revocation: dashboard only (no RFC 7009 endpoint)\nscopes:\n- scope: scan:read\n  description: Read scans — GET /api/v1/scans/{id}, GET /api/v1/scans, the get_scan MCP tool and A2A tasks/get. (Description inferred from the operation surface; the metadata publishes names only.)\n  sources: [well-known/agent-ready-dev-oauth-authorization-server.json, well-known/agent-ready-dev-oauth-protected-resource.json]\n  enforced: false\n- scope: scan:write\n  description: Start scans — POST /api/v1/scans and the scan_site MCP tool /\
  \ A2A skill.\n  sources: [well-known/agent-ready-dev-oauth-authorization-server.json, well-known/agent-ready-dev-oauth-protected-resource.json]\n  enforced: false\n- scope: ask:read\n  description: The NLWeb /api/v1/ask endpoint and the ask tool/skill — public today, no key required.\n  sources: [well-known/agent-ready-dev-oauth-authorization-server.json, well-known/agent-ready-dev-oauth-protected-resource.json]\n  enforced: false\n- scope: mcp\n  description: Access to the hosted MCP endpoint https://agent-ready.dev/api/v1/mcp (the resource named in the protected-resource metadata).\n  sources: [well-known/agent-ready-dev-oauth-authorization-server.json, well-known/agent-ready-dev-oauth-protected-resource.json]\n  enforced: false\neffective_permission_model:\n  basis: plan tier\n  tiers:\n    anonymous: ask, scanMcp, x402 lane, POST /api/scan (3 scans / 30 days per IP), MCP Apps endpoint tools/call\n    free_signed_in: web scans only (10 / 30 days); cannot mint API keys\n    pro: ar_live_\
  \ key — startScan, getScan, listScans, hosted MCP tools/call, A2A scan_site / tasks/get\n  docs: https://agent-ready.dev/pricing\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agent-ready-dev/refs/heads/main/scopes/agent-ready-dev-scopes.yml
summary_line: 4 scopes
tags:
- Agents
- Agent Readiness
- Website Scanning
- Developer Tools
- MCP
- A2A
- llms-txt
- x402
- NLWeb
- Accessibility
- Agent-Native
- Australia
token_urls: []
---
