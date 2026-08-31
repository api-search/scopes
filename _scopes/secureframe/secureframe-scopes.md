---
api_specs:
- filename: secureframe-public-api-openapi.yml
  format: yaml
  label: Secureframe Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/secureframe/refs/heads/main/openapi/secureframe-public-api-openapi.yml
authorization_urls: []
description: 'Secureframe publishes OAuth scopes on ONE surface only: the hosted MCP server. The REST API at api.secureframe.com uses an API key/secret pair with no OAuth flow and no scopes at all — authorization there comes entirely from the RBAC role of the user the key belongs to.'
docs: https://mcp.secureframe.com/mcp_docs
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Secureframe Scopes
name_suffix: OAuth Scopes
note: A single scope named "mcp" grants the whole surface. There is no read-only scope, no per-resource scope and no way to grant an agent a subset — even though the provider labels 63 of its 112 tools read and 49 write. Effective permissions are whatever the authorizing user's RBAC role allows, which the agent cannot enumerate through the API.
overview: 'Secureframe uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Secureframe
provider_slug: secureframe
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: secureframe-scopes
source_filename: secureframe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Secureframe\nproviderId: secureframe\ngenerated: '2026-08-27'\nmodified: '2026-08-27'\nmethod: probed\nsource: https://mcp.secureframe.com/.well-known/oauth-authorization-server (200, 2026-08-27) + https://mcp.secureframe.com/mcp_docs\ndocs: https://mcp.secureframe.com/mcp_docs\ndescription: 'Secureframe publishes OAuth scopes on ONE surface only: the hosted MCP server. The REST API at\n  api.secureframe.com uses an API key/secret pair with no OAuth flow and no scopes at all — authorization there\n  comes entirely from the RBAC role of the user the key belongs to.'\nsurfaces:\n- surface: MCP server\n  endpoint: https://mcp.secureframe.com/\n  flow: OAuth 2.1 authorization_code + PKCE (S256), refresh_token\n  authorization_server: https://mcp.secureframe.com\n  dynamic_client_registration: true\n  scopes_supported:\n  - mcp\n- surface: REST API\n  endpoint: https://api.secureframe.com\n  flow: none\
  \ — apiKey in the Authorization header\n  scopes_supported: []\n  note: 'components.securitySchemes declares exactly one scheme, header_authorization (apiKey, in: header).\n    No oauth2 or openIdConnect scheme exists.'\nscopes:\n- name: mcp\n  description: Permission for an MCP client to use the Secureframe API as the authorizing user, inside one\n    selected company.\n  surface: MCP\n  granted_by: the consent screen during the browser sign-in flow\n  source: scopes_supported in the RFC 8414 metadata; described at https://mcp.secureframe.com/mcp_docs\ngranularity: coarse\nnote: A single scope named \"mcp\" grants the whole surface. There is no read-only scope, no per-resource scope\n  and no way to grant an agent a subset — even though the provider labels 63 of its 112 tools read and 49 write.\n  Effective permissions are whatever the authorizing user's RBAC role allows, which the agent cannot enumerate\n  through the API.\ntoken:\n  access_token_lifetime: 1 hour\n  refresh: silent;\
  \ the refresh credential rotates on each use\n  revocation_endpoint: https://mcp.secureframe.com/oauth/revoke\n  introspection_endpoint: https://mcp.secureframe.com/oauth/introspect\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secureframe/refs/heads/main/scopes/secureframe-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- GRC
- Compliance
- SOC 2
- ISO 27001
- Risk
- CMMC
- FedRAMP
- Security
- Audit
- Trust
token_urls: []
---
