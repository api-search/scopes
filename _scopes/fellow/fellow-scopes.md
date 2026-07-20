---
api_specs:
- filename: fellow-webhooks-asyncapi.yml
  format: yaml
  label: Fellow Developer API
  slug: fellow-developer-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/asyncapi/fellow-webhooks-asyncapi.yml
authorization_urls:
- https://fellow.app/mcp/authorize
description: ''
docs: https://developers.fellow.ai/reference/mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Fellow Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fellow publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fellow API on a user''s behalf.


  Tokens are issued from https://fellow.app/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fellow
provider_slug: fellow
schemes:
- flows:
  - authorizationUrl: https://fellow.app/mcp/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://fellow.app/mcp/token
  name: MCPOAuth
  source: well-known/fellow-oauth-authorization-server.json
scope_count: 5
scope_names:
- read_calendar
- read_meeting_content
- read_action_items
- read_channels
- write_meeting_agenda
scopes:
- description: Read the user's calendar events.
  flows:
  - authorizationCode
  scope: read_calendar
- description: Read meeting content — AI notes, summaries, and transcripts.
  flows:
  - authorizationCode
  scope: read_meeting_content
- description: Read action items the user can access.
  flows:
  - authorizationCode
  scope: read_action_items
- description: Read channels the user belongs to.
  flows:
  - authorizationCode
  scope: read_channels
- description: Write/update meeting agenda content.
  flows:
  - authorizationCode
  scope: write_meeting_agenda
slug: fellow-scopes
source_filename: fellow-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://fellow.app/.well-known/oauth-authorization-server\ndocs: https://developers.fellow.ai/reference/mcp-server\ncontext: >-\n  Fellow's OAuth scopes apply to the hosted MCP server (https://fellow.app/mcp), not\n  the REST Developer API (which uses X-API-KEY). Scopes are advertised in the RFC\n  8414 OAuth 2.0 Authorization Server Metadata document.\nschemes:\n- name: MCPOAuth\n  source: well-known/fellow-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fellow.app/mcp/authorize\n    tokenUrl: https://fellow.app/mcp/token\n    pkce: S256\nscopes:\n- scope: read_calendar\n  description: Read the user's calendar events.\n  flows: [authorizationCode]\n- scope: read_meeting_content\n  description: Read meeting content — AI notes, summaries, and transcripts.\n  flows: [authorizationCode]\n- scope: read_action_items\n  description: Read action items the user can access.\n  flows:\
  \ [authorizationCode]\n- scope: read_channels\n  description: Read channels the user belongs to.\n  flows: [authorizationCode]\n- scope: write_meeting_agenda\n  description: Write/update meeting agenda content.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fellow/refs/heads/main/scopes/fellow-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Saas
- Meetings
- AI
- Meeting Notes
- Transcription
- Productivity
- Action Items
- Webhooks
- MCP
token_urls:
- https://fellow.app/mcp/token
---
