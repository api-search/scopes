---
authorization_urls:
- https://moneyfellows.com/umbraco/delivery/api/v1/security/member/authorize
description: ''
docs: https://moneyfellows.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mfellows Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MFellows publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MFellows API on a user''s behalf.


  Tokens are issued from https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MFellows
provider_slug: mfellows
schemes:
- flows:
  - authorizationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/authorize
    flow: authorizationCode
    tokenUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token
  name: oauth2
  source: well-known/mfellows-oauth-authorization-server.json
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect authentication; request an ID token for the authenticated member.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the client can obtain new access tokens without re-authentication.
  flows:
  - authorizationCode
  scope: offline_access
slug: mfellows-scopes
source_filename: mfellows-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://moneyfellows.com/.well-known/openid-configuration\ndocs: https://moneyfellows.com/.well-known/openid-configuration\nnotes: >-\n  Scopes advertised by the published OpenID Connect discovery document for the\n  moneyfellows.com member-authentication server (Umbraco Content Delivery API).\n  Only the standard OIDC scopes are declared; no product-specific scopes are\n  published.\nschemes:\n- name: oauth2\n  source: well-known/mfellows-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/authorize\n    tokenUrl: https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; request an ID token for the authenticated member.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mfellows-openid-configuration.json\n- scope: offline_access\n\
  \  description: Issue a refresh token so the client can obtain new access tokens without re-authentication.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/mfellows-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mfellows/refs/heads/main/scopes/mfellows-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Fintech
- Financial Services
- Savings
- Lending
- ROSCA
- Payments
- Egypt
- Mobile
- Consumer Finance
token_urls:
- https://moneyfellows.com/umbraco/delivery/api/v1/security/member/token
---
