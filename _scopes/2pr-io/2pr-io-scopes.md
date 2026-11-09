---
authorization_urls:
- https://2pr.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: 2Pr Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: '2pr publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 2pr API on a user''s behalf.


  Tokens are issued from https://2pr.io/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 2pr
provider_slug: 2pr-io
schemes:
- description: '"Sign in with 2pr". Authorization code with PKCE S256; register a client first.'
  flows:
  - authorizationUrl: https://2pr.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://2pr.io/api/oauth/token
  name: oauth2
  source: openapi/2pr-io-openapi.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Call the 2pr.io MCP tools on behalf of the signed-in user.
  flows:
  - authorizationCode
  scope: mcp
slug: 2pr-io-scopes
source_filename: 2pr-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/2pr-io-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/2pr-io-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://2pr.io/oauth/authorize\n    tokenUrl: https://2pr.io/api/oauth/token\n  description: '\"Sign in with 2pr\". Authorization code with PKCE S256; register a client first.'\nscopes:\n- scope: mcp\n  description: Call the 2pr.io MCP tools on behalf of the signed-in user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/2pr-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/2pr-io/scopes/2pr-io-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Artificial Intelligence
- LinkedIn
- Marketing
- Automation
- Software-as-a-Service
token_bound: false
token_urls:
- https://2pr.io/api/oauth/token
---
