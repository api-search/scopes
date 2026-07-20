---
authorization_urls:
- https://api.jasper.ai/oauth2/authorize
description: ''
docs: https://developers.jasper.ai/docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jasper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jasper publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jasper API on a user''s behalf.


  Tokens are issued from https://api.jasper.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jasper
provider_slug: jasper
schemes:
- flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.jasper.ai/oauth2/token
  name: OAuth2
  source: https://api.jasper.ai/.well-known/oauth-authorization-server
scope_count: 6
scope_names:
- mcp
- user
- user:read
- openid
- email
- profile
scopes:
- description: Access the Jasper hosted MCP server tools (brand voices, audiences, agents, content generation).
  flows:
  - authorizationCode
  scope: mcp
- description: Act on behalf of the authenticated Jasper user (default user scope for API/agent access).
  flows:
  - authorizationCode
  scope: user
- description: Read the authenticated user's Jasper profile and workspace membership.
  flows:
  - authorizationCode
  scope: user:read
- description: OpenID Connect authentication — issue an ID token for the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: jasper-scopes
source_filename: jasper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://api.jasper.ai/.well-known/openid-configuration ;\n  https://api.jasper.ai/.well-known/oauth-authorization-server\ndocs: https://developers.jasper.ai/docs/authentication\nschemes:\n- name: OAuth2\n  source: https://api.jasper.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\nscopes:\n- scope: mcp\n  description: Access the Jasper hosted MCP server tools (brand voices, audiences, agents, content generation).\n  flows: [authorizationCode]\n- scope: user\n  description: Act on behalf of the authenticated Jasper user (default user scope for API/agent access).\n  flows: [authorizationCode]\n- scope: user:read\n  description: Read the authenticated user's Jasper profile and workspace membership.\n  flows: [authorizationCode]\n- scope: openid\n  description: OpenID Connect authentication\
  \ — issue an ID token for the user.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email address claim.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/scopes/jasper-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
token_urls:
- https://api.jasper.ai/oauth2/token
---
