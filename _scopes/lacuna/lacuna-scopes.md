---
api_specs:
- filename: lacuna-lacuna-music-api-api-openapi.yml
  format: yaml
  label: Lacuna Lacuna Music API API
  slug: lacuna-lacuna-music-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-lacuna-music-api-api-openapi.yml
- filename: lacuna-music-api-openapi.yml
  format: yaml
  label: Lacuna Music API
  slug: lacuna-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/openapi/lacuna-music-api-openapi.yml
authorization_urls:
- https://www.lacuna.fm/oauth/authorize
description: ''
docs: https://www.lacuna.fm/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lacuna Scopes
name_suffix: OAuth Scopes
note: The published OpenAPI declares only `bearerAuth` (http bearer), so no scopes are derivable from the spec. The OAuth scope surface is published instead in the RFC 8414 authorization-server metadata, the RFC 9728 protected-resource metadata, the A2A agent card, and the MCP server card — all four agree.
overview: 'Lacuna publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lacuna API on a user''s behalf.


  Tokens are issued from https://www.lacuna.fm/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lacuna
provider_slug: lacuna
schemes:
- flows:
  - authorizationUrl: https://www.lacuna.fm/oauth/authorize
    code_challenge_methods_supported:
    - S256
    flow: authorizationCode
    tokenUrl: https://www.lacuna.fm/oauth/token
  name: oauth2
  source: well-known/lacuna-oauth-authorization-server.json
scope_count: 5
scope_names:
- profile
- music:generate
- livecoding:agent
- music:agent
- lyrics:agent
scopes:
- description: Grants the profile scope — account identity.
  flows:
  - authorizationCode
  scope: profile
- description: Grants music generation. Required for music generation over REST, MCP and A2A alike (scopes_required in both the agent-auth block and the MCP server card).
  flows:
  - authorizationCode
  scope: music:generate
- description: Grants the livecoding:agent scope.
  flows:
  - authorizationCode
  scope: livecoding:agent
- description: Grants the music:agent scope.
  flows:
  - authorizationCode
  scope: music:agent
- description: Grants the lyrics:agent scope.
  flows:
  - authorizationCode
  scope: lyrics:agent
slug: lacuna-scopes
source_filename: lacuna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://www.lacuna.fm/.well-known/oauth-authorization-server\ndocs: https://www.lacuna.fm/auth.md\nnote: >-\n  The published OpenAPI declares only `bearerAuth` (http bearer), so no scopes are derivable from the\n  spec. The OAuth scope surface is published instead in the RFC 8414 authorization-server metadata, the\n  RFC 9728 protected-resource metadata, the A2A agent card, and the MCP server card — all four agree.\nschemes:\n  - name: oauth2\n    source: well-known/lacuna-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.lacuna.fm/oauth/authorize\n        tokenUrl: https://www.lacuna.fm/oauth/token\n        code_challenge_methods_supported:\n          - S256\nscopes:\n  - scope: profile\n    description: Grants the profile scope — account identity.\n    flows: [authorizationCode]\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n    \
  \  - a2a/lacuna-agent-card.json\n  - scope: music:generate\n    description: >-\n      Grants music generation. Required for music generation over REST, MCP and A2A alike\n      (scopes_required in both the agent-auth block and the MCP server card).\n    required: true\n    flows: [authorizationCode]\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n      - well-known/lacuna-oauth-protected-resource.json\n      - mcp/lacuna-mcp-server-card.json\n      - a2a/lacuna-agent-card.json\n  - scope: livecoding:agent\n    description: Grants the livecoding:agent scope.\n    flows: [authorizationCode]\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n      - a2a/lacuna-agent-card.json\n  - scope: music:agent\n    description: Grants the music:agent scope.\n    flows: [authorizationCode]\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n      - a2a/lacuna-agent-card.json\n  - scope: lyrics:agent\n    description: Grants the lyrics:agent\
  \ scope.\n    flows: [authorizationCode]\n    sources:\n      - well-known/lacuna-oauth-authorization-server.json\n      - a2a/lacuna-agent-card.json\ngaps:\n  - >-\n    Lacuna publishes scope names but not a scopes/permissions reference page describing what each\n    agent scope (livecoding:agent, music:agent, lyrics:agent) actually authorizes. The metadata\n    descriptions are self-referential (\"Grants the X scope\").\nx-evidence:\n  fetched: '2026-08-09'\n  urls:\n    - url: https://www.lacuna.fm/.well-known/oauth-authorization-server\n      http_status: 200\n    - url: https://www.lacuna.fm/.well-known/oauth-protected-resource\n      http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lacuna/refs/heads/main/scopes/lacuna-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- AI Music
- Music Generation
- AI Song Generator
- AI Lyrics Generator
- Audio
- MIDI
- Songwriting
- Generative AI
- MCP Server
- AgentSkill
- A2A
- Developer Tools
token_urls:
- https://www.lacuna.fm/oauth/token
---
