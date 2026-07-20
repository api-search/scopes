---
authorization_urls:
- https://api.laminalabs.ai/oauth/authorize
description: ''
docs: https://app.laminalabs.ai/simi
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lamina Labs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lamina Labs publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lamina Labs API on a user''s behalf.


  Tokens are issued from https://api.laminalabs.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lamina Labs
provider_slug: lamina-labs
schemes:
- flows:
  - authorizationUrl: https://api.laminalabs.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.laminalabs.ai/oauth/token
  name: LaminaOAuth
  source: well-known/lamina-labs-oauth-authorization-server.json
scope_count: 2
scope_names:
- jobs:create
- jobs:read
scopes:
- description: Submit Simi video generation jobs.
  flows:
  - authorizationCode
  scope: jobs:create
- description: Read Simi video job status and retrieve playback/download URLs.
  flows:
  - authorizationCode
  scope: jobs:read
slug: lamina-labs-scopes
source_filename: lamina-labs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.laminalabs.ai/.well-known/oauth-authorization-server\ndocs: https://app.laminalabs.ai/simi\nschemes:\n- name: LaminaOAuth\n  source: well-known/lamina-labs-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.laminalabs.ai/oauth/authorize\n    tokenUrl: https://api.laminalabs.ai/oauth/token\nscopes:\n- scope: jobs:create\n  description: Submit Simi video generation jobs.\n  flows: [authorizationCode]\n  sources: [well-known/lamina-labs-oauth-authorization-server.json]\n  mcp_tools: [simi_submit_video]\n  action_class: write\n- scope: jobs:read\n  description: Read Simi video job status and retrieve playback/download URLs.\n  flows: [authorizationCode]\n  sources: [well-known/lamina-labs-oauth-authorization-server.json]\n  mcp_tools: [simi_get_video]\n  action_class: read\nnotes:\n- The scope surface is small and cleanly split read/write, which maps one-to-one\
  \ onto\n  the two published MCP tools.\n- Scopes are advertised in `scopes_supported` on both discovery documents; no separate\n  scopes reference page is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lamina-labs/refs/heads/main/scopes/lamina-labs-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Video
- Video Generation
- Machine Learning
- Education
- Media
- Model Context Protocol
- Content Generation
token_urls:
- https://api.laminalabs.ai/oauth/token
---
