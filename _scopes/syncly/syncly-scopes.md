---
api_specs:
- filename: syncly-health-api-openapi.yml
  format: yaml
  label: Syncly Health API
  slug: syncly-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/openapi/syncly-health-api-openapi.yml
- filename: syncly-well-known-api-openapi.yml
  format: yaml
  label: Syncly .well Known API
  slug: syncly-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/openapi/syncly-well-known-api-openapi.yml
authorization_urls:
- https://social-server.syncly.app/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Syncly Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Syncly publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Syncly API on a user''s behalf.


  Tokens are issued from https://social-server.syncly.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Syncly
provider_slug: syncly
schemes:
- flows:
  - authorizationUrl: https://social-server.syncly.app/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://social-server.syncly.app/oauth/token
  name: SynclySocialOAuth
  source: https://social-server.syncly.app/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- syncly:read
- offline_access
scopes:
- description: Read access to the connected Syncly workspace. This is the only resource scope Syncly declares, and it is the scope the MCP server names in its 401 challenge. Description is API Evangelist's reading of the scope name, not provider-published text.
  flows:
  - authorizationCode
  scope: syncly:read
- description: Standard OpenID Connect / OAuth 2.0 scope requesting a refresh token so the client can renew access without a fresh user consent. Declared by the authorization server but not listed in the protected-resource metadata.
  flows:
  - authorizationCode
  scope: offline_access
slug: syncly-scopes
source_filename: syncly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://social-server.syncly.app/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  Syncly publishes no scopes/permissions reference page. The scope set below is read from the\n  provider's own RFC 8414 authorization-server metadata and the RFC 9728 protected-resource\n  metadata, which are the authoritative machine-readable declarations. Descriptions are ours,\n  derived from the scope names and the OAuth specs they come from, and are marked as such.\nschemes:\n- name: SynclySocialOAuth\n  source: https://social-server.syncly.app/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://social-server.syncly.app/oauth/authorize\n    tokenUrl: https://social-server.syncly.app/oauth/token\nscopes:\n- scope: syncly:read\n  description: >-\n    Read access to the connected Syncly workspace. This is the only resource scope Syncly\n    declares, and it is the scope\
  \ the MCP server names in its 401 challenge. Description is\n    API Evangelist's reading of the scope name, not provider-published text.\n  description_source: derived\n  flows: [authorizationCode]\n  sources:\n  - https://social-server.syncly.app/.well-known/oauth-authorization-server\n  - https://mcp.syncly.app/.well-known/oauth-protected-resource\n- scope: offline_access\n  description: >-\n    Standard OpenID Connect / OAuth 2.0 scope requesting a refresh token so the client can\n    renew access without a fresh user consent. Declared by the authorization server but not\n    listed in the protected-resource metadata.\n  description_source: rfc6749-oidc-core\n  flows: [authorizationCode]\n  sources:\n  - https://social-server.syncly.app/.well-known/oauth-authorization-server\nsummary:\n  scope_count: 2\n  resource_scope_count: 1\n  write_scopes: 0\n  note: >-\n    Syncly's OAuth surface is read-only. There is no declared write, admin, or per-resource\n    scope, which matches an MCP\
  \ server whose published capabilities are all analytical reads.\nx-evidence:\n- url: https://social-server.syncly.app/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-13'\n- url: https://mcp.syncly.app/.well-known/oauth-protected-resource\n  http_status: 200\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/scopes/syncly-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Social Intelligence
- Social Listening
- Customer Feedback
- Voice of Customer
- Creator Marketing
- Analytics
- Artificial Intelligence
- MCP
token_urls:
- https://social-server.syncly.app/oauth/token
---
