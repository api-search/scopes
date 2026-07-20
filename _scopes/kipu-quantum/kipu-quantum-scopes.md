---
authorization_urls:
- https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/auth
description: ''
docs: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Kipu Quantum Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kipu Quantum publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kipu Quantum API on a user''s behalf.


  Tokens are issued from https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kipu Quantum
provider_slug: kipu-quantum
schemes:
- flows:
  - authorizationUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token
  name: oidc
  source: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration
scope_count: 12
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- service_account
- microprofile-jwt
- web-origins
- acr
- basic
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
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
- description: Realm and client role claims for the user.
  flows: []
  scope: roles
- description: Issue a refresh token for long-lived / offline access.
  flows: []
  scope: offline_access
- description: Service-account (client_credentials) machine-to-machine access.
  flows: []
  scope: service_account
- description: MicroProfile JWT claims (groups, upn) for service authorization.
  flows: []
  scope: microprofile-jwt
- description: Allowed CORS web origins for the client.
  flows: []
  scope: web-origins
- description: Authentication Context Class Reference claim.
  flows: []
  scope: acr
- description: Basic OIDC claims scope.
  flows: []
  scope: basic
slug: kipu-quantum-scopes
source_filename: kipu-quantum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\ndocs: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\nnotes: >-\n  OAuth2/OIDC scopes advertised by the Kipu Quantum Hub Keycloak provider\n  (PlanQK realm) discovery document. These are the standard OIDC + Keycloak\n  client scopes; the Hub does not yet publish API-permission scopes (v1 SDK\n  docs pending). Captured from scopes_supported verbatim.\nschemes:\n- name: oidc\n  source: https://login.hub.kipu-quantum.com/realms/planqk/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/auth\n    tokenUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n- scope: profile\n  description: Access to the user's basic profile claims.\n- scope: email\n  description: Access to the user's email address claim.\n- scope: address\n  description: Access to the user's address claim.\n- scope: phone\n  description: Access to the user's phone number claim.\n- scope: roles\n  description: Realm and client role claims for the user.\n- scope: offline_access\n  description: Issue a refresh token for long-lived / offline access.\n- scope: service_account\n  description: Service-account (client_credentials) machine-to-machine access.\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (groups, upn) for service authorization.\n- scope: web-origins\n  description: Allowed CORS web origins for the client.\n- scope: acr\n  description: Authentication Context Class Reference claim.\n- scope: basic\n  description: Basic OIDC claims scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kipu-quantum/refs/heads/main/scopes/kipu-quantum-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Company
- Deep Tech
- Quantum Computing
- Quantum
- Artificial Intelligence
- Optimization
- Developer Platform
- SDK
- REST API
- Germany
token_urls:
- https://login.hub.kipu-quantum.com/realms/planqk/protocol/openid-connect/token
---
