---
authorization_urls:
- https://login.tofuhq.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- deviceCode
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Tofu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tofu publishes 4 OAuth 2.0 scopes via the authorizationCode, deviceCode, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tofu API on a user''s behalf.


  Tokens are issued from https://login.tofuhq.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tofu
provider_slug: tofu
schemes:
- flows:
  - authorizationUrl: https://login.tofuhq.com/oauth2/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://login.tofuhq.com/oauth2/token
  - deviceAuthorizationUrl: https://login.tofuhq.com/oauth2/device_authorization
    flow: deviceCode
    tokenUrl: https://login.tofuhq.com/oauth2/token
  - flow: refreshToken
    tokenUrl: https://login.tofuhq.com/oauth2/token
  issuer: https://login.tofuhq.com
  name: TofuOAuth2
  source: well-known/tofu-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OIDC scope requesting an ID token.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Standard OIDC claim set covering basic profile attributes.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Standard OIDC claim set covering the user's email address.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Requests a refresh token for long-lived access.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
slug: tofu-scopes
source_filename: tofu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://login.tofuhq.com/.well-known/openid-configuration\nalso_source: https://login.tofuhq.com/.well-known/oauth-authorization-server\ndocs: null\nschemes:\n- name: TofuOAuth2\n  source: well-known/tofu-oauth-authorization-server.json\n  issuer: https://login.tofuhq.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.tofuhq.com/oauth2/authorize\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n    code_challenge_methods: [S256]\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.tofuhq.com/oauth2/device_authorization\n    tokenUrl: https://login.tofuhq.com/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://login.tofuhq.com/oauth2/token\nscopes:\n- scope: openid\n  description: Standard OIDC scope requesting an ID token.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/tofu-openid-configuration.json,\n    well-known/tofu-oauth-authorization-server.json]\n\
  - scope: profile\n  description: Standard OIDC claim set covering basic profile attributes.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/tofu-openid-configuration.json,\n    well-known/tofu-oauth-authorization-server.json]\n- scope: email\n  description: Standard OIDC claim set covering the user's email address.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/tofu-openid-configuration.json,\n    well-known/tofu-oauth-authorization-server.json]\n- scope: offline_access\n  description: Requests a refresh token for long-lived access.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/tofu-openid-configuration.json,\n    well-known/tofu-oauth-authorization-server.json]\nsummary:\n  scope_count: 4\n  custom_scopes: 0\n  standard_oidc_scopes: 4\nnotes: >-\n  Every scope Tofu advertises is a standard OIDC scope — there are no\n  product/resource scopes (no read/write, no per-object permissions). This\n  authorization server governs application\
  \ sign-in at login.tofuhq.com only. The\n  Enrich API at api.enrich.tofuhq.com uses an opaque bearer API key with no scope\n  surface at all, so no scope model applies to it. Tofu publishes no scopes or\n  permissions reference page; these values were read directly from the two\n  discovery documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tofu/refs/heads/main/scopes/tofu-scopes.yml
summary_line: 4 scopes · authorizationCode/deviceCode/refreshToken
tags:
- Company
- Ai Ml
- Marketing
- Go-To-Market
- Sales
- Automation
- CRM
- Campaigns
- Data Enrichment
- Company Data
- People Data
- Lead Generation
- Agents
- Contact Data
token_urls:
- https://login.tofuhq.com/oauth2/token
---
