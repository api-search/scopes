---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Zspace Scopes
name_suffix: OAuth Scopes
note: scopes_supported read verbatim from the production Keycloak OIDC discovery document. These are the Keycloak realm default client scopes; zSpace publishes no scope or permission reference page, so no application-specific scopes (device, content, roster, licensing) could be found. Descriptions below are the standard OIDC/Keycloak meanings of each scope, not zSpace prose.
overview: 'zSpace publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the zSpace API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: zSpace
provider_slug: zspace
schemes: []
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- web-origins
- microprofile-jwt
scopes:
- description: Required for OpenID Connect; requests an ID token.
  flows: []
  scope: openid
- description: Basic profile claims (name, given_name, family_name, preferred_username).
  flows: []
  scope: profile
- description: The email and email_verified claims.
  flows: []
  scope: email
- description: The address claim.
  flows: []
  scope: address
- description: The phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Requests a refresh token usable while the user is not present.
  flows: []
  scope: offline_access
- description: Keycloak realm and client role mappings in the token.
  flows: []
  scope: roles
- description: Keycloak scope that populates allowed CORS origins in the token.
  flows: []
  scope: web-origins
- description: MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
slug: zspace-scopes
source_filename: zspace-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://auth.zspace.com/auth/realms/master/.well-known/openid-configuration\ndocs: null\nnote: >-\n  scopes_supported read verbatim from the production Keycloak OIDC discovery document.\n  These are the Keycloak realm default client scopes; zSpace publishes no scope or\n  permission reference page, so no application-specific scopes (device, content, roster,\n  licensing) could be found. Descriptions below are the standard OIDC/Keycloak meanings of\n  each scope, not zSpace prose.\nissuer: https://auth.zspace.com/auth/realms/master\nscope_count: 9\nscopes:\n- name: openid\n  description: Required for OpenID Connect; requests an ID token.\n  standard: OpenID Connect Core 1.0\n- name: profile\n  description: Basic profile claims (name, given_name, family_name, preferred_username).\n  standard: OpenID Connect Core 1.0\n- name: email\n  description: The email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n- name:\
  \ address\n  description: The address claim.\n  standard: OpenID Connect Core 1.0\n- name: phone\n  description: The phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0\n- name: offline_access\n  description: Requests a refresh token usable while the user is not present.\n  standard: OpenID Connect Core 1.0\n- name: roles\n  description: Keycloak realm and client role mappings in the token.\n  standard: Keycloak default client scope\n- name: web-origins\n  description: Keycloak scope that populates allowed CORS origins in the token.\n  standard: Keycloak default client scope\n- name: microprofile-jwt\n  description: MicroProfile JWT claims (upn, groups).\n  standard: Eclipse MicroProfile JWT RBAC\ngaps:\n- >-\n  No published scope reference. Every scope here is a Keycloak/OIDC default — zSpace has\n  not defined an application permission model that an integrator could request against.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zspace/refs/heads/main/scopes/zspace-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Education
- Augmented Reality
- Virtual Reality
- EdTech
- Hardware
- 3D
- Simulation
- Career and Technical Education
- Developer SDK
token_bound: false
token_urls: []
---
