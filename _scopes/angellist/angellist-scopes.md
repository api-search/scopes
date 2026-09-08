---
authorization_urls:
- https://auth.angellist.com/authorize
- https://docs.angellist.com/mcp/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Angellist Scopes
name_suffix: OAuth Scopes
note: Scopes read from the provider's own live RFC 8414 / OIDC discovery documents. There is no OpenAPI to derive from — the Investor Management API is GraphQL with introspection disabled — and AngelList publishes no scopes reference page outside these discovery documents. The Investor Management API itself is API-key authenticated and has no scope surface; the scopes below belong to the web sign-in identity provider and to the documentation MCP surface.
overview: 'AngelList publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AngelList API on a user''s behalf.


  Tokens are issued from https://auth.angellist.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AngelList
provider_slug: angellist
schemes:
- flows:
  - authorizationUrl: https://auth.angellist.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.angellist.com/token
  issuer: https://auth.angellist.com
  name: AngelListOIDC
  source: well-known/angellist-auth-openid-configuration.json
- flows:
  - authorizationUrl: https://docs.angellist.com/mcp/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docs.angellist.com/mcp/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docs.angellist.com/mcp/oauth/token
  issuer: https://docs.angellist.com/mcp/oauth
  name: AngelListDocsMCPOAuth
  source: well-known/angellist-docs-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- email
- profile
- mcp:search
scopes:
- description: OpenID Connect sign-in; issue an ID token for the authenticated AngelList user.
  flows:
  - authorizationCode
  scope: openid
- description: Release the authenticated user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Release the authenticated user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Search the AngelList documentation through the documentation MCP surface advertised at https://docs.angellist.com/.well-known/oauth-protected-resource.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:search
slug: angellist-scopes
source_filename: angellist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://auth.angellist.com/.well-known/openid-configuration and\n  https://docs.angellist.com/.well-known/oauth-authorization-server\nnote: >-\n  Scopes read from the provider's own live RFC 8414 / OIDC discovery documents.\n  There is no OpenAPI to derive from — the Investor Management API is GraphQL\n  with introspection disabled — and AngelList publishes no scopes reference page\n  outside these discovery documents. The Investor Management API itself is\n  API-key authenticated and has no scope surface; the scopes below belong to the\n  web sign-in identity provider and to the documentation MCP surface.\nschemes:\n- name: AngelListOIDC\n  issuer: https://auth.angellist.com\n  source: well-known/angellist-auth-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.angellist.com/authorize\n    tokenUrl: https://auth.angellist.com/token\n- name: AngelListDocsMCPOAuth\n  issuer:\
  \ https://docs.angellist.com/mcp/oauth\n  source: well-known/angellist-docs-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docs.angellist.com/mcp/oauth/authorize\n    tokenUrl: https://docs.angellist.com/mcp/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://docs.angellist.com/mcp/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token for the authenticated AngelList user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/angellist-auth-openid-configuration.json\n- scope: email\n  description: Release the authenticated user's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/angellist-auth-openid-configuration.json\n- scope: profile\n  description: Release the authenticated user's basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/angellist-auth-openid-configuration.json\n- scope: mcp:search\n  description: >-\n\
  \    Search the AngelList documentation through the documentation MCP surface\n    advertised at https://docs.angellist.com/.well-known/oauth-protected-resource.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/angellist-docs-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angellist/refs/heads/main/scopes/angellist-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Documents
- Funds
- Investing
- Job
- Startups
- Transaction
- Venture Capital
token_urls:
- https://auth.angellist.com/token
- https://docs.angellist.com/mcp/oauth/token
---
