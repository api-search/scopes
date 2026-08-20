---
api_specs:
- filename: passivelogic-account-api-openapi.yml
  format: yaml
  label: PassiveLogic Account API
  slug: passivelogic-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-account-api-openapi.yml
- filename: passivelogic-api-api-openapi.yml
  format: yaml
  label: PassiveLogic API
  slug: passivelogic-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-api-api-openapi.yml
- filename: passivelogic-app-api-openapi.yml
  format: yaml
  label: PassiveLogic App API
  slug: passivelogic-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-app-api-openapi.yml
- filename: passivelogic-auth-groups-api-openapi.yml
  format: yaml
  label: PassiveLogic Auth Groups API
  slug: passivelogic-auth-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-auth-groups-api-openapi.yml
- filename: passivelogic-authentication-api-openapi.yml
  format: yaml
  label: PassiveLogic Authentication API
  slug: passivelogic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-authentication-api-openapi.yml
- filename: passivelogic-bindings-api-openapi.yml
  format: yaml
  label: PassiveLogic Bindings API
  slug: passivelogic-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-bindings-api-openapi.yml
- filename: passivelogic-default-api-openapi.yml
  format: yaml
  label: PassiveLogic Default API
  slug: passivelogic-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-default-api-openapi.yml
- filename: passivelogic-export-api-openapi.yml
  format: yaml
  label: PassiveLogic Export API
  slug: passivelogic-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-export-api-openapi.yml
- filename: passivelogic-graphql-api-openapi.yml
  format: yaml
  label: PassiveLogic Graph QL API
  slug: passivelogic-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-graphql-api-openapi.yml
- filename: passivelogic-health-api-openapi.yml
  format: yaml
  label: PassiveLogic Health API
  slug: passivelogic-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-health-api-openapi.yml
- filename: passivelogic-images-api-openapi.yml
  format: yaml
  label: PassiveLogic Images API
  slug: passivelogic-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-images-api-openapi.yml
- filename: passivelogic-organization-api-openapi.yml
  format: yaml
  label: PassiveLogic Organization API
  slug: passivelogic-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-organization-api-openapi.yml
- filename: passivelogic-passivelogic-device-api-openapi.yml
  format: yaml
  label: PassiveLogic PassiveLogic Device API
  slug: passivelogic-passivelogic-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-passivelogic-device-api-openapi.yml
- filename: passivelogic-quantum-sync-api-openapi.yml
  format: yaml
  label: PassiveLogic Quantum Sync API
  slug: passivelogic-quantum-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-quantum-sync-api-openapi.yml
- filename: passivelogic-site-api-openapi.yml
  format: yaml
  label: PassiveLogic Site API
  slug: passivelogic-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-site-api-openapi.yml
- filename: passivelogic-tunnel-api-openapi.yml
  format: yaml
  label: PassiveLogic Tunnel API
  slug: passivelogic-tunnel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-tunnel-api-openapi.yml
- filename: passivelogic-utility-api-openapi.yml
  format: yaml
  label: PassiveLogic Utility API
  slug: passivelogic-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/openapi/passivelogic-utility-api-openapi.yml
authorization_urls:
- https://login.passivelogic.com/realms/prod/protocol/openid-connect/auth
description: ''
docs: https://quantumalliance.org/documentation/
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Passivelogic Scopes
name_suffix: OAuth Scopes
note: The PassiveLogic OpenAPI declares no oauth2 securityScheme — the REST API is protected by JWT/API-key headers. The OAuth 2.0 / OpenID Connect surface lives one layer down, on the external Keycloak identity provider that the app redirects to (GET /app/login and GET /api/util/externalauthconfig both point at it). The scopes below are the realm's advertised scopes_supported, read from the anonymous discovery document — they are Keycloak defaults plus the realm-specific "service_account" and "organization" scopes, not a published PassiveLogic permission model. PassiveLogic publishes no per-resource scope reference; API keys "act with the same permissions as a JWT for the user who generated them" (Quantum documentation), so authorization is role-based, not scope-based.
overview: 'PassiveLogic publishes 13 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PassiveLogic API on a user''s behalf.


  Tokens are issued from https://login.passivelogic.com/realms/prod/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PassiveLogic
provider_slug: passivelogic
schemes:
- flows:
  - authorizationUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/auth/device
    flow: deviceCode
    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token
  name: Keycloak OpenID Connect (realm "prod")
  pkce:
  - plain
  - S256
  source: well-known/passivelogic-openid-configuration.json
