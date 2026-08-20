---
authorization_urls:
- https://api.theorg.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Theorg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Org publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Org API on a user''s behalf.


  Tokens are issued from https://api.theorg.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Org
provider_slug: theorg
schemes:
- client_id_metadata_document_supported: true
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.theorg.com/oauth/authorize
    flow: authorizationCode
    note: Public-client authorization code + PKCE, the OAuth 2.1 profile the MCP authorization spec requires. No client secret is used.
    pkce_methods:
    - S256
    tokenUrl: https://api.theorg.com/oauth/token
    token_endpoint_auth_methods:
    - none
  issuer: https://api.theorg.com
  name: OAuth2
  registration_endpoint: https://api.theorg.com/oauth/register
  source: https://api.theorg.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to The Org's Model Context Protocol endpoint at https://api.theorg.com/v1.1/mcp and the tools it exposes. This is the only scope the authorization server advertises; The Org has not decomposed MCP access into per-tool or read/write scopes.
  flows:
  - authorizationCode
  scope: mcp
slug: theorg-scopes
source_filename: theorg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.theorg.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  The Org publishes no scopes / permissions reference page. developers.theorg.com/api/key-concepts\n  documents API-key authentication only and does not mention OAuth at all — the OAuth surface\n  below was read from the live RFC 8414 / RFC 9728 metadata documents the API host serves,\n  not from documentation.\nschemes:\n- name: OAuth2\n  source: https://api.theorg.com/.well-known/oauth-authorization-server\n  issuer: https://api.theorg.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.theorg.com/oauth/authorize\n    tokenUrl: https://api.theorg.com/oauth/token\n    pkce_methods: [S256]\n    token_endpoint_auth_methods: [none]\n    note: >-\n      Public-client authorization code + PKCE, the OAuth 2.1 profile the MCP\n      authorization spec requires. No client secret is used.\n  registration_endpoint: https://api.theorg.com/oauth/register\n\
  \  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\nscopes:\n- scope: mcp\n  description: >-\n    Access to The Org's Model Context Protocol endpoint at https://api.theorg.com/v1.1/mcp\n    and the tools it exposes. This is the only scope the authorization server advertises;\n    The Org has not decomposed MCP access into per-tool or read/write scopes.\n  flows: [authorizationCode]\n  sources:\n  - https://api.theorg.com/.well-known/oauth-authorization-server\n  - https://api.theorg.com/.well-known/oauth-protected-resource\n  - 'WWW-Authenticate challenge on POST https://api.theorg.com/v1.1/mcp (scope=mcp)'\nprotected_resources:\n- resource: https://api.theorg.com/v1.1/mcp\n  authorization_servers: [https://api.theorg.com]\n  scopes_supported: [mcp]\n  bearer_methods_supported: [header]\n  resource_documentation: https://developers.theorg.com/api\nx-evidence:\n  fetched: '2026-08-14'\n  probes:\n  - url: https://api.theorg.com/.well-known/oauth-authorization-server\n\
  \    http_status: 200\n  - url: https://api.theorg.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://api.theorg.com/v1.1/mcp\n    http_status: 401\n    www_authenticate: 'Bearer realm=\"mcp\",resource_metadata=\"https://api.theorg.com/.well-known/oauth-protected-resource/v1.1/mcp\",scope=mcp'\nnotes: >-\n  Scope coverage is deliberately coarse: a single `mcp` scope gates the whole agent\n  surface. The REST API (companies, positions, lists, usage) is not an OAuth protected\n  resource — it remains X-Api-Key only — so OAuth here authorizes agents, not the\n  general API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theorg/refs/heads/main/scopes/theorg-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Organizational Charts
- People Data
- Sales Intelligence
- Prospecting
- Org Chart
- B2B Data
- MCP
- Contact Data
- Lead Generation
- Job
- Agents
token_urls:
- https://api.theorg.com/oauth/token
---
