---
api_specs:
- filename: larridin-scout-openapi.yml
  format: yaml
  label: Larridin Scout API v1
  slug: scout-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/openapi/larridin-scout-openapi.yml
authorization_urls:
- https://login.larridin.com/oauth2/authorize
description: ''
docs: https://docs.larridin.com/api/mcp
flows:
- authorizationCode
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Larridin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Larridin publishes 4 OAuth 2.0 scopes via the authorizationCode and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Larridin API on a user''s behalf.


  Tokens are issued from https://login.larridin.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Larridin
provider_slug: larridin
schemes:
- flows:
  - authorizationUrl: https://login.larridin.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.larridin.com/oauth2/token
  - deviceAuthorizationUrl: https://login.larridin.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://login.larridin.com/oauth2/token
  issuer: https://login.larridin.com
  name: larridinOAuth
  source: well-known/larridin-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the signed-in Larridin user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the signed-in user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the signed-in user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token so the client can maintain access without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
slug: larridin-scopes
source_filename: larridin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: well-known/larridin-oauth-authorization-server.json\ndocs: https://docs.larridin.com/api/mcp\nnotes: >-\n  The Scout REST API v1 does not use OAuth — it authenticates with a company API key and gates access\n  with a single named API-key scope, ANALYTICS. OAuth 2.0 applies to the beta MCP server, whose\n  authorization server publishes the four standard OIDC/OAuth scopes below. No Larridin-specific OAuth\n  scope names are published; nothing beyond what the metadata document advertises is asserted here.\nschemes:\n- name: larridinOAuth\n  source: well-known/larridin-oauth-authorization-server.json\n  issuer: https://login.larridin.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.larridin.com/oauth2/authorize\n    tokenUrl: https://login.larridin.com/oauth2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.larridin.com/oauth2/device_authorization\n    tokenUrl: https://login.larridin.com/oauth2/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the signed-in Larridin user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/larridin-oauth-authorization-server.json\n- scope: profile\n  description: Access to the signed-in user's basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/larridin-oauth-authorization-server.json\n- scope: email\n  description: Access to the signed-in user's email address claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/larridin-oauth-authorization-server.json\n- scope: offline_access\n  description: Issues a refresh token so the client can maintain access without re-prompting the user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/larridin-oauth-authorization-server.json\napi_key_scopes:\n- scope: ANALYTICS\n  description: >-\n    Required on a company API key for every Scout API v1 endpoint. This is an API-key scope, not an\n \
  \   OAuth scope.\n  applies_to: https://scout-api.larridin.com/api/v1\n  sources:\n  - https://docs.larridin.com/api/scout-api-v1-reference\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/larridin/refs/heads/main/scopes/larridin-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode
tags:
- Company
- Artificial Intelligence
- AI Adoption
- AI Governance
- Analytics
- Developer Productivity
- Developer Intelligence
- Workflow Intelligence
- Enterprise Software
- Observability
token_urls:
- https://login.larridin.com/oauth2/token
---
