---
authorization_urls:
- https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
- password
kind: oauth-scopes
layout: scope
method: probed
name: Countertack Scopes
name_suffix: OAuth Scopes
note: Scopes read verbatim from the scopes_supported array of the GoSecure Titan Keycloak realm discovery document. GoSecure publishes no scope/permission reference page that could be found, so the descriptions below only distinguish the standard OpenID Connect / Keycloak built-in scopes from the two realm-specific scopes (titan, service_account); the actual permissions those two grant are not publicly documented and have NOT been guessed.
overview: 'CounterTack publishes 13 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, implicit, and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CounterTack API on a user''s behalf.


  Tokens are issued from https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CounterTack
provider_slug: countertack
schemes:
- flows:
  - authorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth/device
    flow: deviceCode
  - authorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth
    flow: implicit
  - flow: password
    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token
  name: gosec-titan
  source: well-known/countertack-gosec-titan-openid-configuration.json
scope_count: 13
scope_names:
- titan
- service_account
- openid
- profile
- email
- address
- phone
- offline_access
- acr
- roles
- web-origins
- basic
- microprofile-jwt
scopes:
- description: Realm-specific scope for the GoSecure Titan platform. Its granted permissions are not publicly documented.
  flows: []
  scope: titan
- description: Realm-specific scope, presumed to accompany client-credentials service accounts. Its granted permissions are not publicly documented.
  flows: []
  scope: service_account
- description: OpenID Connect core scope; requests an ID token.
  flows: []
  scope: openid
- description: OpenID Connect standard scope for basic profile claims.
  flows: []
  scope: profile
- description: OpenID Connect standard scope for the email and email_verified claims.
  flows: []
  scope: email
- description: OpenID Connect standard scope for the address claim.
  flows: []
  scope: address
- description: OpenID Connect standard scope for phone_number claims.
  flows: []
  scope: phone
- description: OpenID Connect standard scope requesting a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Keycloak built-in client scope carrying the authentication context class reference.
  flows: []
  scope: acr
- description: Keycloak built-in client scope adding realm and client role mappings to the token.
  flows: []
  scope: roles
- description: Keycloak built-in client scope adding allowed CORS origins to the token.
  flows: []
  scope: web-origins
- description: Keycloak built-in client scope adding the core sub/auth_time claims.
  flows: []
  scope: basic
- description: Keycloak built-in client scope emitting MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
slug: countertack-scopes
source_filename: countertack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration\ndocs: null\nnote: 'Scopes read verbatim from the scopes_supported array of the GoSecure Titan\n  Keycloak realm discovery document. GoSecure publishes no scope/permission reference\n  page that could be found, so the descriptions below only distinguish the standard\n  OpenID Connect / Keycloak built-in scopes from the two realm-specific scopes\n  (titan, service_account); the actual permissions those two grant are not publicly\n  documented and have NOT been guessed.'\nschemes:\n- name: gosec-titan\n  source: well-known/countertack-gosec-titan-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth\n    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth/device\n  - flow: implicit\n    authorizationUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/auth\n  - flow: password\n    tokenUrl: https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token\nscopes:\n- scope: titan\n  description: Realm-specific scope for the GoSecure Titan platform. Its granted\n    permissions are not publicly documented.\n  standard: false\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: service_account\n  description: Realm-specific scope, presumed to accompany client-credentials service\n    accounts. Its granted permissions are not publicly documented.\n  standard: false\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: openid\n  description: OpenID Connect core scope; requests an ID token.\n  standard: true\n  sources:\n\
  \  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: profile\n  description: OpenID Connect standard scope for basic profile claims.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: email\n  description: OpenID Connect standard scope for the email and email_verified claims.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: address\n  description: OpenID Connect standard scope for the address claim.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: phone\n  description: OpenID Connect standard scope for phone_number claims.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: offline_access\n  description: OpenID Connect standard scope requesting a refresh token usable while\n    the user is offline.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n\
  - scope: acr\n  description: Keycloak built-in client scope carrying the authentication context\n    class reference.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: roles\n  description: Keycloak built-in client scope adding realm and client role mappings\n    to the token.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: web-origins\n  description: Keycloak built-in client scope adding allowed CORS origins to the token.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: basic\n  description: Keycloak built-in client scope adding the core sub/auth_time claims.\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n- scope: microprofile-jwt\n  description: Keycloak built-in client scope emitting MicroProfile JWT claims (upn,\n    groups).\n  standard: true\n  sources:\n  - well-known/countertack-gosec-titan-openid-configuration.json\n\
  summary:\n  scope_count: 13\n  realm_specific: 2\n  standard: 11\nx-evidence:\n  fetched: '2026-08-11'\n  url: https://login.gosecure.net/realms/gosec-titan/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/countertack/refs/heads/main/scopes/countertack-scopes.yml
summary_line: 13 scopes · authorizationCode/clientCredentials/deviceCode/implicit/password
tags:
- Company
- Security
- Cybersecurity
- Endpoint Security
- Endpoint Detection and Response
- Managed Detection and Response
- Threat Detection
- Incident Response
- SIEM
token_urls:
- https://login.gosecure.net/realms/gosec-titan/protocol/openid-connect/token
---
