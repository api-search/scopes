---
api_specs:
- filename: n3xt-openapi-original.json
  format: json
  label: N3XT API
  slug: n3xt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/openapi/n3xt-openapi-original.json
authorization_urls: []
description: ''
docs: https://helpcenter.n3xt.io/en/articles/12118191-api-getting-started
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: N3Xt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'N3XT publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the N3XT API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: N3XT
provider_slug: n3xt
schemes:
- authorizationUrl: https://authn.n3xt.io
  issuer: https://authn.n3xt.io
  name: OAuth2
  source: https://authn.n3xt.io/.well-known/openid-configuration
  tokenUrl: https://authn.n3xt.io/v1/oauth2/token
scope_count: 8
scope_names:
- openid
- profile
- email
- phone
- offline_access
- full_access
- mcp:read
- mcp:write
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the authenticated principal's profile claims.
  flows: []
  scope: profile
- description: Access to the principal's email address claim.
  flows: []
  scope: email
- description: Access to the principal's phone number claim.
  flows: []
  scope: phone
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
- description: Full access to the N3XT business banking API surface.
  flows: []
  scope: full_access
- description: Read-only access through the N3XT hosted MCP server (mcp.n3xt.io).
  flows: []
  scope: mcp:read
- description: Write / action access through the N3XT hosted MCP server (mcp.n3xt.io).
  flows: []
  scope: mcp:write
slug: n3xt-scopes
source_filename: n3xt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://authn.n3xt.io/.well-known/openid-configuration\ndocs: https://helpcenter.n3xt.io/en/articles/12118191-api-getting-started\nnotes: >-\n  The N3XT OpenAPI declares only a bearerAuth (JWT) scheme with no per-operation\n  scope requirements, so scopes are not derivable from the spec. The N3XT\n  authorization server (authn.n3xt.io) publishes the OAuth 2.0 / OpenID Connect\n  scopes below via its well-known discovery documents. `full_access` is the\n  broad business-API scope; `mcp:read` / `mcp:write` gate the hosted N3XT MCP\n  server at mcp.n3xt.io.\nschemes:\n- name: OAuth2\n  source: https://authn.n3xt.io/.well-known/openid-configuration\n  issuer: https://authn.n3xt.io\n  authorizationUrl: https://authn.n3xt.io\n  tokenUrl: https://authn.n3xt.io/v1/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n\
  - scope: profile\n  description: Access to the authenticated principal's profile claims.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: email\n  description: Access to the principal's email address claim.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: phone\n  description: Access to the principal's phone number claim.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: offline_access\n  description: Issue a refresh token for long-lived, offline access.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: full_access\n  description: Full access to the N3XT business banking API surface.\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: mcp:read\n  description: Read-only access through the N3XT hosted MCP server (mcp.n3xt.io).\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n- scope: mcp:write\n  description: Write / action\
  \ access through the N3XT hosted MCP server (mcp.n3xt.io).\n  sources: [https://authn.n3xt.io/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/n3xt/refs/heads/main/scopes/n3xt-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Crypto
- Banking
- Payments
- Stablecoin
- Fintech
- Blockchain
- API
- MCP
token_urls: []
---
