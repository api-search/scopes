---
api_specs:
- filename: sprig-api-openapi-original.json
  format: json
  label: Sprig API
  slug: sprig-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/openapi/sprig-api-openapi-original.json
authorization_urls:
- https://app.sprig.com/oauth/authorize
description: ''
docs: https://docs.sprig.com/docs/native-ai/sprig-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sprig Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sprig publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sprig API on a user''s behalf.


  Tokens are issued from https://api.sprig.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sprig
provider_slug: sprig
schemes:
- flows:
  - authorizationUrl: https://app.sprig.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.sprig.com/oauth/register
    tokenUrl: https://api.sprig.com/oauth/token
  name: OAuth2
  source: well-known/sprig-oauth-authorization-server.json
scope_count: 5
scope_names:
- environments:read
- surveys:read
- surveys:write
- responses:read
- themes:read
scopes:
- description: Read access to Sprig environments (product/environment metadata).
  flows:
  - authorizationCode
  scope: environments:read
- description: Read access to survey/study configurations.
  flows:
  - authorizationCode
  scope: surveys:read
- description: Create and modify surveys/studies (e.g. drafting studies from AI clients).
  flows:
  - authorizationCode
  scope: surveys:write
- description: Read access to study responses.
  flows:
  - authorizationCode
  scope: responses:read
- description: Read access to AI-identified themes and their associated responses.
  flows:
  - authorizationCode
  scope: themes:read
slug: sprig-scopes
source_filename: sprig-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://mcp.sprig.com/.well-known/oauth-authorization-server\ndocs: https://docs.sprig.com/docs/native-ai/sprig-mcp\nnotes: >-\n  Sprig's REST API (api.sprig.com) authenticates with a static API key\n  (Authorization: API-Key / Bearer). OAuth 2.0 scopes are published for the\n  Sprig MCP server (mcp.sprig.com), whose authorization server is api.sprig.com.\n  Scopes below are taken verbatim from the RFC 8414 / RFC 9728 discovery metadata.\nschemes:\n  - name: OAuth2\n    source: well-known/sprig-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.sprig.com/oauth/authorize\n        tokenUrl: https://api.sprig.com/oauth/token\n        registrationUrl: https://api.sprig.com/oauth/register\n        pkce: S256\nscopes:\n  - scope: environments:read\n    description: Read access to Sprig environments (product/environment metadata).\n    flows: [authorizationCode]\n  -\
  \ scope: surveys:read\n    description: Read access to survey/study configurations.\n    flows: [authorizationCode]\n  - scope: surveys:write\n    description: Create and modify surveys/studies (e.g. drafting studies from AI clients).\n    flows: [authorizationCode]\n  - scope: responses:read\n    description: Read access to study responses.\n    flows: [authorizationCode]\n  - scope: themes:read\n    description: Read access to AI-identified themes and their associated responses.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprig/refs/heads/main/scopes/sprig-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Product Research
- Surveys
- User Insights
- Customer Experience
- Analytics
- Product Analytics
- AI
- SaaS
token_urls:
- https://api.sprig.com/oauth/token
---
