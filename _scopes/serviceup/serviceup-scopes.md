---
authorization_urls:
- https://auth.serviceup.com/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Serviceup Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from the OAuth metadata ServiceUp serves anonymously. ServiceUp publishes no scopes/permissions reference page, so there are no descriptions to enrich from — the descriptions below state only what the scope name and its RFC 9728 resource binding assert, and are marked accordingly.
overview: 'ServiceUp publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ServiceUp API on a user''s behalf.


  Tokens are issued from https://auth.serviceup.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ServiceUp
provider_slug: serviceup
schemes:
- flows:
  - authorizationUrl: https://auth.serviceup.com/api/auth/oauth2/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://auth.serviceup.com/api/auth/oauth2/token
  name: ServiceUpOAuth2
  source: well-known/serviceup-oauth-authorization-server.json
scope_count: 3
scope_names:
- mcp:read
- mcp:write
- offline_access
scopes:
- description: Read access to the ServiceUp MCP server resource (scope name only; no published description).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access to the ServiceUp MCP server resource (scope name only; no published description).
  flows:
  - authorizationCode
  scope: mcp:write
- description: Standard OAuth 2.0 offline access scope (RFC 6749 / OIDC Core), requesting a refresh token. Advertised by the authorization server but not listed on the MCP protected-resource metadata.
  flows:
  - authorizationCode
  scope: offline_access
slug: serviceup-scopes
source_filename: serviceup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://api.serviceup.com/.well-known/oauth-protected-resource/mcp\ndocs: null\nnote: >-\n  Scopes are taken verbatim from the OAuth metadata ServiceUp serves anonymously.\n  ServiceUp publishes no scopes/permissions reference page, so there are no\n  descriptions to enrich from — the descriptions below state only what the scope\n  name and its RFC 9728 resource binding assert, and are marked accordingly.\nschemes:\n- name: ServiceUpOAuth2\n  source: well-known/serviceup-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.serviceup.com/api/auth/oauth2/authorize\n    tokenUrl: https://auth.serviceup.com/api/auth/oauth2/token\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: mcp:read\n  description: Read access to the ServiceUp MCP server resource (scope name only; no published description).\n  description_source: scope-name\n  flows:\n  - authorizationCode\n  resources:\n\
  \  - https://api.serviceup.com/mcp\n  sources:\n  - well-known/serviceup-oauth-protected-resource-mcp.json\n  - well-known/serviceup-oauth-authorization-server.json\n- scope: mcp:write\n  description: Write access to the ServiceUp MCP server resource (scope name only; no published description).\n  description_source: scope-name\n  flows:\n  - authorizationCode\n  resources:\n  - https://api.serviceup.com/mcp\n  sources:\n  - well-known/serviceup-oauth-protected-resource-mcp.json\n  - well-known/serviceup-oauth-authorization-server.json\n- scope: offline_access\n  description: >-\n    Standard OAuth 2.0 offline access scope (RFC 6749 / OIDC Core), requesting a\n    refresh token. Advertised by the authorization server but not listed on the\n    MCP protected-resource metadata.\n  description_source: standard-scope\n  flows:\n  - authorizationCode\n  resources: []\n  sources:\n  - well-known/serviceup-oauth-authorization-server.json\ncoverage:\n  scopes_total: 3\n  granularity: coarse\n\
  \  note: >-\n    Two coarse read/write scopes cover the entire MCP surface — there is no\n    per-resource or per-tool scope decomposition (no fleet:, repair:, invoice:\n    or payment: scopes are advertised), so an agent token cannot be narrowed\n    below \"read everything\" or \"write anything\" on this endpoint.\nx-evidence:\n- url: https://api.serviceup.com/.well-known/oauth-protected-resource/mcp\n  http_status: 200\n  fetched: '2026-08-05'\n- url: https://auth.serviceup.com/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serviceup/refs/heads/main/scopes/serviceup-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Fleet Management
- Vehicle Repair
- Automotive
- Insurance
- Maintenance
- Agentic AI
- MCP
- Transportation
token_urls:
- https://auth.serviceup.com/api/auth/oauth2/token
---
