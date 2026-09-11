---
api_specs:
- filename: aedifion-openapi.yml
  format: yaml
  label: aedifion HTTP API
  slug: aedifion-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/openapi/aedifion-openapi.yml
- filename: aedifion-mqtt-asyncapi.yml
  format: yaml
  label: aedifion MQTT API
  slug: aedifion-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/asyncapi/aedifion-mqtt-asyncapi.yml
authorization_urls:
- https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth
description: ''
docs: https://docs.aedifion.io/en/developers/http-api/guides-and-tutorials/authentication/
flows:
- implicit
- authorizationCode
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Aedifion Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares a single openIDConnect scheme exposing only the mandatory `openid` scope. The authoritative scope list is the one advertised by the aedifion Keycloak realm's own OIDC discovery document, fetched live and saved to well-known/aedifion-openid-configuration.json. These are Keycloak's standard realm scopes plus an `api` scope; aedifion publishes no per-resource scope reference page, and fine-grained authorization on the HTTP API is enforced by role-based access control on projects and datapoints rather than by OAuth scopes.
overview: 'Aedifion publishes 13 OAuth 2.0 scopes via the implicit, authorizationCode, password, and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aedifion API on a user''s behalf.


  Tokens are issued from https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aedifion
provider_slug: aedifion
schemes:
- flows:
  - authorizationUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth
    flow: implicit
  - authorizationUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token
  - flow: password
    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token
  issuer: https://auth.aedifion.io/realms/aedifion
  name: openIDConnect
  source: openapi/aedifion-openapi.yml
scope_count: 13
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- api
- offline_access
- service_account
- basic
- acr
- microprofile-jwt
- web-origins
scopes:
- description: Use OpenID Connect (required). The only scope the OpenAPI itself declares.
  flows:
  - implicit
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, preferred_username, locale).
  flows: []
  scope: profile
- description: Email address and verification status.
  flows: []
  scope: email
- description: Address claim.
  flows: []
  scope: address
- description: Phone number claim.
  flows: []
  scope: phone
- description: Realm and client role mappings, which carry the platform's RBAC assignments.
  flows: []
  scope: roles
- description: Access to the aedifion HTTP API as a resource.
  flows: []
  scope: api
- description: Issue a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Client-credentials service account access.
  flows: []
  scope: service_account
- description: Keycloak basic scope (sub, auth_time claims).
  flows: []
  scope: basic
- description: Authentication context class reference claim.
  flows: []
  scope: acr
- description: MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
- description: CORS allowed origins claim.
  flows: []
  scope: web-origins
slug: aedifion-scopes
source_filename: aedifion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: https://auth.aedifion.io/realms/aedifion/.well-known/openid-configuration\ndocs: https://docs.aedifion.io/en/developers/http-api/guides-and-tutorials/authentication/\nnote: >-\n  The OpenAPI declares a single openIDConnect scheme exposing only the mandatory `openid`\n  scope. The authoritative scope list is the one advertised by the aedifion Keycloak realm's\n  own OIDC discovery document, fetched live and saved to\n  well-known/aedifion-openid-configuration.json. These are Keycloak's standard realm scopes\n  plus an `api` scope; aedifion publishes no per-resource scope reference page, and\n  fine-grained authorization on the HTTP API is enforced by role-based access control on\n  projects and datapoints rather than by OAuth scopes.\nschemes:\n- name: openIDConnect\n  source: openapi/aedifion-openapi.yml\n  issuer: https://auth.aedifion.io/realms/aedifion\n  flows:\n  - flow: implicit\n    authorizationUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth\n    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token\n  - flow: password\n    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: Use OpenID Connect (required). The only scope the OpenAPI itself declares.\n  flows: [implicit, authorizationCode]\n  sources: [openapi/aedifion-openapi.yml, well-known/aedifion-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims (name, preferred_username, locale).\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: email\n  description: Email address and verification status.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: address\n  description: Address\
  \ claim.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: phone\n  description: Phone number claim.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: roles\n  description: Realm and client role mappings, which carry the platform's RBAC assignments.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: api\n  description: Access to the aedifion HTTP API as a resource.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token usable while the user is offline.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: service_account\n  description: Client-credentials service account access.\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: basic\n  description: Keycloak basic scope (sub, auth_time claims).\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: acr\n  description: Authentication context class reference claim.\n\
  \  sources: [well-known/aedifion-openid-configuration.json]\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (upn, groups).\n  sources: [well-known/aedifion-openid-configuration.json]\n- scope: web-origins\n  description: CORS allowed origins claim.\n  sources: [well-known/aedifion-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/scopes/aedifion-scopes.yml
summary_line: 13 scopes · implicit/authorizationCode/password/clientCredentials
tags:
- Building Automation
- Smart Buildings
- Energy Management
- Internet of Things
- Real Estate
- HVAC
- Sustainability
- Time Series
- Analytics
- MQTT
- Building Operations
- ESG
- PropTech
- Germany
token_urls:
- https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token
---
