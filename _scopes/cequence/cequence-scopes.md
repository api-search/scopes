---
authorization_urls:
- https://mcp.aigateway.cequence.ai/authorize
description: ''
docs: https://docs.aigateway.cequence.ai/docs/remote-mcp-servers/cequence-ai-gateway
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cequence Scopes
name_suffix: OAuth Scopes
note: Read from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served by the first-party Cequence AI Gateway MCP endpoint. Cequence publishes no standalone scopes reference page. The scope set is the identity-provider scope set (Descope, fronted by Cequence) — it carries WHO the caller is, not WHAT they may do. Actual permission is resolved server-side from the caller's AI Gateway role and Team membership, which is why the docs state that a read-only role receives an authorization error on write tools rather than being refused a scope at the token endpoint. Do not read this list as a permission model.
overview: 'Cequence Security publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cequence Security API on a user''s behalf.


  Tokens are issued from https://mcp.aigateway.cequence.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cequence Security
provider_slug: cequence
schemes:
- flows:
  - authorizationUrl: https://mcp.aigateway.cequence.ai/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.aigateway.cequence.ai/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://mcp.aigateway.cequence.ai
  name: Cequence AI Gateway MCP OAuth
  source: well-known/cequence-oauth-authorization-server.json
scope_count: 5
scope_names:
- openid
- profile
- email
- descope.claims
- descope.custom_claims
scopes:
- description: OpenID Connect — issue an ID token identifying the caller.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated AI Gateway user.
  flows:
  - authorizationCode
  scope: profile
- description: The authenticated user's email address, used as the audit identity on every tool call.
  flows:
  - authorizationCode
  scope: email
- description: Standard claims from the Descope identity provider that backs AI Gateway login.
  flows:
  - authorizationCode
  scope: descope.claims
- description: Tenant-defined custom claims from Descope, the vehicle for role and team assertions.
  flows:
  - authorizationCode
  scope: descope.custom_claims
slug: cequence-scopes
source_filename: cequence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://mcp.aigateway.cequence.ai/.well-known/oauth-authorization-server\ndocs: https://docs.aigateway.cequence.ai/docs/remote-mcp-servers/cequence-ai-gateway\nnote: >-\n  Read from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource\n  metadata served by the first-party Cequence AI Gateway MCP endpoint. Cequence publishes no\n  standalone scopes reference page. The scope set is the identity-provider scope set (Descope,\n  fronted by Cequence) — it carries WHO the caller is, not WHAT they may do. Actual permission\n  is resolved server-side from the caller's AI Gateway role and Team membership, which is why\n  the docs state that a read-only role receives an authorization error on write tools rather\n  than being refused a scope at the token endpoint. Do not read this list as a permission model.\nschemes:\n- name: Cequence AI Gateway MCP OAuth\n  source: well-known/cequence-oauth-authorization-server.json\n\
  \  issuer: https://mcp.aigateway.cequence.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.aigateway.cequence.ai/authorize\n    tokenUrl: https://mcp.aigateway.cequence.ai/token\n    pkce: S256\n  grant_types_supported: [authorization_code, refresh_token]\nscopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token identifying the caller.\n  flows: [authorizationCode]\n  sources: [well-known/cequence-oauth-authorization-server.json]\n- scope: profile\n  description: Basic profile claims for the authenticated AI Gateway user.\n  flows: [authorizationCode]\n  sources: [well-known/cequence-oauth-authorization-server.json]\n- scope: email\n  description: The authenticated user's email address, used as the audit identity on every tool call.\n  flows: [authorizationCode]\n  sources: [well-known/cequence-oauth-authorization-server.json]\n- scope: descope.claims\n  description: Standard claims from the Descope identity provider that backs AI Gateway\
  \ login.\n  flows: [authorizationCode]\n  sources: [well-known/cequence-oauth-authorization-server.json]\n- scope: descope.custom_claims\n  description: Tenant-defined custom claims from Descope, the vehicle for role and team assertions.\n  flows: [authorizationCode]\n  sources: [well-known/cequence-oauth-authorization-server.json]\nauthorization_model:\n  enforced_by: server-side role and team check, not scope\n  roles_named_in_docs: [PlatformOperator, TenantUser, read-only]\n  evidence: https://docs.aigateway.cequence.ai/docs/remote-mcp-servers/cequence-ai-gateway\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence/refs/heads/main/scopes/cequence-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- AI Protection
- API Discovery
- API Security
- Application Security
- Attack Surface
- Bot Management
- Business Logic Abuse
- CNAPP
- Cybersecurity
- Fraud
- Unified API Protection
token_urls:
- https://mcp.aigateway.cequence.ai/token
---
