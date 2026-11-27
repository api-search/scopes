---
api_specs:
- filename: kaptionai-com-mcp-api-openapi.yml
  format: yaml
  label: Kaption AI MCP API
  slug: kaptionai-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaptionai-com/openapi/kaptionai-com-mcp-api-openapi.yml
authorization_urls:
- https://mcp.kaptionai.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Kaption AI Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kaption AI publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kaption AI API on a user''s behalf.


  Tokens are issued from https://mcp.kaptionai.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kaption AI
provider_slug: kaptionai-com
schemes:
- description: OAuth 2.1 authorization code flow with PKCE (S256) and dynamic client registration at https://mcp.kaptionai.com/register. The user signs in with their phone number and a code sent to them on WhatsApp. Access tokens expire after one hour.
  flows:
  - authorizationUrl: https://mcp.kaptionai.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.kaptionai.com/token
  name: kaptionOAuth
  source: openapi/kaptionai-com-openapi.json
scope_count: 1
scope_names:
- kaption:access
scopes:
- description: Use the Kaption MCP tools on the signed-in user's WhatsApp through Kaption.
  flows:
  - authorizationCode
  scope: kaption:access
slug: kaptionai-com-scopes
source_filename: kaptionai-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kaptionai-com-openapi.json\nschemes:\n- name: kaptionOAuth\n  source: openapi/kaptionai-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.kaptionai.com/authorize\n    tokenUrl: https://mcp.kaptionai.com/token\n  description: OAuth 2.1 authorization code flow with PKCE (S256) and dynamic client registration\n    at https://mcp.kaptionai.com/register. The user signs in with their phone number and a code\n    sent to them on WhatsApp. Access tokens expire after one hour.\nscopes:\n- scope: kaption:access\n  description: Use the Kaption MCP tools on the signed-in user's WhatsApp through Kaption.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/kaptionai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kaptionai-com/scopes/kaptionai-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI Assistant
- Transcription
- Call Recording
- Translation
- Scheduling
- Backups
token_bound: false
token_urls:
- https://mcp.kaptionai.com/token
---
