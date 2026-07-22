---
authorization_urls:
- https://nlp.api.production.unwrap.ai/oauth/authorize
description: ''
docs: https://docs.unwrap.ai/articles/6412771011-unwrap-mcp
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Unwrap Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 scopes advertised by the Unwrap MCP / NLP API authorization server discovery document. Scopes follow a team:<team_id>:<resource>:<action> pattern; the wildcard "*" denotes any team the token is authorized for. All published scopes are read-only.
overview: 'Unwrap publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unwrap API on a user''s behalf.


  Tokens are issued from https://nlp.api.production.unwrap.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unwrap
provider_slug: unwrap
schemes:
- flows:
  - authorizationUrl: https://nlp.api.production.unwrap.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token
  - flow: clientCredentials
    tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token
  name: oauth2
  source: well-known/unwrap-oauth-authorization-server.json
scope_count: 5
scope_names:
- team:*:teams:read
- team:*:groups:read
- team:*:charts:read
- team:*:filters:read
- team:*:entries:read
scopes:
- description: Read access to teams / views.
  flows:
  - authorizationCode
  - clientCredentials
  scope: team:*:teams:read
- description: Read access to feedback groups.
  flows:
  - authorizationCode
  - clientCredentials
  scope: team:*:groups:read
- description: Read access to charts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: team:*:charts:read
- description: Read access to filters.
  flows:
  - authorizationCode
  - clientCredentials
  scope: team:*:filters:read
- description: Read access to feedback entries.
  flows:
  - authorizationCode
  - clientCredentials
  scope: team:*:entries:read
slug: unwrap-scopes
source_filename: unwrap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/unwrap-oauth-authorization-server.json\ndocs: https://docs.unwrap.ai/articles/6412771011-unwrap-mcp\nnote: >-\n  OAuth 2.0 scopes advertised by the Unwrap MCP / NLP API authorization server\n  discovery document. Scopes follow a team:<team_id>:<resource>:<action>\n  pattern; the wildcard \"*\" denotes any team the token is authorized for. All\n  published scopes are read-only.\nschemes:\n  - name: oauth2\n    source: well-known/unwrap-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://nlp.api.production.unwrap.ai/oauth/authorize\n        tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://nlp.api.production.unwrap.ai/oauth/token\nscopes:\n  - scope: team:*:teams:read\n    description: Read access to teams / views.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/unwrap-oauth-authorization-server.json]\n\
  \  - scope: team:*:groups:read\n    description: Read access to feedback groups.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/unwrap-oauth-authorization-server.json]\n  - scope: team:*:charts:read\n    description: Read access to charts.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/unwrap-oauth-authorization-server.json]\n  - scope: team:*:filters:read\n    description: Read access to filters.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/unwrap-oauth-authorization-server.json]\n  - scope: team:*:entries:read\n    description: Read access to feedback entries.\n    flows: [authorizationCode, clientCredentials]\n    sources: [well-known/unwrap-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unwrap/refs/heads/main/scopes/unwrap-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Ai Apps
- Customer Feedback
- Customer Intelligence
- Product Analytics
- Voice of Customer
- NLP
- GraphQL
- MCP
token_urls:
- https://nlp.api.production.unwrap.ai/oauth/token
---
