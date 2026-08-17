---
api_specs:
- filename: improvado-agent-ask-openapi.json
  format: json
  label: Improvado Public Agent Ask API
  slug: improvado-public-agent-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/improvado/refs/heads/main/openapi/improvado-agent-ask-openapi.json
authorization_urls:
- https://report.improvado.io/api/dts/v2/oauth/o/authorize/
description: ''
docs: https://improvado.io/docs-section-topic/improvado-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Improvado Scopes
name_suffix: OAuth Scopes
note: NEW 2026-08-13. The 2026-07-19 round correctly recorded that the Embedded API v3 uses HTTP Basic + Bearer and has no OAuth surface — that is still true of embedded.improvado.io. But Improvado's customer MCP server runs a full OAuth 2.0 authorization server on the tenant domain (report.improvado.io, or a whitelabel domain), and it publishes RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata ANONYMOUSLY. Both were fetched directly; every scope, endpoint and grant type below is read verbatim from those documents, not from prose.
overview: 'Improvado publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Improvado API on a user''s behalf.


  Tokens are issued from https://report.improvado.io/api/dts/v2/oauth/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Improvado
provider_slug: improvado
schemes:
- flows:
  - authorizationUrl: https://report.improvado.io/api/dts/v2/oauth/o/authorize/
    flow: authorizationCode
    pkce:
    - plain
    - S256
    refreshUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/
    tokenUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/
  name: improvadoOAuth
  source: https://report.improvado.io/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 3
scope_names:
- mcp:customer
- mcp:internal
- introspection
scopes:
- description: Customer-facing MCP access. The scope an external AI agent (Claude, ChatGPT/Codex, Gemini CLI, Antigravity, or any MCP client) requests to call the 84-tool Improvado Customer MCP server. This is the scope named in the RFC 9728 protected-resource metadata AND in the 401 WWW-Authenticate challenge returned by the live endpoint.
  flows:
  - authorizationCode
  scope: mcp:customer
- description: Internal MCP access, advertised in the authorization server's scopes_supported. Not referenced in any customer-facing documentation and not accepted by the customer MCP resource (whose scopes_supported lists mcp:customer only). Recorded because the server advertises it; treated as a first-party/internal scope, not a scope a third-party integrator should request.
  flows:
  - authorizationCode
  scope: mcp:internal
- description: Token-introspection scope, advertised in scopes_supported and paired with the RFC 7662 introspection endpoint. Not documented in customer-facing material.
  flows:
  - authorizationCode
  scope: introspection
