---
api_specs:
- filename: whisper-online-openapi.json
  format: json
  label: Whisper API
  slug: whisper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/openapi/whisper-online-openapi.json
authorization_urls: []
description: 'Two permission models. The hosted MCP server is an OAuth 2.1 protected resource: RFC 8414 metadata at https://mcp.whisper.security/.well-known/oauth-authorization-server (fetched 2026-09-19, saved under well-known/) advertises scopes_supported [mcp:read, offline_access, mcp:query], grant types authorization_code + refresh_token, PKCE S256 only, token_endpoint_auth_methods_supported [none], a registration_endpoint (RFC 7591 dynamic client registration) and client_id_metadata_document_supported. The REST control plane uses API-key scopes named in the control-plane docs and the FORBIDDEN_SCOPE error; only the names the provider publishes are listed. The OpenAPI itself declares no oauth2 securityScheme (derive-oauth-scopes.py found none), so this file is searched, not derived.'
docs:
- https://www.whisper.security/docs/ai/mcp/setup
- https://mcp.whisper.security/.well-known/oauth-authorization-server
- https://mcp.whisper.security/.well-known/oauth-protected-resource
- https://whisper.online/docs/control-plane
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Whisper Online Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Whisper Security publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Whisper Security API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Whisper Security
provider_slug: whisper-online
schemes: []
scope_count: 4
scope_names:
- mcp:read
- offline_access
- mcp:query
- mcp:write
scopes:
- description: All seven tools (query, explain_indicator, explain_schema, read_docs, list_workflows, run_workflow, identify), the four resources (whisper://schema/full, whisper://stats, whisper://quota, whisper://server) and the ten prompts — the entire surface; nothing on it can change state.
  flows: []
  scope: mcp:read
- description: A refresh token so the connection survives without another browser round-trip; no additional data access.
  flows: []
  scope: offline_access
- description: Legacy name that grants the same whole surface; documented as "Ask for mcp:read".
  flows: []
  scope: mcp:query
- description: Removed in 2026-08 together with submit_indicator and submit_feedback; no write scope exists.
  flows: []
  scope: mcp:write
slug: whisper-online-scopes
source_filename: whisper-online-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://www.whisper.security/docs/ai/mcp/setup\ndocs:\n- https://www.whisper.security/docs/ai/mcp/setup\n- https://mcp.whisper.security/.well-known/oauth-authorization-server\n- https://mcp.whisper.security/.well-known/oauth-protected-resource\n- https://whisper.online/docs/control-plane\ndescription: >-\n  Two permission models. The hosted MCP server is an OAuth 2.1 protected resource: RFC 8414 metadata at\n  https://mcp.whisper.security/.well-known/oauth-authorization-server (fetched 2026-09-19, saved under\n  well-known/) advertises scopes_supported [mcp:read, offline_access, mcp:query], grant types\n  authorization_code + refresh_token, PKCE S256 only, token_endpoint_auth_methods_supported [none],\n  a registration_endpoint (RFC 7591 dynamic client registration) and client_id_metadata_document_supported.\n  The REST control plane uses API-key scopes named in the control-plane docs and the FORBIDDEN_SCOPE error;\n  only\
  \ the names the provider publishes are listed. The OpenAPI itself declares no oauth2 securityScheme\n  (derive-oauth-scopes.py found none), so this file is searched, not derived.\noauth:\n  issuer: https://mcp.whisper.security\n  authorization_endpoint: https://mcp.whisper.security/oauth/authorize\n  token_endpoint: https://mcp.whisper.security/oauth/token\n  registration_endpoint: https://mcp.whisper.security/oauth/register\n  revocation_endpoint: https://mcp.whisper.security/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  response_types: [code]\n  resource_indicators_supported: true\n  client_id_metadata_document_supported: true\n  default_grant: mcp:read offline_access\n  challenge: 'WWW-Authenticate: Bearer scope=\"mcp:read\" (observed live) — a client that copies the challenge verbatim gets no refresh token; ask for mcp:read offline_access'\n  token_lifetimes:\n    access_token: 1 hour\n \
  \   refresh_token: up to 180 days, rotating on every use\nscopes:\n- scope: mcp:read\n  description: 'All seven tools (query, explain_indicator, explain_schema, read_docs, list_workflows, run_workflow, identify), the four resources (whisper://schema/full, whisper://stats, whisper://quota, whisper://server) and the ten prompts — the entire surface; nothing on it can change state.'\n  surface: hosted MCP\n- scope: offline_access\n  description: A refresh token so the connection survives without another browser round-trip; no additional data access.\n  surface: hosted MCP\n- scope: mcp:query\n  description: Legacy name that grants the same whole surface; documented as \"Ask for mcp:read\".\n  surface: hosted MCP\n  legacy: true\n- scope: mcp:write\n  description: Removed in 2026-08 together with submit_indicator and submit_feedback; no write scope exists.\n  surface: hosted MCP\n  removed: 2026-08\napi_key_scopes:\n  note: 'Static API keys on the MCP connector are not scope-limited (\"a key\
  \ carries whatever its tenant is entitled to\"). On the control plane, \"register, policy, and revoke need admin:dns; the rest need the matching read/write scope\"; DNS rights are granted automatically at signup.'\n  scopes:\n  - scope: admin:dns\n    grants: 'whisper.agents ops register, policy, revoke'\n    source: https://whisper.online/docs/control-plane\n  - scope: dns:logs:read\n    grants: 'whisper.agents op logs'\n    source: 'control-plane docs error example {\"code\":\"FORBIDDEN_SCOPE\",\"message\":\"Missing required scope: dns:logs:read\"}'\n  key_prefixes:\n    whisper.online platform: whisper_live_\n    whisper.security signup (agent-signup docs): whisper-\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whisper-online/refs/heads/main/scopes/whisper-online-scopes.yml
summary_line: 4 scopes
tags:
- Agent Identity
- Agents
- IPv6
- DNS
- DNSSEC
- Threat Intelligence
- Security
- Egress
- A2A
- MCP
- RDAP
- Transparency Log
- Graph Database
- agent-native
- Netherlands
token_urls: []
---
