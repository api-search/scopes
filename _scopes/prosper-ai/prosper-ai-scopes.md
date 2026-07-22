---
api_specs:
- filename: prosper-ai-voice-openapi.json
  format: json
  label: Prosper Voice API
  slug: prosper-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/openapi/prosper-ai-voice-openapi.json
authorization_urls:
- https://voice.getprosperapp.com/mcp/authorize
description: ''
docs: https://voice.getprosperapp.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Prosper Ai Scopes
name_suffix: OAuth Scopes
note: OAuth scopes here belong to the hosted MCP OAuth server (issuer https://voice.getprosperapp.com/mcp). The REST API uses API-key auth and declares no OAuth scopes in its OpenAPI.
overview: 'Prosper AI publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Prosper AI API on a user''s behalf.


  Tokens are issued from https://voice.getprosperapp.com/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prosper AI
provider_slug: prosper-ai
schemes:
- flows:
  - authorizationUrl: https://voice.getprosperapp.com/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://voice.getprosperapp.com/mcp/token
  name: MCP OAuth2
  source: https://voice.getprosperapp.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- read
scopes:
- description: Read access to Prosper resources exposed through the MCP server
  flows:
  - authorizationCode
  scope: read
slug: prosper-ai-scopes
source_filename: prosper-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://voice.getprosperapp.com/.well-known/oauth-authorization-server\ndocs: https://voice.getprosperapp.com/.well-known/oauth-authorization-server\nnote: >-\n  OAuth scopes here belong to the hosted MCP OAuth server (issuer\n  https://voice.getprosperapp.com/mcp). The REST API uses API-key auth and\n  declares no OAuth scopes in its OpenAPI.\nschemes:\n- name: MCP OAuth2\n  source: https://voice.getprosperapp.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://voice.getprosperapp.com/mcp/authorize\n    tokenUrl: https://voice.getprosperapp.com/mcp/token\nscopes:\n- scope: read\n  description: Read access to Prosper resources exposed through the MCP server\n  flows: [authorizationCode]\n  sources: [https://voice.getprosperapp.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosper-ai/refs/heads/main/scopes/prosper-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Healthcare
- Voice AI
- Revenue Cycle Management
- Patient Access
- EHR Integration
- AI Agents
- MCP
token_urls:
- https://voice.getprosperapp.com/mcp/token
---
