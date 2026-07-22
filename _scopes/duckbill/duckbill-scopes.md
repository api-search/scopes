---
authorization_urls:
- https://clerk.getduckbill.com/oauth/authorize
description: ''
docs: https://getduckbill.com/platform
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Duckbill Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Duckbill publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Duckbill API on a user''s behalf.


  Tokens are issued from https://clerk.getduckbill.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Duckbill
provider_slug: duckbill
schemes:
- flows:
  - authorizationUrl: https://clerk.getduckbill.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.getduckbill.com/oauth/token
  name: OAuth2
  source: well-known/duckbill-oauth-authorization-server.json
scope_count: 6
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
scopes:
- description: OpenID Connect sign-in; issue an ID token for the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to basic profile claims (name, given_name, family_name, picture, preferred_username).
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Read the user's public metadata stored in Clerk.
  flows:
  - authorizationCode
  scope: public_metadata
- description: Read the user's private metadata stored in Clerk.
  flows:
  - authorizationCode
  scope: private_metadata
- description: Issue a refresh token for long-lived, offline access.
  flows:
  - authorizationCode
  scope: offline_access
slug: duckbill-scopes
source_filename: duckbill-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://clerk.getduckbill.com/.well-known/oauth-authorization-server\ndocs: https://getduckbill.com/platform\nnotes: >-\n  Scopes advertised by Duckbill's OAuth 2.0 / OIDC authorization server\n  (Clerk-hosted on clerk.getduckbill.com). These are the OIDC identity scopes the\n  \"Connect to Claude\" MCP OAuth flow requests; Duckbill publishes no separate\n  fine-grained API-permission scope reference.\nschemes:\n- name: OAuth2\n  source: well-known/duckbill-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.getduckbill.com/oauth/authorize\n    tokenUrl: https://clerk.getduckbill.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token for the authenticated user.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to basic profile claims (name, given_name, family_name, picture, preferred_username).\n  flows:\
  \ [authorizationCode]\n- scope: email\n  description: Access to the user's email and email_verified claims.\n  flows: [authorizationCode]\n- scope: public_metadata\n  description: Read the user's public metadata stored in Clerk.\n  flows: [authorizationCode]\n- scope: private_metadata\n  description: Read the user's private metadata stored in Clerk.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duckbill/refs/heads/main/scopes/duckbill-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Consumer
- AI Assistant
- Personal Assistant
- Task Automation
- Agents
- MCP
- Concierge
token_urls:
- https://clerk.getduckbill.com/oauth/token
---
