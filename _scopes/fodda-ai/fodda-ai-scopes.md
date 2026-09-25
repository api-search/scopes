---
api_specs:
- filename: fodda-ai-openapi.yml
  format: yaml
  label: Fodda Context & Research API
  slug: fodda-context-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/openapi/fodda-ai-openapi.yml
authorization_urls:
- https://clerk.fodda.ai/oauth/authorize
description: ''
docs: https://www.fodda.ai/connect
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Fodda Ai Scopes
name_suffix: OAuth Scopes
note: derive-oauth-scopes.py found no oauth2 scheme in the OpenAPI (the REST contract declares apiKey + bearer SPT only), so this file is built from the provider's published discovery documents. The scopes are identity scopes of the Clerk-delegated authorization server plus the single resource scope "read" advertised by the www-hosted protected-resource document; no per-tool or per-graph scopes are published, and MCP tool authorization is by account/plan rather than scope.
overview: 'Fodda (PSFK) publishes 8 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fodda (PSFK) API on a user''s behalf.


  Tokens are issued from https://clerk.fodda.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fodda (PSFK)
provider_slug: fodda-ai
schemes:
- flows:
  - authorizationUrl: https://clerk.fodda.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://clerk.fodda.ai/oauth/register
    tokenUrl: https://clerk.fodda.ai/oauth/token
  - deviceAuthorizationUrl: https://clerk.fodda.ai/oauth/device_authorization
    flow: deviceCode
    tokenUrl: https://clerk.fodda.ai/oauth/token
  name: oauth2
  source: well-known/fodda-ai-clerk-oauth-authorization-server.json
scope_count: 8
scope_names:
- read
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: Read access to the MCP resource https://mcp.fodda.ai/mcp (scopes_supported in the www-hosted RFC 9728 document; bearer_methods_supported [header]).
  flows:
  - authorizationCode
  scope: read
- description: OpenID Connect authentication (id_token, RS256).
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: 'Profile claims: name, given_name, family_name, picture, preferred_username.'
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: email and email_verified claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Clerk user public metadata.
  flows:
  - authorizationCode
  - deviceCode
  scope: public_metadata
- description: Clerk user private metadata.
  flows:
  - authorizationCode
  - deviceCode
  scope: private_metadata
- description: Issue a refresh token (grant refresh_token supported).
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Read the user's organization membership (org_id claim).
  flows:
  - authorizationCode
  - deviceCode
  scope: user:org:read
slug: fodda-ai-scopes
source_filename: fodda-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: well-known/fodda-ai-clerk-oauth-authorization-server.json + well-known/fodda-ai-clerk-openid-configuration.json\n  + well-known/fodda-ai-www-oauth-protected-resource.json\ndocs: https://www.fodda.ai/connect\nnote: derive-oauth-scopes.py found no oauth2 scheme in the OpenAPI (the REST contract declares apiKey + bearer SPT\n  only), so this file is built from the provider's published discovery documents. The scopes are identity scopes\n  of the Clerk-delegated authorization server plus the single resource scope \"read\" advertised by the www-hosted\n  protected-resource document; no per-tool or per-graph scopes are published, and MCP tool authorization is by account/plan\n  rather than scope.\nschemes:\n- name: oauth2\n  source: well-known/fodda-ai-clerk-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.fodda.ai/oauth/authorize\n    tokenUrl: https://clerk.fodda.ai/oauth/token\n\
  \    pkce: S256\n    registrationUrl: https://clerk.fodda.ai/oauth/register\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://clerk.fodda.ai/oauth/device_authorization\n    tokenUrl: https://clerk.fodda.ai/oauth/token\nscopes:\n- scope: read\n  description: Read access to the MCP resource https://mcp.fodda.ai/mcp (scopes_supported in the www-hosted RFC\n    9728 document; bearer_methods_supported [header]).\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/fodda-ai-www-oauth-protected-resource.json\n  kind: resource\n- scope: openid\n  description: OpenID Connect authentication (id_token, RS256).\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-openid-configuration.json\n  kind: identity\n- scope: profile\n  description: 'Profile claims: name, given_name, family_name, picture, preferred_username.'\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-openid-configuration.json\n  kind: identity\n\
  - scope: email\n  description: email and email_verified claims.\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-openid-configuration.json\n  kind: identity\n- scope: public_metadata\n  description: Clerk user public metadata.\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-oauth-authorization-server.json\n  kind: identity\n- scope: private_metadata\n  description: Clerk user private metadata.\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-oauth-authorization-server.json\n  kind: identity\n- scope: offline_access\n  description: Issue a refresh token (grant refresh_token supported).\n  flows:\n  - authorizationCode\n  - deviceCode\n  sources:\n  - well-known/fodda-ai-clerk-oauth-authorization-server.json\n  kind: identity\n- scope: user:org:read\n  description: Read the user's organization membership (org_id claim).\n  flows:\n  - authorizationCode\n  - deviceCode\n\
  \  sources:\n  - well-known/fodda-ai-clerk-oauth-authorization-server.json\n  kind: identity\nclaims_supported:\n- sub\n- iss\n- aud\n- exp\n- iat\n- email\n- email_verified\n- name\n- given_name\n- family_name\n- picture\n- preferred_username\n- org_id\ngaps: No scope-to-tool or scope-to-graph mapping is published; the protected-resource documents on mcp.fodda.ai\n  list no scopes at all (only authorization_servers).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fodda-ai/refs/heads/main/scopes/fodda-ai-scopes.yml
summary_line: 8 scopes · authorizationCode/deviceCode
tags:
- Market Intelligence
- Trend Research
- Knowledge Graph
- Consumer Insights
- Earnings Intelligence
- Brand Intelligence
- Research
- Institutional Data
- MCP
- A2A
- Agent-Native
- Machine Payments
- Company
token_urls:
- https://clerk.fodda.ai/oauth/token
---
