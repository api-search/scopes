---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Kuaishou Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kuaishou uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kuaishou
provider_slug: kuaishou
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: kuaishou-scopes
source_filename: kuaishou-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://kling.ai/.well-known/oauth-protected-resource (HTTP 200, application/json) and\n  https://kling.ai/.well-known/oauth-authorization-server/auth (HTTP 200, application/json), both\n  fetched 2026-08-12\nnotes: >-\n  These scopes are not derived from any spec and not guessed — they are read verbatim from the\n  scopes_supported array of Kuaishou's own machine-readable OAuth metadata for the Kling AI MCP server.\n  The descriptions below are the pipeline's plain-language reading of each scope name; the provider\n  publishes the identifiers only, with no scope reference page found. The Kuaishou Open Platform\n  (open.kuaishou.com) and Kwai for Business (developers.kwai.com) publish NO scope reference on any\n  public surface, so no scopes are asserted for them.\napis:\n- api: kuaishou:kling-ai\n  authorization_server: https://kling.ai/auth\n  resource: https://kling.ai/mcp\n  flow: authorization_code\n  pkce: S256\n\
  \  dynamic_client_registration: https://kling.ai/auth/register\n  scope_count: 3\n  scopes:\n  - name: generation.create\n    description: >-\n      Submit generation tasks (text-to-image, image-to-image, text-to-video, image-to-video) and upload\n      the source files they consume. This is the write/spend scope — generation consumes account credits.\n    verified: true\n    source: scopes_supported\n  - name: generation.read\n    description: >-\n      Read the status and result URLs of previously submitted generation tasks (the query_tasks tool).\n    verified: true\n    source: scopes_supported\n  - name: account.credit.read\n    description: >-\n      Read membership tier and remaining credit balance (the query_membership_and_credits tool).\n    verified: true\n    source: scopes_supported\n- api: kuaishou:open-platform\n  scope_count: 0\n  scopes: []\n  note: >-\n    The Open Platform runs an OAuth 2.0 authorization-code flow at /oauth2/authorize and\n    /oauth2/access_token and\
  \ a client_credentials flow for standalone mini programs, but its\n    permission/product reference sits inside the registered-developer console. No public scope list was\n    retrievable, so none is asserted.\n- api: kuaishou:kwai-for-business\n  scope_count: 0\n  scopes: []\n  note: No authorization or token endpoint could be confirmed on the public surface.\ndocs: null\ndocs_note: >-\n  No human-readable scope/permission reference page was found for the Kling AI OAuth scopes; the\n  machine-readable metadata document is the only public source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuaishou/refs/heads/main/scopes/kuaishou-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Social
- Video
- Short Video
- Live Streaming
- Advertising
- Marketing
- Social Media
- Content
- China
- AI
- Generative AI
- Machine Learning
- MCP
token_urls: []
---
