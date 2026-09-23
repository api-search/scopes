---
api_specs:
- filename: openhandle-openapi.yml
  format: yaml
  label: Openhandle API
  slug: openhandle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/openapi/openhandle-openapi.yml
authorization_urls:
- https://api.openhandle.dev/oauth/authorize
description: ''
docs: https://openhandle.dev/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Openhandle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Openhandle publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Openhandle API on a user''s behalf.


  Tokens are issued from https://api.openhandle.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Openhandle
provider_slug: openhandle
schemes:
- description: OAuth grants for the MCP endpoint only. REST operations require OpenhandleKey.
  flows:
  - authorizationUrl: https://api.openhandle.dev/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.openhandle.dev/oauth/token
  name: OpenhandleMCPOAuth
  source: openapi/openhandle-openapi.yml
scope_count: 4
scope_names:
- mcp
- read:instagram
- read:tiktok
- read:twitter
scopes:
- description: Read public social data through all MCP tools (legacy default).
  flows:
  - authorizationCode
  scope: mcp
- description: Read public Instagram data through MCP tools.
  flows:
  - authorizationCode
  scope: read:instagram
- description: Read public TikTok data through MCP tools.
  flows:
  - authorizationCode
  scope: read:tiktok
- description: Read public X (Twitter) data through MCP tools.
  flows:
  - authorizationCode
  scope: read:twitter
slug: openhandle-scopes
source_filename: openhandle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://openhandle.dev/docs/mcp\nschemes:\n- name: OpenhandleMCPOAuth\n  source: openapi/openhandle-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openhandle.dev/oauth/authorize\n    tokenUrl: https://api.openhandle.dev/oauth/token\n  description: OAuth grants for the MCP endpoint only. REST operations require OpenhandleKey.\nscopes:\n- scope: mcp\n  description: Read public social data through all MCP tools (legacy default).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openhandle-openapi.yml\n- scope: read:instagram\n  description: Read public Instagram data through MCP tools.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openhandle-openapi.yml\n- scope: read:tiktok\n  description: Read public TikTok data through MCP tools.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openhandle-openapi.yml\n- scope: read:twitter\n  description: Read public X (Twitter)\
  \ data through MCP tools.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openhandle-openapi.yml\ndocs: https://openhandle.dev/docs/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/scopes/openhandle-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Social Data
- Instagram
- TikTok
- twitter
- Reddit
- Public Data
- social-media-api
- MCP
- creator-analytics
- Social Listening
token_urls:
- https://api.openhandle.dev/oauth/token
---
