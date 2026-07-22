---
authorization_urls:
- https://clerk.getmilana.ai/oauth/authorize
description: ''
docs: https://clerk.com/docs/oauth/scoped-access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Vantara Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Milana publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Milana API on a user''s behalf.


  Tokens are issued from https://clerk.getmilana.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Milana
provider_slug: vantara
schemes:
- flows:
  - authorizationUrl: https://clerk.getmilana.ai/oauth/authorize
    dynamic_client_registration: https://clerk.getmilana.ai/oauth/register
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    tokenUrl: https://clerk.getmilana.ai/oauth/token
  issuer: https://clerk.getmilana.ai
  name: OAuth2
  source: well-known/vantara-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: OpenID Connect authentication (standard OIDC scope).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's profile claims (standard OIDC scope).
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email address (standard OIDC scope).
  flows:
  - authorizationCode
  scope: email
- description: Read the user's public metadata (Clerk scoped-access scope).
  flows:
  - authorizationCode
  scope: public_metadata
- description: Read the user's private metadata (Clerk scoped-access scope).
  flows:
  - authorizationCode
  scope: private_metadata
- description: Issue a refresh token for long-lived access (standard OAuth scope).
  flows:
  - authorizationCode
  scope: offline_access
- description: Read the user's organization membership (Clerk scoped-access scope).
  flows:
  - authorizationCode
  scope: user:org:read
slug: vantara-scopes
source_filename: vantara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.getmilana.ai/.well-known/oauth-authorization-server\ndocs: https://clerk.com/docs/oauth/scoped-access\nnotes: >-\n  Milana (formerly Vantara) publishes no OpenAPI, but its hosted MCP server at\n  https://app.getmilana.ai/mcp authenticates via OAuth 2.0 against the Clerk-run\n  authorization server at https://clerk.getmilana.ai. Scopes below are exactly\n  the scopes_supported list from the RFC 8414 authorization-server metadata.\nschemes:\n  - name: OAuth2\n    source: well-known/vantara-oauth-authorization-server.json\n    issuer: https://clerk.getmilana.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.getmilana.ai/oauth/authorize\n        tokenUrl: https://clerk.getmilana.ai/oauth/token\n        pkce: S256\n        refresh_token: true\n        dynamic_client_registration: https://clerk.getmilana.ai/oauth/register\nscopes:\n  - scope: openid\n    description: OpenID Connect\
  \ authentication (standard OIDC scope).\n    flows: [authorizationCode]\n  - scope: profile\n    description: Access to the user's profile claims (standard OIDC scope).\n    flows: [authorizationCode]\n  - scope: email\n    description: Access to the user's email address (standard OIDC scope).\n    flows: [authorizationCode]\n  - scope: public_metadata\n    description: Read the user's public metadata (Clerk scoped-access scope).\n    flows: [authorizationCode]\n  - scope: private_metadata\n    description: Read the user's private metadata (Clerk scoped-access scope).\n    flows: [authorizationCode]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access (standard OAuth scope).\n    flows: [authorizationCode]\n  - scope: 'user:org:read'\n    description: Read the user's organization membership (Clerk scoped-access scope).\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantara/refs/heads/main/scopes/vantara-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- AI
- Session Replay
- Product Analytics
- Developer Tools
- Agents
- SDK
token_urls:
- https://clerk.getmilana.ai/oauth/token
---
