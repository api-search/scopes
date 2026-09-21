---
api_specs:
- filename: humanbrowser-cloud-openapi.json
  format: json
  label: Human Browser API
  slug: human-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/openapi/humanbrowser-cloud-openapi.json
authorization_urls:
- https://agent.humanbrowser.cloud/authorize
description: ''
docs:
- https://agent.humanbrowser.cloud/.well-known/oauth-authorization-server
- https://agent.humanbrowser.cloud/.well-known/oauth-protected-resource
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Humanbrowser Cloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Virix Labs publishes 5 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virix Labs API on a user''s behalf.


  Tokens are issued from https://agent.humanbrowser.cloud/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virix Labs
provider_slug: humanbrowser-cloud
schemes:
- description: Least-privilege scoped access. Request only the scopes an agent needs.
  flows:
  - flow: clientCredentials
    tokenUrl: https://agent.humanbrowser.cloud/oauth/token
    tokenUrl_status: 404 (GET and POST, 2026-09-19)
  name: oauth2
  source: openapi/humanbrowser-cloud-openapi.json
- description: RFC 8414 metadata; resource https://agent.humanbrowser.cloud/mcp per RFC 9728.
  flows:
  - authorizationUrl: https://agent.humanbrowser.cloud/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://agent.humanbrowser.cloud/token
  name: mcp-oauth
  source: well-known/humanbrowser-cloud-oauth-authorization-server.json
scope_count: 5
scope_names:
- session:run
- account:read
- account:topup
- mcp:run
- mcp:read
scopes:
- description: Spawn and drive browser sessions
  flows:
  - clientCredentials
  scope: session:run
- description: Read token balance, usage and account state
  flows:
  - clientCredentials
  scope: account:read
- description: Create top-ups / purchases against the account
  flows:
  - clientCredentials
  scope: account:topup
- description: undocumented — by name, invoke MCP tools that run browser tasks
  flows:
  - authorizationCode
  scope: mcp:run
- description: undocumented — by name, read-only MCP access
  flows:
  - authorizationCode
  scope: mcp:read
slug: humanbrowser-cloud-scopes
source_filename: humanbrowser-cloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/humanbrowser-cloud-openapi.json\ndocs:\n- https://agent.humanbrowser.cloud/.well-known/oauth-authorization-server\n- https://agent.humanbrowser.cloud/.well-known/oauth-protected-resource\nsummary: >-\n  Two scope vocabularies from two OAuth surfaces that do not reference each other. The OpenAPI's oauth2\n  clientCredentials scheme declares session:run, account:read and account:topup and binds them per\n  operation — but its tokenUrl (https://agent.humanbrowser.cloud/oauth/token) 404s on GET and POST. The\n  live authorization server's RFC 8414 metadata on the same host declares mcp:run and mcp:read for the\n  MCP resource, with no per-tool binding published anywhere. Neither vocabulary is documented on a\n  scopes/permissions page (/docs/oauth 404). Every shipped integration uses the unscoped hb_live_ bearer\n  token instead.\nschemes:\n- name: oauth2\n  source: openapi/humanbrowser-cloud-openapi.json\n  flows:\n  -\
  \ flow: clientCredentials\n    tokenUrl: https://agent.humanbrowser.cloud/oauth/token\n    tokenUrl_status: 404 (GET and POST, 2026-09-19)\n  description: Least-privilege scoped access. Request only the scopes an agent needs.\n- name: mcp-oauth\n  source: well-known/humanbrowser-cloud-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://agent.humanbrowser.cloud/authorize\n    tokenUrl: https://agent.humanbrowser.cloud/token\n    pkce: S256\n  description: RFC 8414 metadata; resource https://agent.humanbrowser.cloud/mcp per RFC 9728.\nscopes:\n- scope: session:run\n  description: Spawn and drive browser sessions\n  flows:\n  - clientCredentials\n  operations: [runA2ATask]\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n- scope: account:read\n  description: Read token balance, usage and account state\n  flows:\n  - clientCredentials\n  operations: [getAccount, getUsage]\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n-\
  \ scope: account:topup\n  description: Create top-ups / purchases against the account\n  flows:\n  - clientCredentials\n  operations: [topUp]\n  sources:\n  - openapi/humanbrowser-cloud-openapi.json\n- scope: mcp:run\n  description: undocumented — by name, invoke MCP tools that run browser tasks\n  flows:\n  - authorizationCode\n  operations: []\n  sources:\n  - well-known/humanbrowser-cloud-oauth-authorization-server.json\n  - well-known/humanbrowser-cloud-oauth-protected-resource.json\n- scope: mcp:read\n  description: undocumented — by name, read-only MCP access\n  flows:\n  - authorizationCode\n  operations: []\n  sources:\n  - well-known/humanbrowser-cloud-oauth-authorization-server.json\n  - well-known/humanbrowser-cloud-oauth-protected-resource.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanbrowser-cloud/refs/heads/main/scopes/humanbrowser-cloud-scopes.yml
summary_line: 5 scopes · clientCredentials/authorizationCode
tags:
- Browser Automation
- Cloud Browser
- AI Agents
- A2A
- MCP
- Web Scraping
- Residential Proxies
- CAPTCHA Solving
- Human-in-the-Loop
- Computer Use
- agent-native
- United Kingdom
token_urls:
- https://agent.humanbrowser.cloud/oauth/token
- https://agent.humanbrowser.cloud/token
---
