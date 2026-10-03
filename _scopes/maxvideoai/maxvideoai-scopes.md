---
authorization_urls:
- https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/authorize
description: ''
docs: https://maxvideoai.com/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Maxvideoai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MaxVideoAI publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MaxVideoAI API on a user''s behalf.


  Tokens are issued from https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MaxVideoAI
provider_slug: maxvideoai
schemes:
- flows:
  - authorizationUrl: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token
  name: OAuth2
  source: well-known/maxvideoai-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- profile
- offline_access
scopes:
- description: OpenID Connect authentication of the connecting user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email for account identification.
  flows:
  - authorizationCode
  scope: email
- description: Access to the user's basic profile.
  flows:
  - authorizationCode
  scope: profile
- description: Refresh-token issuance for long-lived connections.
  flows:
  - authorizationCode
  scope: offline_access
slug: maxvideoai-scopes
source_filename: maxvideoai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: searched\nsource: https://api.maxvideoai.com/.well-known/oauth-authorization-server\ndocs: https://maxvideoai.com/docs/mcp\nschemes:\n- name: OAuth2\n  source: well-known/maxvideoai-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the connecting user.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email for account identification.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Refresh-token issuance for long-lived connections.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes are coarse identity/consent scopes only; per-tool authorization\n\
  \  (planning vs paid generation) is enforced server-side behind the single OAuth\n  grant, not via distinct OAuth scopes. The MCP client requests openid,email,profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maxvideoai/refs/heads/main/scopes/maxvideoai-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Artificial Intelligence
- Video Generation
- Image Generation
- MCP
- Agent-Native
- Text-to-Video
- Image-to-Video
- Creative Production
- Pay As You Go
token_urls:
- https://vujvontfztdzszylnsyc.supabase.co/auth/v1/oauth/token
---
