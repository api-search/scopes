---
api_specs:
- filename: airia-openapi.yml
  format: yaml
  label: Airia Web APIs
  slug: airia-web-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/openapi/airia-openapi.yml
authorization_urls: []
description: OAuth scopes Airia publishes. These come from the MCP Gateway's RFC 9728 protected-resource metadata and the Keycloak realm's OpenID discovery document, both fetched anonymously — not from the REST OpenAPI, which declares only apiKey schemes (X-API-Key and a session cookie) and no oauth2 securityScheme at all. So the platform REST API is not scope-governed; the MCP Gateway is. Access to the REST API is instead governed by ROLES bound to a key, which are resolved live on every request; the role/permission vocabulary is documented in the console's permissions reference and is not published anonymously.
docs: https://airia.ai/docs/settings/developer/api-keys
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Airia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Airia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airia
provider_slug: airia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: airia-scopes
source_filename: airia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://mcp-gateway.airia.ai/.well-known/oauth-protected-resource\ndocs: https://airia.ai/docs/settings/developer/api-keys\ndescription: >-\n  OAuth scopes Airia publishes. These come from the MCP Gateway's RFC 9728 protected-resource\n  metadata and the Keycloak realm's OpenID discovery document, both fetched anonymously — not from\n  the REST OpenAPI, which declares only apiKey schemes (X-API-Key and a session cookie) and no\n  oauth2 securityScheme at all. So the platform REST API is not scope-governed; the MCP Gateway is.\n  Access to the REST API is instead governed by ROLES bound to a key, which are resolved live on\n  every request; the role/permission vocabulary is documented in the console's permissions reference\n  and is not published anonymously.\nauthorization_servers:\n- issuer: https://mcp-gateway.airia.ai\n  metadata: well-known/airia-mcp-gateway-oauth-authorization-server.json\n  authorization_endpoint: https://identity.airia.ai/auth/realms/airia/protocol/openid-connect/auth\n\
  \  token_endpoint: https://identity.airia.ai/auth/realms/airia/protocol/openid-connect/token\n  registration_endpoint: https://mcp-gateway.airia.ai/.well-known/oauth-authorization-server/v1/register\n  pkce: S256\n- issuer: https://identity.airia.ai/auth/realms/airia\n  metadata: well-known/airia-identity-openid-configuration.json\n  registration_endpoint: https://identity.airia.ai/auth/realms/airia/clients-registrations/openid-connect\nresources:\n- resource: https://mcp-gateway.airia.ai\n  metadata: well-known/airia-mcp-gateway-oauth-protected-resource.json\n  bearer_methods_supported:\n  - header\n- resource: https://prodaus.mcp-gateway.airia.ai\n  metadata: well-known/airia-prodaus-mcp-gateway-oauth-protected-resource.json\n  note: Australian regional gateway; identical scope set.\nscopes:\n- name: mcp.read\n  description: Read access to the MCP Gateway — list and inspect the tools, resources and skills a gateway exposes.\n  source: https://mcp-gateway.airia.ai/.well-known/oauth-protected-resource\n\
  - name: mcp.write\n  description: Invoke tools through the MCP Gateway.\n  source: https://mcp-gateway.airia.ai/.well-known/oauth-protected-resource\n- name: openid\n  description: Standard OIDC scope; issues an ID token.\n- name: profile\n  description: Standard OIDC profile claims.\n- name: email\n  description: Standard OIDC email claim.\n- name: address\n  description: Standard OIDC address claim.\n- name: phone\n  description: Standard OIDC phone claim.\n- name: roles\n  description: Keycloak realm/client roles claim — the roles that decide what a token can do inside Airia.\n- name: groups\n  description: Keycloak group membership claim.\n- name: active_organization\n  description: The tenant/organization the token is currently acting within.\n- name: enterprise\n  description: Airia enterprise client scope.\n- name: basic\n  description: Keycloak basic scope (sub, auth_time).\n- name: acr\n  description: Authentication context class reference.\n- name: web-origins\n  description:\
  \ Keycloak CORS origins scope.\n- name: microprofile-jwt\n  description: MicroProfile JWT claims (upn, groups).\nidentity_realm_only_scopes:\n- name: airia-knowledge\n  description: >-\n    Present on the identity.airia.ai realm but NOT in the MCP Gateway's advertised scope set —\n    knowledge/retrieval access issued to first-party surfaces.\n  source: https://identity.airia.ai/auth/realms/airia/.well-known/openid-configuration\n- name: service_account\n  description: Client-credentials service-account scope on the realm, not offered through the gateway.\n  source: https://identity.airia.ai/auth/realms/airia/.well-known/openid-configuration\nrest_api_authorization:\n  model: roles-on-api-key\n  note: >-\n    Not OAuth scopes. A key is created with either no roles (a personal access token carrying the\n    creating user's permissions) or one or more roles (a service account). Permissions are resolved\n    fresh on every request from those roles, Platform Admin can never be assigned to\
  \ a key, and a\n    key cannot be issued with more permission than its creator holds at creation time.\n  docs: https://airia.ai/docs/settings/developer/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airia/refs/heads/main/scopes/airia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Enterprise AI
- AI Agents
- AI Governance
- AI Security
- MCP
- MCP Gateway
- Agent Orchestration
- LLM Gateway
- AI Discovery
- Red Teaming
- Guardrails
- Knowledge Retrieval
- RAG
- Agent-Native
token_urls: []
---
