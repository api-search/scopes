---
authorization_urls:
- https://auth.eu.cynomi.com/authorize
description: ''
docs: https://cynomi.com/platform/integrations/public-api/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cynomi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cynomi publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cynomi API on a user''s behalf.


  Tokens are issued from https://auth.eu.cynomi.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cynomi
provider_slug: cynomi
schemes:
- flows:
  - authorizationUrl: https://auth.eu.cynomi.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.eu.cynomi.com/oauth/token
  name: Auth0OIDC
  source: well-known/cynomi-openid-configuration.json
scope_count: 11
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: User's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: User's given name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: User's family name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: User's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: User's profile picture claim.
  flows:
  - authorizationCode
  scope: picture
- description: User's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: User's address claim.
  flows:
  - authorizationCode
  scope: address
slug: cynomi-scopes
source_filename: cynomi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.eu.cynomi.com/.well-known/openid-configuration\ndocs: https://cynomi.com/platform/integrations/public-api/\nnotes: >-\n  These are the OpenID Connect standard scopes advertised by Cynomi's Auth0\n  tenant (scopes_supported in the discovery document). They govern identity /\n  profile claims on the login flow. Cynomi's Public API authorizes calls with a\n  JWT access token bound to the audience https://api.prod-eu.eu.cynomi.com/;\n  per-resource API permission scopes are not published on the public discovery\n  surface (the Public API reference is gated behind login), so only the\n  OIDC identity scopes are captured here.\nschemes:\n- name: Auth0OIDC\n  source: well-known/cynomi-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eu.cynomi.com/authorize\n    tokenUrl: https://auth.eu.cynomi.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication;\
  \ issue an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email and email_verified claims.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n- scope: name\n  description: User's full name claim.\n  flows: [authorizationCode]\n- scope: given_name\n  description: User's given name claim.\n  flows: [authorizationCode]\n- scope: family_name\n  description: User's family name claim.\n  flows: [authorizationCode]\n- scope: nickname\n  description: User's nickname claim.\n  flows: [authorizationCode]\n- scope: picture\n  description: User's profile picture claim.\n  flows: [authorizationCode]\n- scope: phone\n  description: User's phone number claim.\n  flows: [authorizationCode]\n- scope: address\n  description: User's address claim.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cynomi/refs/heads/main/scopes/cynomi-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Company
- Cybersecurity
- Security
- Compliance
- vCISO
- Risk Management
- GRC
- MSP
- MSSP
- Vulnerability Management
token_urls:
- https://auth.eu.cynomi.com/oauth/token
---
