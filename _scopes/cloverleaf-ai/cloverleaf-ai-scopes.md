---
authorization_urls:
- https://auth.cloverleaf.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cloverleaf Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cloverleaf AI publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cloverleaf AI API on a user''s behalf.


  Tokens are issued from https://auth.cloverleaf.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cloverleaf AI
provider_slug: cloverleaf-ai
schemes:
- authorization_servers:
  - https://auth.cloverleaf.ai/
  flows:
  - authorizationUrl: https://auth.cloverleaf.ai/authorize
    flow: authorizationCode
    tokenUrl: https://auth.cloverleaf.ai/oauth/token
  name: mcp-oauth2
  resource: https://mcp.cloverleaf.ai/
  source: well-known/cloverleaf-ai-oauth-protected-resource.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, nickname, picture).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and verification status claims.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the agent session survives access-token expiry.
  flows:
  - authorizationCode
  scope: offline_access
slug: cloverleaf-ai-scopes
source_filename: cloverleaf-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource,\n  https://auth.cloverleaf.ai/.well-known/openid-configuration\n\n# No OpenAPI exists to derive scopes from; these are read straight from the live\n# OAuth/OIDC discovery documents. Cloverleaf AI publishes no scopes reference page.\n\nschemes:\n- name: mcp-oauth2\n  source: well-known/cloverleaf-ai-oauth-protected-resource.json\n  resource: https://mcp.cloverleaf.ai/\n  authorization_servers: [https://auth.cloverleaf.ai/]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.cloverleaf.ai/authorize\n    tokenUrl: https://auth.cloverleaf.ai/oauth/token\n\n# Scopes the MCP protected resource declares it accepts (RFC 9728 scopes_supported).\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/cloverleaf-ai-oauth-protected-resource.json]\n- scope: profile\n\
  \  description: Basic profile claims (name, nickname, picture).\n  flows: [authorizationCode]\n  sources: [well-known/cloverleaf-ai-oauth-protected-resource.json]\n- scope: email\n  description: Email address and verification status claims.\n  flows: [authorizationCode]\n  sources: [well-known/cloverleaf-ai-oauth-protected-resource.json]\n- scope: offline_access\n  description: Issue a refresh token so the agent session survives access-token expiry.\n  flows: [authorizationCode]\n  sources: [well-known/cloverleaf-ai-oauth-protected-resource.json]\n\nfinding: >-\n  The MCP server declares ONLY the four standard OIDC/OAuth identity scopes. There is no\n  resource-scoped permission vocabulary — nothing like read:meetings, read:opportunities\n  or write:salesforce — so the token an agent obtains carries no least-privilege signal\n  about which Cloverleaf AI data or tools it may reach. Authorization is therefore\n  enforced entirely server-side against the authenticated user's tenant entitlements.\n\
  \  This is a genuine gap in the contract, recorded rather than papered over: it is the\n  single most useful thing the provider could publish next for agent consumers.\n\nx-evidence:\n- url: https://mcp.cloverleaf.ai/.well-known/oauth-protected-resource\n  http_status: 200\n- url: https://auth.cloverleaf.ai/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloverleaf-ai/refs/heads/main/scopes/cloverleaf-ai-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Government
- B2G
- Sales Intelligence
- Public Sector
- GovTech
- Procurement
- RFP
- Legislative Intelligence
- Speech to Text
- Artificial Intelligence
token_urls:
- https://auth.cloverleaf.ai/oauth/token
---
