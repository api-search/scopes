---
authorization_urls:
- https://app.rapidcanvas.ai/oauth/authorize
description: ''
docs: https://app.rapidcanvas.ai/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Rapidcanvas Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RapidCanvas publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RapidCanvas API on a user''s behalf.


  Tokens are issued from https://app.rapidcanvas.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RapidCanvas
provider_slug: rapidcanvas
schemes:
- flows:
  - authorizationUrl: https://app.rapidcanvas.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://app.rapidcanvas.ai/oauth/token
  name: OAuth2
  source: well-known/rapidcanvas-oauth-authorization-server.json
scope_count: 4
scope_names:
- mcp
- openid
- profile
- email
scopes:
- description: Access the RapidCanvas MCP gateway and invoke FastAPI-derived MCP tools.
  flows:
  - authorizationCode
  scope: mcp
- description: OpenID Connect authentication (issue an ID token).
  flows:
  - authorizationCode
  scope: openid
- description: Access the signed-in user's basic profile.
  flows:
  - authorizationCode
  scope: profile
- description: Access the signed-in user's email address.
  flows:
  - authorizationCode
  scope: email
slug: rapidcanvas-scopes
source_filename: rapidcanvas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.rapidcanvas.ai/.well-known/oauth-authorization-server\ndocs: https://app.rapidcanvas.ai/.well-known/oauth-authorization-server\nschemes:\n  - name: OAuth2\n    source: well-known/rapidcanvas-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.rapidcanvas.ai/oauth/authorize\n        tokenUrl: https://app.rapidcanvas.ai/oauth/token\n        pkce: S256\nscopes:\n  - scope: mcp\n    description: Access the RapidCanvas MCP gateway and invoke FastAPI-derived MCP tools.\n    flows: [authorizationCode]\n  - scope: openid\n    description: OpenID Connect authentication (issue an ID token).\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access the signed-in user's basic profile.\n    flows: [authorizationCode]\n  - scope: email\n    description: Access the signed-in user's email address.\n    flows: [authorizationCode]\nnotes: >-\n  Scopes\
  \ are advertised in the RFC 8414 OAuth 2.0 Authorization Server Metadata\n  at app.rapidcanvas.ai. The `mcp` scope fronts the MCP gateway introduced in the\n  July 14, 2026 release (FastAPI endpoints exposed as MCP tools).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidcanvas/refs/heads/main/scopes/rapidcanvas-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Agentic AI
- Data Science
- MLOps
- Enterprise AI
- AI Governance
- Low Code
- Developer Tools
token_urls:
- https://app.rapidcanvas.ai/oauth/token
---
