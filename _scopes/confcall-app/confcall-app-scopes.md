---
api_specs:
- filename: confcall-app-artifacts-api-openapi.yml
  format: yaml
  label: confcall Artifacts API
  slug: confcall-app-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-artifacts-api-openapi.yml
- filename: confcall-app-embed-api-openapi.yml
  format: yaml
  label: confcall Embed API
  slug: confcall-app-embed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-embed-api-openapi.yml
- filename: confcall-app-recordings-api-openapi.yml
  format: yaml
  label: confcall Recordings API
  slug: confcall-app-recordings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-recordings-api-openapi.yml
- filename: confcall-app-rooms-api-openapi.yml
  format: yaml
  label: confcall Rooms API
  slug: confcall-app-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/confcall-app/openapi/confcall-app-rooms-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.confcall.app/api-reference.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: confcall Scopes
name_suffix: OAuth Scopes
note: confcall:* scopes are declared in the OpenAPI and tagged per route on the API reference; use:*/read:* scopes are documented only for the <agent-widget> JWT (agent.confcall.app), not in the control-plane contract.
overview: 'confcall publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the confcall API on a user''s behalf.


  Tokens are issued from https://auth.confcall.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: confcall
provider_slug: confcall-app
schemes:
- description: 'OAuth 2.0 client-credentials grant. Exchange a client id/secret at the token URL for a short-lived bearer JWT and send it as `Authorization: Bearer <token>`. Operations with x-auth jwtOrApiKey accept either this or ApiKeyAuth; x-auth jwt operations need a user-context token.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.confcall.app/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/confcall-app-openapi.yml
scope_count: 5
scope_names:
- confcall:history
- confcall:rooms
- use:chat-agent
- use:voice-agent
- read:ivr-config
scopes:
- description: Read meeting artifacts (transcripts, summaries, action items)
  flows:
  - clientCredentials
  scope: confcall:history
- description: Manage rooms and invite/remove the AI agent
  flows:
  - clientCredentials
  scope: confcall:rooms
- description: Chat sessions (agent-widget JWT)
  flows: []
  scope: use:chat-agent
- description: Voice calls (agent-widget JWT)
  flows: []
  scope: use:voice-agent
- description: IVR config access (agent-widget JWT)
  flows: []
  scope: read:ivr-config
slug: confcall-app-scopes
source_filename: confcall-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.confcall.app/api-reference.html\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/confcall-app-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.confcall.app/oauth/token\n  description: 'OAuth 2.0 client-credentials grant. Exchange a client id/secret at\n    the token URL for a short-lived bearer JWT and send it as `Authorization: Bearer\n    <token>`. Operations with x-auth jwtOrApiKey accept either this or ApiKeyAuth;\n    x-auth jwt operations need a user-context token.'\nscopes:\n- scope: confcall:history\n  description: Read meeting artifacts (transcripts, summaries, action items)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/confcall-app-openapi.yml\n  - https://docs.confcall.app/api-reference.html\n  operations:\n  - listRoomArtifacts\n  - getArtifact\n- scope: confcall:rooms\n  description: Manage rooms and invite/remove the AI agent\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/confcall-app-openapi.yml\n  - https://docs.confcall.app/api-reference.html\n  operations:\n  - deleteRoom\n  - inviteAiAgent\n  - removeAiAgent\n- scope: use:chat-agent\n  description: Chat sessions (agent-widget JWT)\n  flows: []\n  token: short-lived JWT passed to <agent-widget> auth-token\n  sources:\n  - https://docs.confcall.app/agent-widget.html\n- scope: use:voice-agent\n  description: Voice calls (agent-widget JWT)\n  flows: []\n  token: short-lived JWT passed to <agent-widget> auth-token\n  sources:\n  - https://docs.confcall.app/agent-widget.html\n- scope: read:ivr-config\n  description: IVR config access (agent-widget JWT)\n  flows: []\n  token: short-lived JWT passed to <agent-widget> auth-token\n  sources:\n  - https://docs.confcall.app/agent-widget.html\ndocs: https://docs.confcall.app/api-reference.html\nnote: confcall:* scopes are declared in the OpenAPI and tagged per route on the API\n  reference; use:*/read:* scopes are documented only for the\
  \ <agent-widget> JWT (agent.confcall.app),\n  not in the control-plane contract.\n"
source_yaml_url: https://artifacts.apis.io/confcall-app/scopes/confcall-app-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Company
- Video Conferencing
- AI Agents
- Embeddable Widgets
- Telephony
- Transcription
- MCP
- Communications
token_bound: false
token_urls:
- https://auth.confcall.app/oauth/token
---
