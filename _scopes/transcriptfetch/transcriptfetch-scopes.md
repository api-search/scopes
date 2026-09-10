---
api_specs:
- filename: transcriptfetch-api-v2-openapi.json
  format: json
  label: TranscriptFetch REST API
  slug: transcriptfetch-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/openapi/transcriptfetch-api-v2-openapi.json
authorization_urls: []
description: ''
docs: https://transcriptfetch.com/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Transcriptfetch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TranscriptFetch uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TranscriptFetch
provider_slug: transcriptfetch
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: transcriptfetch-scopes
source_filename: transcriptfetch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: >-\n  https://transcriptfetch.com/.well-known/oauth-protected-resource and\n  https://clerk.transcriptfetch.com/.well-known/oauth-authorization-server (both HTTP\n  200, fetched 2026-09-09). The REST OpenAPI declares only bearerAuth (API key), so\n  derive-oauth-scopes.py found no oauth2 scheme; these scopes come from the served\n  OAuth metadata, which governs the MCP surface.\ndocs: https://transcriptfetch.com/docs/mcp\nsurface: MCP server (https://transcriptfetch.com/mcp) via Clerk-run OAuth; REST API uses bearer API keys without scopes.\nscopes:\n- name: openid\n  description: OpenID Connect authentication (standard OIDC scope).\n- name: profile\n  description: Access to basic profile claims (name, picture, preferred_username).\n- name: email\n  description: Access to the account email address and verification status.\n- name: offline_access\n  description: Refresh-token issuance for long-lived MCP client connections.\n-\
  \ name: public_metadata\n  description: Clerk user public metadata (authorization-server metadata; not documented per-endpoint by TranscriptFetch).\n- name: private_metadata\n  description: Clerk user private metadata (authorization-server metadata; not documented per-endpoint by TranscriptFetch).\nnotes:\n- The protected-resource document scopes_supported lists openid, profile, email, offline_access for the MCP resource.\n- Identity scopes only — API authorization is account/credit-based, not scope-partitioned; there are no per-tool or per-endpoint scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcriptfetch/refs/heads/main/scopes/transcriptfetch-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- transcripts
- speech-to-text
- captions
- youtube
- tiktok
- instagram
- podcasts
- mcp
- llms-txt
- openapi
- Transcription
- Speech-to-Text
- Video
- Podcasts
- AI/LLM
- RAG
- Agents
- MCP
- Developer Tools
- Media
- Content
- YouTube
- TikTok
- Instagram
- Spotify
- Apple Podcasts
token_urls: []
---
