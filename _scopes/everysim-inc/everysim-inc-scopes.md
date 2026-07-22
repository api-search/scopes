---
authorization_urls: []
description: ''
docs: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Everysim Inc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'EverySim Inc. publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the EverySim Inc. API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EverySim Inc.
provider_slug: everysim-inc
schemes:
- authorizationUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/auth
  name: openIdConnect
  source: well-known/everysim-inc-openid-configuration.json
  tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token
scope_count: 13
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- organization
- offline_access
- microprofile-jwt
- service_account
- web-origins
- acr
- basic
scopes:
- description: OpenID Connect authentication
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Email address claim
  flows: []
  scope: email
- description: Postal address claim
  flows: []
  scope: address
- description: Phone number claim
  flows: []
  scope: phone
- description: Realm and client role mappings
  flows: []
  scope: roles
- description: Organization membership claims
  flows: []
  scope: organization
- description: Refresh-token / offline access
  flows: []
  scope: offline_access
- description: MicroProfile JWT claims (groups, upn)
  flows: []
  scope: microprofile-jwt
- description: Service-account (client-credentials) scope
  flows: []
  scope: service_account
- description: Allowed CORS web origins
  flows: []
  scope: web-origins
- description: Authentication Context Class Reference
  flows: []
  scope: acr
- description: Basic realm claims
  flows: []
  scope: basic
slug: everysim-inc-scopes
source_filename: everysim-inc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration\ndocs: https://auth.everysim.io/realms/everysim/.well-known/openid-configuration\nnotes: >-\n  Scopes advertised by EverySim's OpenID Connect discovery document\n  (scopes_supported) for the \"everysim\" realm. Standard OIDC + Keycloak\n  realm scopes; no public OpenAPI declares per-operation scopes.\nschemes:\n- name: openIdConnect\n  source: well-known/everysim-inc-openid-configuration.json\n  authorizationUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/auth\n  tokenUrl: https://auth.everysim.io/realms/everysim/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\n- scope: profile\n  description: Basic profile claims\n- scope: email\n  description: Email address claim\n- scope: address\n  description: Postal address claim\n- scope: phone\n  description: Phone number claim\n- scope:\
  \ roles\n  description: Realm and client role mappings\n- scope: organization\n  description: Organization membership claims\n- scope: offline_access\n  description: Refresh-token / offline access\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (groups, upn)\n- scope: service_account\n  description: Service-account (client-credentials) scope\n- scope: web-origins\n  description: Allowed CORS web origins\n- scope: acr\n  description: Authentication Context Class Reference\n- scope: basic\n  description: Basic realm claims\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everysim-inc/refs/heads/main/scopes/everysim-inc-scopes.yml
summary_line: 13 scopes
tags:
- Company
- Authentication
- OpenID Connect
- OAuth 2.0
- Single Sign-On
- Identity
token_urls: []
---
