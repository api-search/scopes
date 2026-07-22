---
authorization_urls:
- https://api.superset.sh/api/auth/oauth2/authorize
description: ''
docs: https://docs.superset.sh/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Superset Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Superset publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Superset API on a user''s behalf.


  Tokens are issued from https://api.superset.sh/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Superset
provider_slug: superset
schemes:
- flows:
  - authorizationUrl: https://api.superset.sh/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.superset.sh/api/auth/oauth2/token
  issuer: https://api.superset.sh
  name: OAuth2.1
  source: https://api.superset.sh/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access to the user's basic profile.
  flows: []
  scope: profile
- description: Access to the user's email address.
  flows: []
  scope: email
- description: Issue a refresh token for offline/long-lived access.
  flows: []
  scope: offline_access
slug: superset-scopes
source_filename: superset-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.superset.sh/.well-known/oauth-authorization-server\ndocs: https://docs.superset.sh/mcp\nschemes:\n  - name: OAuth2.1\n    source: https://api.superset.sh/.well-known/oauth-authorization-server\n    issuer: https://api.superset.sh\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.superset.sh/api/auth/oauth2/authorize\n        tokenUrl: https://api.superset.sh/api/auth/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication.\n    sources: [https://api.superset.sh/.well-known/oauth-authorization-server]\n  - scope: profile\n    description: Access to the user's basic profile.\n    sources: [https://api.superset.sh/.well-known/oauth-authorization-server]\n  - scope: email\n    description: Access to the user's email address.\n    sources: [https://api.superset.sh/.well-known/oauth-authorization-server]\n  - scope: offline_access\n    description: Issue\
  \ a refresh token for offline/long-lived access.\n    sources: [https://api.superset.sh/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superset/refs/heads/main/scopes/superset-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Developer Tools
- AI Agents
- Code Editor
- IDE
- Coding Agents
- MCP
- CLI
- SDK
- Git Worktrees
- Automation
- Y Combinator
token_urls:
- https://api.superset.sh/api/auth/oauth2/token
---
