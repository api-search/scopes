---
api_specs:
- filename: karumi-public-api-openapi.json
  format: json
  label: Karumi Public API
  slug: karumi-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/openapi/karumi-public-api-openapi.json
authorization_urls:
- https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/authorize
description: ''
docs: https://www.karumi.ai/mcp-documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Karumi Scopes
name_suffix: OAuth Scopes
note: 'Karumi''s OpenAPI declares no oauth2 security scheme — the Public API is API-key only. The OAuth surface belongs to the MCP server, which advertises RFC 9728 protected-resource metadata and delegates to a Supabase Auth authorization server. The scopes below are read verbatim from that authorization server''s RFC 8414 metadata (scopes_supported). They are Supabase''s standard OIDC scope set, NOT Karumi-defined permissions: Karumi publishes no scope or permission reference page. Per-tool authorization is instead enforced two ways — server-side organization scoping ("access is scoped to the organization(s) your account belongs to") and client-side confirmation on the 13 write/destructive tools. That confirmation model is captured in mcp/karumi-mcp.yml, not here.'
overview: 'Karumi publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Karumi API on a user''s behalf.


  Tokens are issued from https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Karumi
provider_slug: karumi
schemes:
- authorization_server: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1
  flows:
  - authorizationUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/authorize
    code_challenge_methods:
    - S256
    - plain
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    tokenUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token
  name: OAuth2
  resource: https://api.karumi.ai/mcp
  sources:
  - well-known/karumi-oauth-authorization-server.json
  type: oauth2
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- offline_access
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the Karumi user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, picture, preferred_username, updated_at).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Phone number and phone_number_verified claim.
  flows:
  - authorizationCode
  scope: phone
- description: Issues a refresh token so the MCP client can keep the connector alive without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
slug: karumi-scopes
source_filename: karumi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.karumi.ai/.well-known/oauth-protected-resource\ndocs: https://www.karumi.ai/mcp-documentation\napplies_to: Karumi MCP Server (https://api.karumi.ai/mcp/)\nnote: >-\n  Karumi's OpenAPI declares no oauth2 security scheme — the Public API is API-key only.\n  The OAuth surface belongs to the MCP server, which advertises RFC 9728\n  protected-resource metadata and delegates to a Supabase Auth authorization server.\n  The scopes below are read verbatim from that authorization server's RFC 8414 metadata\n  (scopes_supported). They are Supabase's standard OIDC scope set, NOT Karumi-defined\n  permissions: Karumi publishes no scope or permission reference page. Per-tool\n  authorization is instead enforced two ways — server-side organization scoping (\"access\n  is scoped to the organization(s) your account belongs to\") and client-side confirmation\n  on the 13 write/destructive tools. That confirmation model is captured\
  \ in\n  mcp/karumi-mcp.yml, not here.\nschemes:\n- name: OAuth2\n  type: oauth2\n  authorization_server: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1\n  resource: https://api.karumi.ai/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token\n    code_challenge_methods:\n    - S256\n    - plain\n    grant_types:\n    - authorization_code\n    - refresh_token\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the Karumi\n    user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\n- scope: profile\n  description: Basic profile claims (name, picture, preferred_username, updated_at).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\n\
  - scope: email\n  description: Email address and email_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\n- scope: phone\n  description: Phone number and phone_number_verified claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\n- scope: offline_access\n  description: Issues a refresh token so the MCP client can keep the connector alive\n    without re-consent.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/karumi-oauth-authorization-server.json\ngaps:\n- No Karumi-specific resource scopes (e.g. sessions:read, audiences:write) are published,\n  so an MCP client cannot request least-privilege access to a subset of the 37 tools.\n- No scopes/permissions reference page exists on karumi.ai.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karumi/refs/heads/main/scopes/karumi-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- AI Agents
- Product Demos
- Sales Enablement
- Go-To-Market
- SaaS
- Conversational AI
- Video
- Y Combinator
- mcp
- agent-native
- analytics
- conversation-intelligence
token_urls:
- https://qmfmxcidbawbvkcstvio.supabase.co/auth/v1/oauth/token
---
