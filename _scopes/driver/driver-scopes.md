---
authorization_urls:
- https://api.us1.driverai.com/mcp/authorize
description: ''
docs: https://www.driver.ai/docs/mcp-setup
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Driver Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Driver publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Driver API on a user''s behalf.


  Tokens are issued from https://api.us1.driverai.com/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Driver
provider_slug: driver
schemes:
- flows:
  - authorizationUrl: https://api.us1.driverai.com/mcp/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.us1.driverai.com/mcp/token
  name: oauth2
  source: https://api.us1.driverai.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect authentication of the acting user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email address.
  flows:
  - authorizationCode
  scope: email
slug: driver-scopes
source_filename: driver-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.us1.driverai.com/.well-known/oauth-authorization-server\ndocs: https://www.driver.ai/docs/mcp-setup\nschemes:\n- name: oauth2\n  source: https://api.us1.driverai.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.us1.driverai.com/mcp/authorize\n    tokenUrl: https://api.us1.driverai.com/mcp/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the acting user.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email address.\n  flows: [authorizationCode]\nnotes: >-\n  The MCP OAuth 2.1 authorization server advertises only identity scopes\n  (openid/profile/email). Resource authorization is enforced by Driver's\n  role-based access model (Source Admin / Source Member, direct or\
  \ team-\n  inherited), not by OAuth scopes. Personal access tokens inherit the user's\n  role; machine keys are granted per source.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/driver/refs/heads/main/scopes/driver-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- AI
- Developer Tools
- Code Documentation
- MCP
- Codebase Intelligence
- Agents
- Developer Experience
token_urls:
- https://api.us1.driverai.com/mcp/token
---
