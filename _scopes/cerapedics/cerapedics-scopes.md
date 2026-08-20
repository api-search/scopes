---
authorization_urls:
- https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cerapedics Scopes
name_suffix: OAuth Scopes
note: Cerapedics publishes no OpenAPI, so 0-working/derive-oauth-scopes.py had nothing to read. These scopes come from the live RFC 9728 protected-resource metadata and the RFC 8414 authorization-server metadata, which are the provider's own published scope declarations. No scopes-reference documentation page exists.
overview: 'Cerapedics publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cerapedics API on a user''s behalf.


  Tokens are issued from https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cerapedics
provider_slug: cerapedics
schemes:
- flows:
  - authorizationUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token
  name: mcp_oauth2
  resource: https://mcp.cerapedics.com/mcp
  source: well-known/cerapedics-oauth-protected-resource.json
scope_count: 4
scope_names:
- https://mcp.cerapedics.com/mcp/user_impersonation
- openid
- profile
- offline_access
scopes:
- description: Delegated access to the Cerapedics MCP server, acting on the signed-in user's behalf. The single resource-specific scope this API declares.
  flows:
  - authorizationCode
  scope: https://mcp.cerapedics.com/mcp/user_impersonation
- description: OpenID Connect sign-in; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the signed-in user.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token so the client can renew access without user interaction.
  flows:
  - authorizationCode
  scope: offline_access
slug: cerapedics-scopes
source_filename: cerapedics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: https://mcp.cerapedics.com/.well-known/oauth-protected-resource\nnote: >-\n  Cerapedics publishes no OpenAPI, so 0-working/derive-oauth-scopes.py had nothing to\n  read. These scopes come from the live RFC 9728 protected-resource metadata and the\n  RFC 8414 authorization-server metadata, which are the provider's own published scope\n  declarations. No scopes-reference documentation page exists.\ndocs: null\nschemes:\n- name: mcp_oauth2\n  source: well-known/cerapedics-oauth-protected-resource.json\n  resource: https://mcp.cerapedics.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token\nscopes:\n- scope: https://mcp.cerapedics.com/mcp/user_impersonation\n  description: Delegated access to the Cerapedics MCP server,\
  \ acting on the signed-in\n    user's behalf. The single resource-specific scope this API declares.\n  kind: resource\n  flows: [authorizationCode]\n  sources: [well-known/cerapedics-oauth-protected-resource.json, well-known/cerapedics-oauth-authorization-server.json]\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token.\n  kind: standard\n  flows: [authorizationCode]\n  sources: [well-known/cerapedics-oauth-authorization-server.json]\n- scope: profile\n  description: Basic profile claims for the signed-in user.\n  kind: standard\n  flows: [authorizationCode]\n  sources: [well-known/cerapedics-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user\n    interaction.\n  kind: standard\n  flows: [authorizationCode]\n  sources: [well-known/cerapedics-oauth-authorization-server.json]\nobservations:\n- >-\n  The scope model is coarse: one blanket user_impersonation scope governs the entire\n\
  \  MCP tool surface, so there is no per-tool or read-vs-write separation an agent\n  runtime could use to constrain what a delegated token may do.\nx-evidence:\n  fetched: '2026-08-02'\n  urls:\n  - {url: 'https://mcp.cerapedics.com/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://mcp.cerapedics.com/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerapedics/refs/heads/main/scopes/cerapedics-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Medical Devices
- Orthopedics
- Orthobiologics
- Bone Graft
- Spine Surgery
- Healthcare
- Life Sciences
- MCP
token_urls:
- https://login.microsoftonline.com/901bf24d-83de-4486-804c-8c263fdb31f4/oauth2/v2.0/token
---
