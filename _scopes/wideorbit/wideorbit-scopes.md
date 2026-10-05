---
authorization_urls: []
description: ''
docs: https://www.wideorbit.com/io/
flows:
- authorization_code
kind: oauth-scopes
layout: scope
method: searched
name: Wideorbit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WideOrbit publishes 10 OAuth 2.0 scopes via the authorization_code flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the WideOrbit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WideOrbit
provider_slug: wideorbit
schemes: []
scope_count: 10
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- microprofile-jwt
- acr
- web-origins
scopes:
- description: Enables OpenID Connect; required to obtain an ID token. This is the scope the gateway client requests by default.
  flows: []
  scope: openid
- description: Access to the end user's basic profile claims (name, preferred_username, etc.).
  flows: []
  scope: profile
- description: Access to the user's email address and email_verified claim.
  flows: []
  scope: email
- description: Access to the user's postal address claim.
  flows: []
  scope: address
- description: Access to the user's phone number claims.
  flows: []
  scope: phone
- description: Includes realm and client role mappings in the token for authorization decisions.
  flows: []
  scope: roles
- description: Grants a refresh token for long-lived, offline machine-to-machine access.
  flows: []
  scope: offline_access
- description: Emits MicroProfile-JWT compatible claims (groups, upn) for service authorization.
  flows: []
  scope: microprofile-jwt
- description: Authentication Context Class Reference; conveys the level/assurance of authentication.
  flows: []
  scope: acr
- description: Controls allowed CORS web origins for browser-based clients.
  flows: []
  scope: web-origins
slug: wideorbit-scopes
source_filename: wideorbit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  scopes_supported from the WO Central Keycloak \"externalgateway\" realm OIDC\n  discovery document\n  (https://sso.wocentral.com/auth/realms/externalgateway/.well-known/openid-configuration)\ndocs: https://www.wideorbit.com/io/\nsummary: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by the WO Central identity\n  provider realm that guards the WideOrbit.io API gateway. These are the\n  identity-provider (Keycloak) realm scopes; fine-grained business\n  authorizations for Traffic/Network/Omni objects are provisioned per\n  certified-partner client and documented inside the authenticated developer\n  portal rather than published publicly.\nflow: authorization_code\nscopes:\n- name: openid\n  description: Enables OpenID Connect; required to obtain an ID token. This is the scope the gateway client requests by default.\n- name: profile\n  description: Access to the end user's basic profile claims (name, preferred_username,\
  \ etc.).\n- name: email\n  description: Access to the user's email address and email_verified claim.\n- name: address\n  description: Access to the user's postal address claim.\n- name: phone\n  description: Access to the user's phone number claims.\n- name: roles\n  description: Includes realm and client role mappings in the token for authorization decisions.\n- name: offline_access\n  description: Grants a refresh token for long-lived, offline machine-to-machine access.\n- name: microprofile-jwt\n  description: Emits MicroProfile-JWT compatible claims (groups, upn) for service authorization.\n- name: acr\n  description: Authentication Context Class Reference; conveys the level/assurance of authentication.\n- name: web-origins\n  description: Controls allowed CORS web origins for browser-based clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wideorbit/refs/heads/main/scopes/wideorbit-scopes.yml
summary_line: 10 scopes · authorization_code
tags:
- Company
- Advertising
- AdTech
- Media
- Broadcasting
- Radio
- Television
- Ad Management
- Programmatic
- Media Sales
token_bound: false
token_urls: []
---
