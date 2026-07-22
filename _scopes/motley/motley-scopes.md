---
authorization_urls:
- https://clerk.motley.ai/oauth/authorize
description: Motley Cloud exposes an OAuth 2.0 authorization server (RFC 8414 metadata, backed by Clerk) at issuer https://app.motley.ai. Scopes are advertised in the server metadata's scopes_supported. Authorization code flow with PKCE (S256); dynamic client registration is supported.
docs: https://clerk.com/docs/oauth/scoped-access
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Motley Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Motley publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Motley API on a user''s behalf.


  Tokens are issued from https://clerk.motley.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Motley
provider_slug: motley
schemes:
- flows:
  - authorizationUrl: https://clerk.motley.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://clerk.motley.ai/oauth/token
  name: OAuth2
  source: well-known/motley-oauth-authorization-server.json
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
- description: OpenID Connect authentication (issue an ID token).
  flows: []
  scope: openid
- description: Access the user's basic profile claims (name).
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
- description: Read the user's public metadata.
  flows: []
  scope: public_metadata
- description: Read the user's private metadata.
  flows: []
  scope: private_metadata
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
- description: Read the user's organization membership/context.
  flows: []
  scope: user:org:read
slug: motley-scopes
source_filename: motley-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.motley.ai/.well-known/oauth-authorization-server\ndocs: https://clerk.com/docs/oauth/scoped-access\ndescription: >-\n  Motley Cloud exposes an OAuth 2.0 authorization server (RFC 8414 metadata,\n  backed by Clerk) at issuer https://app.motley.ai. Scopes are advertised in the\n  server metadata's scopes_supported. Authorization code flow with PKCE (S256);\n  dynamic client registration is supported.\nissuer: https://app.motley.ai\nschemes:\n- name: OAuth2\n  source: well-known/motley-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.motley.ai/oauth/authorize\n    tokenUrl: https://clerk.motley.ai/oauth/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication (issue an ID token).\n- scope: profile\n  description: Access the user's basic profile claims (name).\n- scope: email\n  description: Access the user's email address.\n\
  - scope: public_metadata\n  description: Read the user's public metadata.\n- scope: private_metadata\n  description: Read the user's private metadata.\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n- scope: \"user:org:read\"\n  description: Read the user's organization membership/context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motley/refs/heads/main/scopes/motley-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Semantic Layer
- Business Intelligence
- Analytics
- AI Agents
- MCP
- SQL
- Data
- Reporting
token_urls:
- https://clerk.motley.ai/oauth/token
---
