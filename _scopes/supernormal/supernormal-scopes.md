---
api_specs:
- filename: supernormal-openapi-original.json
  format: json
  label: Supernormal API
  slug: supernormal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/openapi/supernormal-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.supernormal.com/api-reference/introduction
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Supernormal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'supernormal publishes 11 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the supernormal API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: supernormal
provider_slug: supernormal
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-TOKEN
  source: openapi/supernormal-openapi-original.json
  type: apiKey
- authorizationUrl: https://api.supernormal.com/oauth/authorize
  flow: authorizationCode
  name: OAuth2
  source: well-known/supernormal-oauth-authorization-server.json
  tokenUrl: https://api.supernormal.com/oauth/token
  type: oauth2
scope_count: 11
scope_names:
- user:read
- calendar_events:read
- calendar_events:write
- posts:read
- agents:read
- agents:write
- agent_sessions:read
- agent_sessions:write
- recordings:read
- projects:read
- projects:write
scopes:
- description: Read user information.
  flows: []
  scope: user:read
- description: Read calendar events.
  flows: []
  scope: calendar_events:read
- description: Write calendar events (toggle whether a meeting is captured).
  flows: []
  scope: calendar_events:write
- description: Read the current user's meeting posts, notes, and transcripts.
  flows: []
  scope: posts:read
- description: Read the current user's AI agents.
  flows: []
  scope: agents:read
- description: Create, publish, and unpublish AI agents.
  flows: []
  scope: agents:write
- description: Read an agent's sessions.
  flows: []
  scope: agent_sessions:read
- description: Create an agent session.
  flows: []
  scope: agent_sessions:write
- description: Read meeting recordings (OAuth / MCP surface).
  flows: []
  scope: recordings:read
- description: Read projects (OAuth / MCP surface).
  flows: []
  scope: projects:read
- description: Write projects (OAuth / MCP surface).
  flows: []
  scope: projects:write
slug: supernormal-scopes
source_filename: supernormal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/supernormal-openapi-original.json\ndocs: https://docs.supernormal.com/api-reference/introduction\nnotes: >-\n  Supernormal exposes two scope surfaces. (1) API-key (X-API-TOKEN) scopes selected when\n  minting a key in account settings and enforced per-operation in the REST API — the spec\n  declares user/calendar_events scopes in the securityScheme x-scopes map and references\n  additional posts/agents/agent_sessions scopes in operation security requirements. (2) The\n  OAuth 2.0 authorization server (used for the MCP server) advertises its own scopes_supported\n  in RFC 8414 metadata. Both are captured below.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  source: openapi/supernormal-openapi-original.json\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.supernormal.com/oauth/authorize\n  tokenUrl: https://api.supernormal.com/oauth/token\n\
  \  source: well-known/supernormal-oauth-authorization-server.json\nscopes:\n# --- API-key (X-API-TOKEN) scopes ---\n- scope: user:read\n  description: Read user information.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: calendar_events:read\n  description: Read calendar events.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: calendar_events:write\n  description: Write calendar events (toggle whether a meeting is captured).\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: posts:read\n  description: Read the current user's meeting posts, notes, and transcripts.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: agents:read\n  description: Read the current user's AI agents.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: agents:write\n  description: Create, publish, and unpublish AI agents.\n  surface: api-key\n\
  \  sources: [openapi/supernormal-openapi-original.json]\n- scope: agent_sessions:read\n  description: Read an agent's sessions.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n- scope: agent_sessions:write\n  description: Create an agent session.\n  surface: api-key\n  sources: [openapi/supernormal-openapi-original.json]\n# --- OAuth 2.0 authorization-server scopes (MCP) ---\n- scope: recordings:read\n  description: Read meeting recordings (OAuth / MCP surface).\n  surface: oauth\n  sources: [well-known/supernormal-oauth-authorization-server.json]\n- scope: projects:read\n  description: Read projects (OAuth / MCP surface).\n  surface: oauth\n  sources: [well-known/supernormal-oauth-authorization-server.json]\n- scope: projects:write\n  description: Write projects (OAuth / MCP surface).\n  surface: oauth\n  sources: [well-known/supernormal-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supernormal/refs/heads/main/scopes/supernormal-scopes.yml
summary_line: 11 scopes
tags:
- Company
- Meetings
- Meeting Notes
- Transcription
- AI Agents
- Voice Agents
- Productivity
- Collaboration
- Model Context Protocol
- REST API
token_urls: []
---
