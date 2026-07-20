---
authorization_urls:
- https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/auth
description: ''
docs: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Joor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Joor publishes 9 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Joor API on a user''s behalf.


  Tokens are issued from https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Joor
provider_slug: joor
schemes:
- flows:
  - authorizationUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token
  issuer: https://auth.jooraccess.com/auth/realms/joor
  name: openIdConnect
  source: well-known/joor-openid-configuration.json
scope_count: 9
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- web-origins
- microprofile-jwt
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to basic profile claims (name, preferred_username, etc.).
  flows: []
  scope: profile
- description: Access to the user's email address claim.
  flows: []
  scope: email
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Access to the user's phone number claim.
  flows: []
  scope: phone
- description: Realm and client role claims for the authenticated principal.
  flows: []
  scope: roles
- description: Issue a refresh token for offline / long-lived access.
  flows: []
  scope: offline_access
- description: CORS web-origin allow-list claim for browser clients.
  flows: []
  scope: web-origins
- description: MicroProfile JWT claims (groups, upn) for service authorization.
  flows: []
  scope: microprofile-jwt
slug: joor-scopes
source_filename: joor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration\ndocs: https://auth.jooraccess.com/auth/realms/joor/.well-known/openid-configuration\nschemes:\n- name: openIdConnect\n  source: well-known/joor-openid-configuration.json\n  issuer: https://auth.jooraccess.com/auth/realms/joor\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/auth\n    tokenUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: profile\n  description: Access to basic profile claims (name, preferred_username, etc.).\n  sources: [well-known/joor-openid-configuration.json]\n\
  - scope: email\n  description: Access to the user's email address claim.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: address\n  description: Access to the user's address claim.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: phone\n  description: Access to the user's phone number claim.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: roles\n  description: Realm and client role claims for the authenticated principal.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for offline / long-lived access.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: web-origins\n  description: CORS web-origin allow-list claim for browser clients.\n  sources: [well-known/joor-openid-configuration.json]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (groups, upn) for service authorization.\n  sources: [well-known/joor-openid-configuration.json]\n\
  notes: >-\n  These are the scopes advertised by JOOR's Keycloak realm discovery document\n  (scopes_supported). They are the standard Keycloak/OIDC scope set; JOOR does\n  not publish an application-level scope reference on a public developer portal.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joor/refs/heads/main/scopes/joor-scopes.yml
summary_line: 9 scopes · authorizationCode/clientCredentials
tags:
- Company
- Fashion
- Wholesale
- Retail
- eCommerce
- B2B
- Marketplace
- Payments
token_urls:
- https://auth.jooraccess.com/auth/realms/joor/protocol/openid-connect/token
---
