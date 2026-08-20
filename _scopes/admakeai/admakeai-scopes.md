---
authorization_urls:
- https://admakeai.com/oauth/authorize
description: ''
docs: https://github.com/mesmerlord/admakeai-mcp#permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Admakeai Scopes
name_suffix: OAuth Scopes
note: No OpenAPI exists to derive from, so this is read from the provider's live RFC 8414 authorization-server metadata and the scope descriptions the provider publishes in its own MCP server card and MCP README. Three functional scopes plus offline_access; scope is filtered at tools/list, so a narrower grant removes the tools entirely rather than failing them at call time.
overview: 'AdMakeAI publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdMakeAI API on a user''s behalf.


  Tokens are issued from https://admakeai.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdMakeAI
provider_slug: admakeai
schemes:
- flows:
  - authorizationUrl: https://admakeai.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://admakeai.com/api/oauth/token
  issuer: https://admakeai.com
  name: oauth2
  source: https://admakeai.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- mcp:read
- mcp:write
- mcp:publish
- offline_access
scopes:
- description: Read the account, projects, generated ads, competitor research results, and Facebook/Meta ad performance.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Generate ads, upload images, write ad copy, and prepare campaign drafts. Spends plan credits.
  flows:
  - authorizationCode
  scope: mcp:write
- description: Push drafts live and pause or resume running Facebook campaigns, ad sets, and ads.
  flows:
  - authorizationCode
  scope: mcp:publish
- description: Issue a rotating refresh token.
  flows:
  - authorizationCode
  scope: offline_access
slug: admakeai-scopes
source_filename: admakeai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://admakeai.com/.well-known/oauth-authorization-server (probed 2026-08-11, HTTP 200)\ndocs: https://github.com/mesmerlord/admakeai-mcp#permissions\nnote: >-\n  No OpenAPI exists to derive from, so this is read from the provider's live RFC 8414 authorization-server metadata and\n  the scope descriptions the provider publishes in its own MCP server card and MCP README. Three functional scopes plus\n  offline_access; scope is filtered at tools/list, so a narrower grant removes the tools entirely rather than failing\n  them at call time.\nschemes:\n  - name: oauth2\n    issuer: https://admakeai.com\n    source: https://admakeai.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://admakeai.com/oauth/authorize\n        tokenUrl: https://admakeai.com/api/oauth/token\n        code_challenge_methods: [S256]\nscopes:\n  - scope: mcp:read\n    consent_label: Read\
  \ your account\n    description: >-\n      Read the account, projects, generated ads, competitor research results, and Facebook/Meta ad performance.\n    covers: [projects, generations, research results, analytics]\n    flows: [authorizationCode]\n    tools: 40\n  - scope: mcp:write\n    consent_label: Create ads and drafts\n    description: >-\n      Generate ads, upload images, write ad copy, and prepare campaign drafts. Spends plan credits.\n    covers: [image generation, video generation, ad copy, ad sets, campaign drafts]\n    flows: [authorizationCode]\n    tools: 16\n  - scope: mcp:publish\n    consent_label: Manage live Facebook ads\n    description: >-\n      Push drafts live and pause or resume running Facebook campaigns, ad sets, and ads.\n    covers: [live Meta status changes, publishing drafts]\n    flows: [authorizationCode]\n    tools: 9\n    note: Six of the nine pause/resume tools in this class are currently disabled and fail closed.\n  - scope: offline_access\n    description:\
  \ Issue a rotating refresh token.\n    flows: [authorizationCode]\nenforcement:\n  point: tools/list\n  detail: A connection approved without mcp:publish cannot even list the live-action tools.\n  revocation: https://admakeai.com/api/oauth/revoke\n  source: https://admakeai.com/.well-known/mcp.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admakeai/refs/heads/main/scopes/admakeai-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Advertising
- Marketing
- AdTech
- Generative AI
- Image-Generation
- Video Generation
- Meta Ads
- Competitive Intelligence
- MCP
- Agents
- Agent Skills
token_urls:
- https://admakeai.com/api/oauth/token
---
