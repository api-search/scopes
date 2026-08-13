---
api_specs:
- filename: yieldmo-dcs-mcp-openapi.json
  format: json
  label: Yieldmo DCS Reporting API
  slug: yieldmo-dcs-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-dcs-mcp-openapi.json
authorization_urls:
- https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Yieldmo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yieldmo publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yieldmo API on a user''s behalf.


  Tokens are issued from https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yieldmo
provider_slug: yieldmo
schemes:
- flows:
  - authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token
  issuer: https://api.yieldmo.com/dcs/mcp
  name: mcp-oauth2
  source: well-known/yieldmo-oauth-authorization-server.json
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: Standard OpenID Connect scope; returns the subject identifier. The only scope the protected resource itself advertises as required.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Standard OpenID Connect scope; returns basic profile claims.
  flows:
  - authorizationCode
  - implicit
  scope: profile
- description: Standard OpenID Connect scope; returns the email claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
slug: yieldmo-scopes
source_filename: yieldmo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://api.yieldmo.com/.well-known/oauth-authorization-server (scopes_supported) and\n  https://api.yieldmo.com/.well-known/oauth-protected-resource (scopes_supported for the resource)\ndocs: null\ndocs_note: >-\n  Yieldmo publishes no scopes or permissions reference page. Everything below was read off the\n  provider's own OAuth discovery documents. The OpenAPI at openapi/yieldmo-dcs-mcp-openapi.json\n  declares no securitySchemes at all, so no operation-level scope requirements can be derived —\n  the scope surface is identity-only.\n\nschemes:\n  - name: mcp-oauth2\n    source: well-known/yieldmo-oauth-authorization-server.json\n    issuer: https://api.yieldmo.com/dcs/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize\n        tokenUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token\n\nscopes:\n  - scope:\
  \ openid\n    description: Standard OpenID Connect scope; returns the subject identifier. The only scope the protected resource itself advertises as required.\n    flows: [authorizationCode, implicit]\n    required_by_resource: true\n    sources:\n      - well-known/yieldmo-oauth-authorization-server.json\n      - well-known/yieldmo-oauth-protected-resource.json\n  - scope: profile\n    description: Standard OpenID Connect scope; returns basic profile claims.\n    flows: [authorizationCode, implicit]\n    required_by_resource: false\n    sources: [well-known/yieldmo-oauth-authorization-server.json]\n  - scope: email\n    description: Standard OpenID Connect scope; returns the email claim.\n    flows: [authorizationCode, implicit]\n    required_by_resource: false\n    sources: [well-known/yieldmo-oauth-authorization-server.json]\n\nanalysis: >-\n  All three scopes are the stock OpenID Connect set emitted by an Amazon Cognito user pool. Yieldmo\n  has defined NO resource-server scopes of\
  \ its own — there is no read/write split, no per-report or\n  per-advertiser scope, and no scope that constrains which campaigns or advertisers a token can\n  reach. Authorization for the 19 campaign-reporting operations is therefore entirely implicit in\n  the identity, enforced server-side and invisible to the client. An agent cannot request least\n  privilege against this API because no narrower privilege is offered.\n\nscope_count: 3\nprovider_defined_scope_count: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/scopes/yieldmo-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Advertising
- Programmatic
- Native Advertising
- Ad Exchange
- Publisher Monetization
- Header Bidding
- Contextual Targeting
- Ad Formats
- Supply-Side Platform
- SSP
- Campaign Reporting
- Attention Analytics
- MCP
- Prebid
- AdTech
token_urls:
- https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token
---
