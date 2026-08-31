---
authorization_urls:
- https://api.thetaray.com/_mcp/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Thetaray Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ThetaRay publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ThetaRay API on a user''s behalf.


  Tokens are issued from https://api.thetaray.com/_mcp/oauth2/token-portal.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ThetaRay
provider_slug: thetaray
schemes:
- flows:
  - authorizationUrl: https://api.thetaray.com/_mcp/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal
  - flow: clientCredentials
    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal
  name: RedoclyPortalOAuth2
  source: well-known/thetaray-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in portal user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the signed-in user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access the signed-in user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so an agent or client can renew access without re-prompting.
  flows:
  - authorizationCode
  scope: offline_access
slug: thetaray-scopes
source_filename: thetaray-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://api.thetaray.com/.well-known/oauth-authorization-server\nraw: well-known/thetaray-oauth-authorization-server.json\nscope_note: >-\n  These are the OAuth 2.0 scopes advertised by the authorization server that fronts the ThetaRay\n  developer portal and its MCP endpoint on api.thetaray.com. They are identity/session scopes, not\n  ThetaRay product permissions — ThetaRay publishes no public scope or permission reference for its\n  AML monitoring and screening API, and no OpenAPI with oauth2 securitySchemes was retrievable.\nschemes:\n- name: RedoclyPortalOAuth2\n  source: well-known/thetaray-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.thetaray.com/_mcp/oauth2/auth\n    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal\n  - flow: clientCredentials\n    tokenUrl: https://api.thetaray.com/_mcp/oauth2/token-portal\nscopes:\n- scope: openid\n  description:\
  \ OpenID Connect authentication; issue an ID token for the signed-in portal user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/thetaray-oauth-authorization-server.json\n- scope: profile\n  description: Access the signed-in user's basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/thetaray-oauth-authorization-server.json\n- scope: email\n  description: Access the signed-in user's email address claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/thetaray-oauth-authorization-server.json\n- scope: offline_access\n  description: Issue a refresh token so an agent or client can renew access without re-prompting.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/thetaray-oauth-authorization-server.json\nx-evidence:\n- fetched: '2026-08-05'\n  url: https://api.thetaray.com/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-05'\n  url: https://api.thetaray.com/.well-known/oauth-protected-resource/mcp\n\
  \  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thetaray/refs/heads/main/scopes/thetaray-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- anti-money-laundering
- financial-crime
- transaction-monitoring
- sanctions-screening
- kyc
- regtech
- risk-assessment
- artificial-intelligence
- banking
- Fintech
- Payments
- Compliance
- MCP
token_urls:
- https://api.thetaray.com/_mcp/oauth2/token-portal
---
