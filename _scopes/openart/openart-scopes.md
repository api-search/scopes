---
authorization_urls:
- https://openart.ai/suite/api/auth/oauth/authorize
description: ''
docs: https://openart.ai/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Openart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Openart publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Openart API on a user''s behalf.


  Tokens are issued from https://openart.ai/suite/api/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Openart
provider_slug: openart
schemes:
- flows:
  - authorizationUrl: https://openart.ai/suite/api/auth/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://openart.ai/suite/api/auth/oauth/token
  name: OAuth2
  source: well-known/openart-oauth-authorization-server.json
scope_count: 1
scope_names:
- full_access
scopes:
- description: 'Full access to the authenticated OpenArt account and its capabilities (image/video generation, model discovery, library, projects, account credits/plan). This is the only scope OpenArt''s OAuth server advertises (scopes_supported: [full_access]); it is a coarse, all-or-nothing grant.'
  flows:
  - authorizationCode
  scope: full_access
slug: openart-scopes
source_filename: openart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openart.ai/.well-known/oauth-authorization-server\ndocs: https://openart.ai/mcp\nschemes:\n- name: OAuth2\n  source: well-known/openart-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://openart.ai/suite/api/auth/oauth/authorize\n    tokenUrl: https://openart.ai/suite/api/auth/oauth/token\nscopes:\n- scope: full_access\n  description: >-\n    Full access to the authenticated OpenArt account and its capabilities\n    (image/video generation, model discovery, library, projects, account\n    credits/plan). This is the only scope OpenArt's OAuth server advertises\n    (scopes_supported: [full_access]); it is a coarse, all-or-nothing grant.\n  flows: [authorizationCode]\n  sources: [well-known/openart-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openart/refs/heads/main/scopes/openart-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Creative Tools
- MCP
- Model Context Protocol
token_urls:
- https://openart.ai/suite/api/auth/oauth/token
---
