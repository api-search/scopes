---
authorization_urls:
- https://api.luciq.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Instabug Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Instabug (Luciq) publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Instabug (Luciq) API on a user''s behalf.


  Tokens are issued from https://api.luciq.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Instabug (Luciq)
provider_slug: instabug
schemes:
- description: OAuth 2.0 with Dynamic Client Registration. The Luciq MCP server advertises its authorization and token endpoints to MCP clients that register dynamically — no pre-shared client ID/secret is required.
  flows:
  - authorizationUrl: https://api.luciq.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.luciq.ai/oauth/token
  name: oauth2
  source: openapi/instabug-mcp-server-openapi.yml
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read access to applications, crashes, occurrences, hangs, bugs, and reviews
  flows:
  - authorizationCode
  scope: mcp:read
slug: instabug-scopes
source_filename: instabug-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/instabug-mcp-server-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/instabug-mcp-server-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.luciq.ai/oauth/authorize\n    tokenUrl: https://api.luciq.ai/oauth/token\n  description: OAuth 2.0 with Dynamic Client Registration. The Luciq MCP server advertises its\n    authorization and token endpoints to MCP clients that register dynamically — no pre-shared\n    client ID/secret is required.\nscopes:\n- scope: mcp:read\n  description: Read access to applications, crashes, occurrences, hangs, bugs, and reviews\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/instabug-mcp-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabug/refs/heads/main/scopes/instabug-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Agentic AI
- APM
- Application Performance Monitoring
- Bug Reporting
- Crash Reporting
- MCP
- Mobile
- Mobile Observability
- Observability
- Session Replay
token_urls:
- https://api.luciq.ai/oauth/token
---
