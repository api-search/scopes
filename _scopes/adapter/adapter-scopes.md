---
api_specs:
- filename: adapter-openapi.json
  format: json
  label: Adapter Cognition API
  slug: adapter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/openapi/adapter-openapi.json
authorization_urls:
- https://api.adapter.com/v1/oauth2/authorize
description: ''
docs: https://api.adapter.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Adapter Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adapter publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adapter API on a user''s behalf.


  Tokens are issued from https://api.adapter.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adapter
provider_slug: adapter
schemes:
- flows:
  - authorizationUrl: https://api.adapter.com/v1/oauth2/authorize
    client_id_metadata_document_supported: true
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.adapter.com/v1/oauth2/token
    token_endpoint_auth_methods:
    - none
  name: OAuth2
  source: https://api.adapter.com/.well-known/oauth-authorization-server
scope_count: 2
scope_names:
- mcp:read
- offline_access
scopes:
- description: Read access to the Adapter hosted MCP server (agent/tool access to cognition queries).
  flows:
  - authorizationCode
  scope: mcp:read
- description: Issue a refresh token so an agent can maintain long-lived access without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
slug: adapter-scopes
source_filename: adapter-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api.adapter.com/.well-known/oauth-authorization-server\ndocs: https://api.adapter.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: https://api.adapter.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.adapter.com/v1/oauth2/authorize\n    tokenUrl: https://api.adapter.com/v1/oauth2/token\n    pkce: S256\n    token_endpoint_auth_methods: [none]\n    client_id_metadata_document_supported: true\nscopes:\n- scope: mcp:read\n  description: Read access to the Adapter hosted MCP server (agent/tool access to cognition queries).\n  flows: [authorizationCode]\n  sources: [https://api.adapter.com/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Issue a refresh token so an agent can maintain long-lived access without re-consent.\n  flows: [authorizationCode]\n  sources: [https://api.adapter.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapter/refs/heads/main/scopes/adapter-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Ai
- Cognition
- Knowledge Graph
- Memory
- Agents
- MCP
- LLM
token_urls:
- https://api.adapter.com/v1/oauth2/token
---
