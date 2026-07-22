---
api_specs:
- filename: sageox-openapi-original.json
  format: json
  label: SageOx API
  slug: sageox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/openapi/sageox-openapi-original.json
authorization_urls:
- https://sageox.ai/api/auth/oauth2/authorize
description: ''
docs: https://sageox.ai/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sageox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SageOx publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SageOx API on a user''s behalf.


  Tokens are issued from https://sageox.ai/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SageOx
provider_slug: sageox
schemes:
- flows:
  - authorizationUrl: https://sageox.ai/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://sageox.ai/api/auth/oauth2/token
  name: oauth2
  source: well-known/sageox-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect — issue an ID token identifying the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims (name).
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived / offline access.
  flows:
  - authorizationCode
  scope: offline_access
slug: sageox-scopes
source_filename: sageox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: well-known/sageox-openid-configuration.json\ndocs: https://sageox.ai/docs/mcp\nschemes:\n- name: oauth2\n  source: well-known/sageox-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sageox.ai/api/auth/oauth2/authorize\n    tokenUrl: https://sageox.ai/api/auth/oauth2/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect — issue an ID token identifying the user.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims (name).\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email and email_verified claims.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived / offline access.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes are the OAuth/OIDC authorization-server scopes advertised in the\n  discovery documents. MCP client\
  \ connections request a scoped grant mapped to\n  the user's SageOx account; per-resource access is further constrained by the\n  user's team/bubble permissions rather than by additional OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sageox/refs/heads/main/scopes/sageox-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- AI Agents
- Developer Tools
- Knowledge Management
- Agent Memory
- Model Context Protocol
- MCP
- CLI
- Team Collaboration
- Agentic Engineering
token_urls:
- https://sageox.ai/api/auth/oauth2/token
---
