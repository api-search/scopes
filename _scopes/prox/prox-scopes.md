---
authorization_urls:
- https://signin.useprox.com/oauth2/authorize
description: ''
docs: https://useprox.com/docs/mcp
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Prox Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Prox publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Prox API on a user''s behalf.


  Tokens are issued from https://signin.useprox.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Prox
provider_slug: prox
schemes:
- flows:
  - authorizationUrl: https://signin.useprox.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://signin.useprox.com/oauth2/token
  - deviceAuthorizationUrl: https://signin.useprox.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://signin.useprox.com/oauth2/token
  issuer: https://signin.useprox.com
  name: OAuth2
  source: https://signin.useprox.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in user.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Access the user's email address claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Issue a refresh token so the client can obtain new access tokens without re-prompting.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: prox-scopes
source_filename: prox-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://mcp.useprox.com/.well-known/oauth-authorization-server\ndocs: https://useprox.com/docs/mcp\nschemes:\n  - name: OAuth2\n    source: https://signin.useprox.com/.well-known/oauth-authorization-server\n    issuer: https://signin.useprox.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://signin.useprox.com/oauth2/authorize\n        tokenUrl: https://signin.useprox.com/oauth2/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://signin.useprox.com/oauth2/device_authorization\n        tokenUrl: https://signin.useprox.com/oauth2/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token for the signed-in user.\n    flows: [authorizationCode, deviceCode]\n    sources: [https://signin.useprox.com/.well-known/openid-configuration]\n  - scope: profile\n    description: Access the user's basic profile claims.\n    flows: [authorizationCode,\
  \ deviceCode]\n    sources: [https://signin.useprox.com/.well-known/openid-configuration]\n  - scope: email\n    description: Access the user's email address claim.\n    flows: [authorizationCode, deviceCode]\n    sources: [https://signin.useprox.com/.well-known/openid-configuration]\n  - scope: offline_access\n    description: Issue a refresh token so the client can obtain new access tokens without re-prompting.\n    flows: [authorizationCode, deviceCode]\n    sources: [https://signin.useprox.com/.well-known/openid-configuration]\nnotes: >-\n  Prox's authorization server (WorkOS AuthKit) advertises the standard OIDC scope\n  set only. Prox does not publish product-level (resource) scopes; MCP access is\n  gated per user by the signed-in workspace's own permissions rather than by OAuth\n  scope, and every tool call is attributed to the user's identity.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prox/refs/heads/main/scopes/prox-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Artificial Intelligence
- MCP
- Model Context Protocol
- Manufacturing
- Product Support
- Knowledge Base
- Documentation
- Agents
token_urls:
- https://signin.useprox.com/oauth2/token
---