scope_count: 13
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- organization
- service_account
- microprofile-jwt
- basic
- acr
- web-origins
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, preferred_username).
  flows:
  - authorizationCode
  scope: profile
- description: Email address and email_verified claim.
  flows:
  - authorizationCode
  scope: email
- description: Address claim.
  flows:
  - authorizationCode
  scope: address
- description: Phone number claims.
  flows:
  - authorizationCode
  scope: phone
- description: Realm and client role claims used for PassiveLogic authorization decisions.
  flows:
  - authorizationCode
  scope: roles
- description: Issues an offline refresh token for long-lived, unattended access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Organization membership claim — maps to the PassiveLogic organization/auth-group model.
  flows:
  - authorizationCode
  scope: organization
- description: Service-account claims for client-credentials (machine) clients.
  flows:
  - clientCredentials
  scope: service_account
- description: MicroProfile JWT claims (upn, groups).
  flows:
  - authorizationCode
  scope: microprofile-jwt
- description: Keycloak "basic" scope — sub, auth_time claims.
  flows:
  - authorizationCode
  scope: basic
- description: Authentication Context Class Reference claim.
  flows:
  - authorizationCode
  scope: acr
- description: CORS allowed-origins claim used by browser clients.
  flows:
  - authorizationCode
  scope: web-origins
slug: passivelogic-scopes
source_filename: passivelogic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://login.passivelogic.com/realms/prod/.well-known/openid-configuration\ndocs: https://quantumalliance.org/documentation/\nnote: >-\n  The PassiveLogic OpenAPI declares no oauth2 securityScheme — the REST API is protected by JWT/API-key headers. The\n  OAuth 2.0 / OpenID Connect surface lives one layer down, on the external Keycloak identity provider that the app\n  redirects to (GET /app/login and GET /api/util/externalauthconfig both point at it). The scopes below are the\n  realm's advertised scopes_supported, read from the anonymous discovery document — they are Keycloak defaults plus\n  the realm-specific \"service_account\" and \"organization\" scopes, not a published PassiveLogic permission model.\n  PassiveLogic publishes no per-resource scope reference; API keys \"act with the same permissions as a JWT for the\n  user who generated them\" (Quantum documentation), so authorization is role-based, not scope-based.\n\
  issuer: https://login.passivelogic.com/realms/prod\nschemes:\n- name: Keycloak OpenID Connect (realm \"prod\")\n  source: well-known/passivelogic-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/auth\n    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/auth/device\n    tokenUrl: https://login.passivelogic.com/realms/prod/protocol/openid-connect/token\n  pkce: [plain, S256]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows: [authorizationCode]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, preferred_username).\n  flows: [authorizationCode]\n\
  - scope: email\n  description: Email address and email_verified claim.\n  flows: [authorizationCode]\n- scope: address\n  description: Address claim.\n  flows: [authorizationCode]\n- scope: phone\n  description: Phone number claims.\n  flows: [authorizationCode]\n- scope: roles\n  description: Realm and client role claims used for PassiveLogic authorization decisions.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issues an offline refresh token for long-lived, unattended access.\n  flows: [authorizationCode]\n- scope: organization\n  description: Organization membership claim — maps to the PassiveLogic organization/auth-group model.\n  flows: [authorizationCode]\n- scope: service_account\n  description: Service-account claims for client-credentials (machine) clients.\n  flows: [clientCredentials]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (upn, groups).\n  flows: [authorizationCode]\n- scope: basic\n  description: Keycloak \"basic\" scope\
  \ — sub, auth_time claims.\n  flows: [authorizationCode]\n- scope: acr\n  description: Authentication Context Class Reference claim.\n  flows: [authorizationCode]\n- scope: web-origins\n  description: CORS allowed-origins claim used by browser clients.\n  flows: [authorizationCode]\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://login.passivelogic.com/realms/prod/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passivelogic/refs/heads/main/scopes/passivelogic-scopes.yml
summary_line: 13 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Digital Twin
- Building Automation
- HVAC
- Smart Buildings
- Autonomous Systems
- GraphQL
- Ontology
- IoT
- Edge Computing
- Physical AI
- Energy
token_urls:
- https://login.passivelogic.com/realms/prod/protocol/openid-connect/token
---
