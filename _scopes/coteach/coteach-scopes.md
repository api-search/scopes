---
authorization_urls:
- https://www.coteach.ai/api/oauth/authorize
description: ''
docs: https://www.coteach.ai/.well-known/oauth-protected-resource
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Coteach Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoTeach publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoTeach API on a user''s behalf.


  Tokens are issued from https://www.coteach.ai/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoTeach
provider_slug: coteach
schemes:
- flows:
  - authorizationUrl: https://www.coteach.ai/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.coteach.ai/api/oauth/token
  name: OAuth2
  source: https://www.coteach.ai/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- email
- profile
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token identifying the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access to the authenticated user's basic profile information.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for long-lived, offline access.
  flows:
  - authorizationCode
  scope: offline_access
slug: coteach-scopes
source_filename: coteach-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.coteach.ai/.well-known/oauth-authorization-server\ndocs: https://www.coteach.ai/.well-known/oauth-protected-resource\nschemes:\n- name: OAuth2\n  source: https://www.coteach.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.coteach.ai/api/oauth/authorize\n    tokenUrl: https://www.coteach.ai/api/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token identifying the user.\n  flows:\n  - authorizationCode\n  sources:\n  - https://www.coteach.ai/.well-known/oauth-authorization-server\n- scope: email\n  description: Access to the authenticated user's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - https://www.coteach.ai/.well-known/oauth-authorization-server\n- scope: profile\n  description: Access to the authenticated user's basic profile information.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - https://www.coteach.ai/.well-known/oauth-authorization-server\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n  flows:\n  - authorizationCode\n  sources:\n  - https://www.coteach.ai/.well-known/oauth-authorization-server\nnotes: Scopes advertised by CoTeach's OAuth authorization server. The protected-resource\n  metadata for the MCP server (/api/mcp) requires the openid, email, and profile\n  scopes; offline_access is additionally offered for refresh tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coteach/refs/heads/main/scopes/coteach-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Education
- EdTech
- Mathematics
- K-12
- Teachers
- Curriculum
- Lesson Planning
- AI Assistant
- Illustrative Mathematics
- MCP
token_urls:
- https://www.coteach.ai/api/oauth/token
---
