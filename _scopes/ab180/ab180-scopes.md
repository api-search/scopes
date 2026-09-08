---
api_specs:
- filename: overview
  format: yaml
  label: Airbridge API
  slug: airbridge-api
  spec_type: Postman
  url: https://www.postman.com/airbridge-engineering/workspace/airbridge-api/overview
authorization_urls:
- https://mcp.airbridge.io/oauth/authorize
description: ''
docs: https://www.airbridge.io/en/product/airbridge-ai
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Ab180 Scopes
name_suffix: OAuth Scopes
note: The Airbridge REST API uses bearer API tokens with no OAuth scope surface — its only permission granularity is the two token TYPES (API Token, Tracking Link API Token), recorded in authentication/ab180-authentication.yml. The only OAuth surface Airbridge operates is the MCP server, whose scopes are read here from its live RFC 8414 / RFC 9728 / OpenID Connect Discovery documents.
overview: 'Ab180 publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ab180 API on a user''s behalf.


  Tokens are issued from https://mcp.airbridge.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ab180
provider_slug: ab180
schemes:
- flows:
  - authorizationUrl: https://mcp.airbridge.io/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://mcp.airbridge.io/oauth/token
  issuer: https://mcp.airbridge.io
  name: airbridgeMcpOAuth
  resource: https://mcp.airbridge.io/mcp
  source: well-known/ab180-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Request an OpenID Connect ID token identifying the Airbridge user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated Airbridge user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the authenticated Airbridge user.
  flows:
  - authorizationCode
  scope: email
slug: ab180-scopes
source_filename: ab180-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://mcp.airbridge.io/.well-known/oauth-authorization-server\ndocs: https://www.airbridge.io/en/product/airbridge-ai\nnote: 'The Airbridge REST API uses bearer API tokens with no OAuth scope surface — its\n  only permission granularity is the two token TYPES (API Token, Tracking Link API Token),\n  recorded in authentication/ab180-authentication.yml. The only OAuth surface Airbridge\n  operates is the MCP server, whose scopes are read here from its live RFC 8414 / RFC 9728\n  / OpenID Connect Discovery documents.'\nschemes:\n- name: airbridgeMcpOAuth\n  source: well-known/ab180-oauth-authorization-server.json\n  issuer: https://mcp.airbridge.io\n  resource: https://mcp.airbridge.io/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.airbridge.io/oauth/authorize\n    tokenUrl: https://mcp.airbridge.io/oauth/token\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: openid\n  description: Request\
  \ an OpenID Connect ID token identifying the Airbridge user.\n  flows: [authorizationCode]\n  sources: [well-known/ab180-oauth-authorization-server.json, well-known/ab180-oauth-protected-resource.json]\n- scope: profile\n  description: Basic profile claims for the authenticated Airbridge user.\n  flows: [authorizationCode]\n  sources: [well-known/ab180-oauth-authorization-server.json, well-known/ab180-oauth-protected-resource.json]\n- scope: email\n  description: Email address claim for the authenticated Airbridge user.\n  flows: [authorizationCode]\n  sources: [well-known/ab180-oauth-authorization-server.json, well-known/ab180-oauth-protected-resource.json]\ngaps:\n  note: 'The advertised scopes are identity scopes only. Nothing in the published metadata\n    expresses what Airbridge DATA an MCP token may reach — data authorization is implied\n    by the user''s dashboard permissions, not by a scope. No scopes/permissions reference\n    page is published.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab180/refs/heads/main/scopes/ab180-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Attribution
- Mobile Measurement
- Marketing
- Analytics
- Advertising
- Deep Linking
- Mobile
- Reporting
- South Korea
token_urls:
- https://mcp.airbridge.io/oauth/token
---
