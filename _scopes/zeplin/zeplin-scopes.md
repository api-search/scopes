---
authorization_urls:
- /v1/oauth/authorize
description: ''
docs: https://docs.zeplin.dev/reference/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Zeplin Scopes
name_suffix: OAuth Scopes
note: Zeplin's OAuth 2.0 (authorization code with PKCE) does not use or document granular scopes; the authorize endpoint accepts no scope parameter and authorized apps get broad read/write access on behalf of the user (https://docs.zeplin.dev/reference/authentication).
overview: 'Zeplin uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zeplin
provider_slug: zeplin
schemes:
- flows:
  - authorizationUrl: /v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: /v1/oauth/token
  name: OAuth2
  source: openapi/zeplin-zeplin-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: zeplin-scopes
source_filename: zeplin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zeplin-zeplin-api-openapi.yml\ndocs: https://docs.zeplin.dev/reference/authentication\nnote: Zeplin's OAuth 2.0 (authorization code with PKCE) does not use or document\n  granular scopes; the authorize endpoint accepts no scope parameter and authorized\n  apps get broad read/write access on behalf of the user\n  (https://docs.zeplin.dev/reference/authentication).\nschemes:\n- name: OAuth2\n  source: openapi/zeplin-zeplin-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/oauth/authorize\n    tokenUrl: /v1/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeplin/refs/heads/main/scopes/zeplin-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Design
- Design Handoff
- Developer Tools
- Figma
- Sketch
- Adobe XD
- Style Guides
- Components
- Assets
- Webhooks
token_urls:
- /v1/oauth/token
---
