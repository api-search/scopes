---
authorization_urls:
- https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sessionai Scopes
name_suffix: OAuth Scopes
note: Scopes are read from the live RFC 8414 authorization-server metadata that Session AI's own RFC 9728 protected-resource metadata names for its MCP server. Session AI publishes no scopes reference page of its own, and these are the generic OIDC scopes advertised by the authorization server rather than Session AI product permissions. The REST platform API is API-key authenticated and has no OAuth scope surface at all.
overview: 'Session AI publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Session AI API on a user''s behalf.


  Tokens are issued from https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Session AI
provider_slug: sessionai
schemes:
- flows:
  - authorizationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token
  issuer: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1
  name: mcp-oauth
  source: well-known/sessionai-oauth-authorization-server.json
scope_count: 5
scope_names:
- openid
- profile
- email
- phone
- offline_access
scopes:
- description: OpenID Connect sign-in; returns an ID token for the authenticated subject.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the authenticated user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the authenticated user's phone claim.
  flows:
  - authorizationCode
  scope: phone
- description: Issues a refresh token so the client can act without the user present.
  flows:
  - authorizationCode
  scope: offline_access
slug: sessionai-scopes
source_filename: sessionai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/.well-known/oauth-authorization-server\nnote: >-\n  Scopes are read from the live RFC 8414 authorization-server metadata that Session AI's\n  own RFC 9728 protected-resource metadata names for its MCP server. Session AI publishes\n  no scopes reference page of its own, and these are the generic OIDC scopes advertised by\n  the authorization server rather than Session AI product permissions. The REST platform\n  API is API-key authenticated and has no OAuth scope surface at all.\napplies_to: https://sessionai.com/mcp\nschemes:\n- name: mcp-oauth\n  issuer: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1\n  source: well-known/sessionai-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/authorize\n    tokenUrl: https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token\nscopes:\n-\
  \ scope: openid\n  description: OpenID Connect sign-in; returns an ID token for the authenticated subject.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the authenticated user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the authenticated user's email claim.\n  flows: [authorizationCode]\n- scope: phone\n  description: Access to the authenticated user's phone claim.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issues a refresh token so the client can act without the user present.\n  flows: [authorizationCode]\nscope_count: 5\nproduct_scopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sessionai/refs/heads/main/scopes/sessionai-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- Ecommerce
- Retail
- Personalization
- Marketing
- Agentic AI
- Decisioning
- Customer Data
- Events
- Real Time
- MCP
token_urls:
- https://jsaqyxhgmkgcyaocjnzz.supabase.co/auth/v1/oauth/token
---
