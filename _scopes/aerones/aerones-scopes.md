---
api_specs:
- filename: aerones-operations-hub-openapi.json
  format: json
  label: Aerones Operations Hub API
  slug: aerones-operations-hub
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/openapi/aerones-operations-hub-openapi.json
authorization_urls:
- https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Aerones Scopes
name_suffix: OAuth Scopes
note: 'The Operations Hub OpenAPI declares no oauth2 securityScheme, so there is nothing to derive from the spec - derive-oauth-scopes.py reported zero oauth2 schemes. The scopes below are the scopes_supported list read verbatim off the Keycloak realm''s OIDC discovery document, which is served anonymously. They are Keycloak''s standard OIDC and built-in client scopes, not an Aerones-authored permission model: no per-resource scope (read:turbines and the like) is published anywhere. Field-level authorization on the GraphQL surface is expressed instead with a @hasPerm(permissions: [PermDefinition!]!) directive carried in the published SDL; the permission strings themselves are not enumerated in the schema.'
overview: 'Aerones publishes 12 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aerones API on a user''s behalf.


  Tokens are issued from https://sso.aerones.com/realms/aerones/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aerones
provider_slug: aerones
schemes:
- flows:
  - authorizationUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth/device
    flow: deviceCode
  name: KeycloakOIDC
  realm: aerones
  source: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration
scope_count: 12
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- acr
- basic
- web-origins
- organization
- microprofile-jwt
scopes:
- description: OIDC authentication request marker.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).
  flows: []
  scope: profile
- description: Standard OIDC email claim.
  flows: []
  scope: email
- description: Standard OIDC address claim.
  flows: []
  scope: address
- description: Standard OIDC phone claim.
  flows: []
  scope: phone
- description: Keycloak realm and client role mappings in the token.
  flows: []
  scope: roles
- description: Requests an offline refresh token.
  flows: []
  scope: offline_access
- description: Authentication context class reference.
  flows: []
  scope: acr
- description: Keycloak built-in scope carrying sub and auth_time.
  flows: []
  scope: basic
- description: Keycloak built-in scope adding allowed CORS origins to the token.
  flows: []
  scope: web-origins
- description: Keycloak organization membership claim.
  flows: []
  scope: organization
- description: Keycloak built-in MicroProfile JWT scope (upn, groups).
  flows: []
  scope: microprofile-jwt
slug: aerones-scopes
source_filename: aerones-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration\nnote: >-\n  The Operations Hub OpenAPI declares no oauth2 securityScheme, so there is nothing to\n  derive from the spec - derive-oauth-scopes.py reported zero oauth2 schemes. The scopes\n  below are the scopes_supported list read verbatim off the Keycloak realm's OIDC\n  discovery document, which is served anonymously. They are Keycloak's standard OIDC and\n  built-in client scopes, not an Aerones-authored permission model: no per-resource scope\n  (read:turbines and the like) is published anywhere. Field-level authorization on the\n  GraphQL surface is expressed instead with a @hasPerm(permissions: [PermDefinition!]!)\n  directive carried in the published SDL; the permission strings themselves are not\n  enumerated in the schema.\nschemes:\n- name: KeycloakOIDC\n  realm: aerones\n  source: https://sso.aerones.com/realms/aerones/.well-known/openid-configuration\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth\n    tokenUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://sso.aerones.com/realms/aerones/protocol/openid-connect/auth/device\nscopes:\n- scope: openid\n  description: OIDC authentication request marker.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: profile\n  description: Standard OIDC profile claims (name, given_name, family_name, preferred_username).\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: email\n  description: Standard OIDC email claim.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: address\n  description: Standard OIDC address claim.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n\
  - scope: phone\n  description: Standard OIDC phone claim.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: roles\n  description: Keycloak realm and client role mappings in the token.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: offline_access\n  description: Requests an offline refresh token.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: acr\n  description: Authentication context class reference.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: basic\n  description: Keycloak built-in scope carrying sub and auth_time.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: web-origins\n  description: Keycloak built-in scope adding allowed CORS origins to the token.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n- scope: organization\n  description: Keycloak organization membership claim.\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n\
  - scope: microprofile-jwt\n  description: Keycloak built-in MicroProfile JWT scope (upn, groups).\n  sources: [well-known/aerones-sso-aerones-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerones/refs/heads/main/scopes/aerones-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Wind Energy
- Renewable Energy
- Robotics
- Drones
- Inspection
- Field Service Management
- Asset Management
- Industrial
- Energy
- Maintenance
- Latvia
token_urls:
- https://sso.aerones.com/realms/aerones/protocol/openid-connect/token
---
