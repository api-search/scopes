---
authorization_urls: []
description: ''
docs: https://docs.caliza.com/docs/authenticate
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Caliza Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Caliza publishes 10 OAuth 2.0 scopes via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Caliza API on a user''s behalf.


  Tokens are issued from https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Caliza
provider_slug: caliza
schemes:
- flows:
  - flow: password
    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
  name: OAuth2 (Keycloak realm "caliza")
  source: well-known/caliza-openid-configuration.json
scope_count: 10
scope_names:
- openid
- email
- profile
- offline_access
- roles
- address
- phone
- web-origins
- microprofile-jwt
- acr
scopes:
- description: OpenID Connect authentication; issues an ID token identifying the integrator.
  flows:
  - password
  - authorizationCode
  scope: openid
- description: Access to the integrator's email claim.
  flows:
  - password
  - authorizationCode
  scope: email
- description: Access to the integrator's profile claims (name, preferred_username).
  flows:
  - password
  - authorizationCode
  scope: profile
- description: Issues a refresh token for long-lived offline access.
  flows:
  - password
  - authorizationCode
  scope: offline_access
- description: Includes realm/client role mappings in the token.
  flows:
  - password
  - authorizationCode
  scope: roles
- description: Access to address claims.
  flows:
  - authorizationCode
  scope: address
- description: Access to phone-number claims.
  flows:
  - authorizationCode
  scope: phone
- description: Populates allowed CORS web origins.
  flows:
  - authorizationCode
  scope: web-origins
- description: MicroProfile JWT claims mapping.
  flows:
  - authorizationCode
  scope: microprofile-jwt
- description: Authentication Context Class Reference claim.
  flows:
  - authorizationCode
  scope: acr
slug: caliza-scopes
source_filename: caliza-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.caliza.com/auth/realms/caliza/.well-known/openid-configuration\ndocs: https://docs.caliza.com/docs/authenticate\nschemes:\n- name: OAuth2 (Keycloak realm \"caliza\")\n  source: well-known/caliza-openid-configuration.json\n  flows:\n  - flow: password\n    tokenUrl: https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token identifying the integrator.\n  flows: [password, authorizationCode]\n- scope: email\n  description: Access to the integrator's email claim.\n  flows: [password, authorizationCode]\n- scope: profile\n  description: Access to the integrator's profile claims (name, preferred_username).\n  flows: [password, authorizationCode]\n- scope: offline_access\n  description: Issues a refresh token for long-lived offline access.\n  flows: [password, authorizationCode]\n- scope: roles\n  description: Includes\
  \ realm/client role mappings in the token.\n  flows: [password, authorizationCode]\n- scope: address\n  description: Access to address claims.\n  flows: [authorizationCode]\n- scope: phone\n  description: Access to phone-number claims.\n  flows: [authorizationCode]\n- scope: web-origins\n  description: Populates allowed CORS web origins.\n  flows: [authorizationCode]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims mapping.\n  flows: [authorizationCode]\n- scope: acr\n  description: Authentication Context Class Reference claim.\n  flows: [authorizationCode]\nnotes: >-\n  Scopes are the standard Keycloak/OIDC scope set advertised by the realm\n  discovery document; the documented quickstart token response returns\n  \"scope\": \"email openid profile\". API-level authorization is enforced through\n  realm roles (e.g. ROLE_CREATE_TRANSACTIONS, ROLE_VIEW_ACTIVITY,\n  ROLE_MANAGE_PAYMENT_CONTACTS) carried inside the access-token JWT rather than\n  through granular OAuth resource\
  \ scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/scopes/caliza-scopes.yml
summary_line: 10 scopes · password
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Stablecoins
- Remittances
- Foreign Exchange
- Virtual Accounts
- Payouts
- KYC
- Latin America
token_urls:
- https://api.caliza.com/auth/realms/caliza/protocol/openid-connect/token
---
