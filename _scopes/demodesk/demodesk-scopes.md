---
api_specs:
- filename: demodesk-v2-openapi.yml
  format: yaml
  label: Demodesk Public API (v2)
  slug: demodesk-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v2-openapi.yml
- filename: demodesk-v1-openapi.json
  format: json
  label: Demodesk API V1 (deprecated)
  slug: demodesk-api-v1-deprecated
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/openapi/demodesk-v1-openapi.json
authorization_urls:
- https://demodesk.com/oauth/authorize
description: ''
docs: https://demodesk.com/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Demodesk Scopes
name_suffix: OAuth Scopes
note: Demodesk's REST API authenticates with a Bearer API key and declares no OAuth2 scopes in its OpenAPI. OAuth2 is used by the hosted MCP server (https://demodesk.com/mcp); its authorization-server metadata publishes a single scope. Captured from the live well-known document, not the OpenAPI.
overview: 'Demodesk publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Demodesk API on a user''s behalf.


  Tokens are issued from https://demodesk.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demodesk
provider_slug: demodesk
schemes:
- flows:
  - authorizationUrl: https://demodesk.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://demodesk.com/oauth/introspect
    pkce: S256
    registrationUrl: https://demodesk.com/oauth/register
    revocationUrl: https://demodesk.com/oauth/revoke
    tokenUrl: https://demodesk.com/oauth/token
  name: OAuth2 (MCP)
  source: https://demodesk.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Access to the Demodesk MCP server tool surface (the v2 API capabilities).
  flows:
  - authorizationCode
  scope: mcp:tools
slug: demodesk-scopes
source_filename: demodesk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://demodesk.com/.well-known/oauth-authorization-server\ndocs: https://demodesk.com/mcp\nnote: >-\n  Demodesk's REST API authenticates with a Bearer API key and declares no OAuth2\n  scopes in its OpenAPI. OAuth2 is used by the hosted MCP server\n  (https://demodesk.com/mcp); its authorization-server metadata publishes a\n  single scope. Captured from the live well-known document, not the OpenAPI.\nschemes:\n- name: OAuth2 (MCP)\n  source: https://demodesk.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://demodesk.com/oauth/authorize\n    tokenUrl: https://demodesk.com/oauth/token\n    registrationUrl: https://demodesk.com/oauth/register\n    revocationUrl: https://demodesk.com/oauth/revoke\n    introspectionUrl: https://demodesk.com/oauth/introspect\n    pkce: S256\nscopes:\n- scope: mcp:tools\n  description: Access to the Demodesk MCP server tool surface (the\
  \ v2 API capabilities).\n  flows: [authorizationCode]\n  sources: [https://demodesk.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demodesk/refs/heads/main/scopes/demodesk-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Sales
- AI
- Conversation Intelligence
- Video Conferencing
- CRM
- Transcription
- Webhooks
- MCP
token_urls:
- https://demodesk.com/oauth/token
---