slug: improvado-scopes
source_filename: improvado-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://report.improvado.io/.well-known/oauth-authorization-server\ndocs: https://improvado.io/docs-section-topic/improvado-mcp\ntype: OAuthScopes\nnote: >-\n  NEW 2026-08-13. The 2026-07-19 round correctly recorded that the Embedded API v3 uses HTTP Basic +\n  Bearer and has no OAuth surface — that is still true of embedded.improvado.io. But Improvado's\n  customer MCP server runs a full OAuth 2.0 authorization server on the tenant domain\n  (report.improvado.io, or a whitelabel domain), and it publishes RFC 8414 authorization-server\n  metadata and RFC 9728 protected-resource metadata ANONYMOUSLY. Both were fetched directly; every\n  scope, endpoint and grant type below is read verbatim from those documents, not from prose.\nauthorization_server:\n  issuer: https://report.improvado.io\n  metadata_url: https://report.improvado.io/.well-known/oauth-authorization-server\n  metadata_file: well-known/improvado-oauth-authorization-server.json\n\
  \  http_status: 200\n  rfc: RFC 8414\n  authorization_endpoint: https://report.improvado.io/api/dts/v2/oauth/o/authorize/\n  token_endpoint: https://report.improvado.io/api/dts/v2/oauth/o/token/\n  revocation_endpoint: https://report.improvado.io/api/dts/v2/oauth/o/revoke_token/\n  introspection_endpoint: https://report.improvado.io/api/dts/v2/oauth/o/introspect/\n  registration_endpoint: https://report.improvado.io/api/dts/v2/oauth/o/register/\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n  code_challenge_methods_supported: [plain, S256]\n  pkce: true\nprotected_resource:\n  resource: https://report.improvado.io/experimental/agent/api/mcp-customer/v1/invoke/\n  metadata_url: https://report.improvado.io/.well-known/oauth-protected-resource/experimental/agent/api/mcp-customer/v1/invoke/\n\
  \  metadata_file: well-known/improvado-oauth-protected-resource.json\n  http_status: 200\n  rfc: RFC 9728\n  authorization_servers: [https://report.improvado.io]\n  bearer_methods_supported: [header]\n  scopes_supported: [mcp:customer]\nschemes:\n- name: improvadoOAuth\n  type: oauth2\n  source: https://report.improvado.io/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://report.improvado.io/api/dts/v2/oauth/o/authorize/\n    tokenUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/\n    refreshUrl: https://report.improvado.io/api/dts/v2/oauth/o/token/\n    pkce: [plain, S256]\nscopes:\n- scope: mcp:customer\n  description: >-\n    Customer-facing MCP access. The scope an external AI agent (Claude, ChatGPT/Codex, Gemini CLI,\n    Antigravity, or any MCP client) requests to call the 84-tool Improvado Customer MCP server. This\n    is the scope named in the RFC 9728 protected-resource metadata AND in the 401 WWW-Authenticate\n\
  \    challenge returned by the live endpoint.\n  flows: [authorizationCode]\n  audience: https://report.improvado.io/experimental/agent/api/mcp-customer/v1/invoke/\n  sources:\n  - https://report.improvado.io/.well-known/oauth-authorization-server\n  - https://report.improvado.io/.well-known/oauth-protected-resource/experimental/agent/api/mcp-customer/v1/invoke/\n  - https://improvado.io/docs-section-topic/improvado-mcp\n  documented_by_provider: true\n  provider_reference: >-\n    Improvado's Gemini CLI setup block instructs users to configure \"oauth\": {\"scopes\": [\"mcp:customer\"]}.\n- scope: mcp:internal\n  description: >-\n    Internal MCP access, advertised in the authorization server's scopes_supported. Not referenced in\n    any customer-facing documentation and not accepted by the customer MCP resource (whose\n    scopes_supported lists mcp:customer only). Recorded because the server advertises it; treated as\n    a first-party/internal scope, not a scope a third-party integrator\
  \ should request.\n  flows: [authorizationCode]\n  sources: [https://report.improvado.io/.well-known/oauth-authorization-server]\n  documented_by_provider: false\n- scope: introspection\n  description: >-\n    Token-introspection scope, advertised in scopes_supported and paired with the RFC 7662\n    introspection endpoint. Not documented in customer-facing material.\n  flows: [authorizationCode]\n  sources: [https://report.improvado.io/.well-known/oauth-authorization-server]\n  documented_by_provider: false\nsession:\n  ttl: 15 minutes\n  backing_store: Redis\n  scope_binding: workspace-scoped\n  source: https://improvado.io/docs-section-topic/improvado-mcp\n  note: >-\n    Improvado documents each MCP session as a workspace-scoped OAuth token with a 15-minute\n    Redis-backed TTL, stating that multi-tenant agent infrastructure maps 1:1 so cross-tenant leakage\n    is prevented by architecture. Distinct from the Embedded API v3's 30-minute Bearer token.\nnot_covered:\n  surface: https://embedded.improvado.io\
  \ (Embedded API v3)\n  reason: >-\n    The Embedded API v3 has no OAuth surface — HTTP Basic for workspace management and token minting,\n    30-minute opaque Bearer tokens for workspace-scoped resources. Its /.well-known/oauth-authorization-server\n    returns 404. See authentication/improvado-authentication.yml.\nx-evidence:\n- fetched: '2026-08-13'\n  url: https://report.improvado.io/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-13'\n  url: https://report.improvado.io/.well-known/oauth-protected-resource/experimental/agent/api/mcp-customer/v1/invoke/\n  http_status: 200\n  content_type: application/json\n- fetched: '2026-08-13'\n  url: https://report.improvado.io/experimental/agent/api/mcp-customer/v1/invoke/\n  http_status: 401\n  note: 'WWW-Authenticate: Bearer resource_metadata=\"...\", scope=\"mcp:customer\"'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/improvado/refs/heads/main/scopes/improvado-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Analytics
- Data Pipeline
- ETL
- Advertising Data
- Business Intelligence
- Data Integration
- AI Agents
- MCP
- Agent Readiness
token_urls:
- https://report.improvado.io/api/dts/v2/oauth/o/token/
---
