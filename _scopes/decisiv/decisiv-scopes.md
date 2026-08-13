---
api_specs:
- filename: decisiv-account-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Account Management
  slug: decisiv-srm-gateway-account-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-account-management-openapi.yml
- filename: decisiv-asset-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Asset Management
  slug: decisiv-srm-gateway-asset-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-asset-management-openapi.yml
- filename: decisiv-service-management-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Service Management
  slug: decisiv-srm-gateway-service-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-management-openapi.yml
- filename: decisiv-telematics-openapi.yml
  format: yaml
  label: Decisiv SRM Gateway - Telematics
  slug: decisiv-srm-gateway-telematics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-telematics-openapi.yml
- filename: decisiv-global-assets-openapi.yml
  format: yaml
  label: Decisiv Global Assets API
  slug: decisiv-global-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-global-assets-openapi.yml
- filename: decisiv-service-provider-openapi.yml
  format: yaml
  label: Decisiv Service Provider API
  slug: decisiv-service-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/openapi/decisiv-service-provider-openapi.yml
authorization_urls:
- https://login.decisiv.net/auth/api_gateway
description: ''
docs: https://api-docs.decisiv.net/docs/api/oauth/
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: probed
name: Decisiv Scopes
name_suffix: OAuth Scopes
note: Decisiv's OpenAPI security schemes declare oauth2 flows with EMPTY scope maps in all six specs, so the spec-derived pass produced zero scopes. The real scope list comes from the provider's own OAuth 2.0 / OIDC discovery document at login.decisiv.net, which publishes scopes_supported. Decisiv does not publish a per-resource scope reference page; authorization is granted per OAuth Application through account provisioning (a request to an unprovisioned module returns 428 with decisiv:access:003 "OAuth Application does not have appropriate provisioning to access this resource"), which means the coarse scopes below are the whole published scope vocabulary.
overview: 'Decisiv publishes 5 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Decisiv API on a user''s behalf.


  Tokens are issued from https://login.decisiv.net/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Decisiv
provider_slug: decisiv
schemes:
- flows:
  - authorizationUrl: https://login.decisiv.net/auth/api_gateway
    flow: authorizationCode
    refreshUrl: https://login.decisiv.net/oauth/token
    scopes_declared_in_spec: 0
    tokenUrl: https://login.decisiv.net/oauth/token
  name: OAuth2AuthorizationCode
  note: required flow for all new integrations
  source: openapi/decisiv-account-management-openapi.yml
  status: current
- flows:
  - flow: password
    scopes_declared_in_spec: 0
    tokenUrl: https://login.decisiv.net/oauth/token
  name: OAuth2Password
  note: Marked "**Deprecated.**" in the spec description — available only during the migration window to the authorization-code flow and slated for removal in a future release.
  source: openapi/decisiv-account-management-openapi.yml
  status: deprecated
- flows:
  - flow: password
    scopes_declared_in_spec: 0
    tokenUrl: https://portal.decisivapps.com/oauth/token
  name: OAuth2Password
  source: openapi/decisiv-global-assets-openapi.yml
  status: deprecated
scope_count: 5
scope_names:
- openid
- public
- read
- write
- update
scopes:
- description: Request an OpenID Connect ID token alongside the access token.
  flows: []
  scope: openid
- description: Public / unauthenticated-tier access.
  flows: []
  scope: public
- description: Read access to the resources the OAuth Application is provisioned for.
  flows: []
  scope: read
- description: Create access to the resources the OAuth Application is provisioned for.
  flows: []
  scope: write
- description: Modify access to the resources the OAuth Application is provisioned for.
  flows: []
  scope: update
slug: decisiv-scopes
source_filename: decisiv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://login.decisiv.net/.well-known/openid-configuration\ndocs: https://api-docs.decisiv.net/docs/api/oauth/\nnote: >-\n  Decisiv's OpenAPI security schemes declare oauth2 flows with EMPTY scope maps in all six specs, so the\n  spec-derived pass produced zero scopes. The real scope list comes from the provider's own OAuth 2.0 /\n  OIDC discovery document at login.decisiv.net, which publishes scopes_supported. Decisiv does not\n  publish a per-resource scope reference page; authorization is granted per OAuth Application through\n  account provisioning (a request to an unprovisioned module returns 428 with\n  decisiv:access:003 \"OAuth Application does not have appropriate provisioning to access this resource\"),\n  which means the coarse scopes below are the whole published scope vocabulary.\nissuer: decisiv.net\nauthorization_server: https://login.decisiv.net\nschemes:\n- name: OAuth2AuthorizationCode\n  source: openapi/decisiv-account-management-openapi.yml\n\
  \  status: current\n  note: required flow for all new integrations\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.decisiv.net/auth/api_gateway\n    tokenUrl: https://login.decisiv.net/oauth/token\n    refreshUrl: https://login.decisiv.net/oauth/token\n    scopes_declared_in_spec: 0\n- name: OAuth2Password\n  source: openapi/decisiv-account-management-openapi.yml\n  status: deprecated\n  note: >-\n    Marked \"**Deprecated.**\" in the spec description — available only during the migration window to\n    the authorization-code flow and slated for removal in a future release.\n  flows:\n  - flow: password\n    tokenUrl: https://login.decisiv.net/oauth/token\n    scopes_declared_in_spec: 0\n- name: OAuth2Password\n  source: openapi/decisiv-global-assets-openapi.yml\n  status: deprecated\n  flows:\n  - flow: password\n    tokenUrl: https://portal.decisivapps.com/oauth/token\n    scopes_declared_in_spec: 0\nscopes:\n- scope: openid\n  description: Request an OpenID\
  \ Connect ID token alongside the access token.\n  sources: [https://login.decisiv.net/.well-known/openid-configuration]\n- scope: public\n  description: Public / unauthenticated-tier access.\n  sources: [https://login.decisiv.net/.well-known/openid-configuration]\n- scope: read\n  description: Read access to the resources the OAuth Application is provisioned for.\n  sources: [https://login.decisiv.net/.well-known/openid-configuration]\n- scope: write\n  description: Create access to the resources the OAuth Application is provisioned for.\n  sources: [https://login.decisiv.net/.well-known/openid-configuration]\n- scope: update\n  description: Modify access to the resources the OAuth Application is provisioned for.\n  sources: [https://login.decisiv.net/.well-known/openid-configuration]\ngrant_types_supported:\n- authorization_code\n- refresh_token\n- password\n- client_credentials\npkce:\n  supported: true\n  code_challenge_methods: [S256, plain]\nid_token:\n  signing_alg: [ES256]\n  jwks_uri:\
  \ https://login.decisiv.net/oauth/discovery/keys\n  claims:\n  - iss\n  - sub\n  - aud\n  - exp\n  - iat\n  - username\n  - email\n  - id\n  - first_name\n  - last_name\n  - name\n  - phone\n  - roles\n  - rbac_groups\n  - rbac_permissions\nendpoints:\n  authorization: https://login.decisiv.net/oauth/authorize\n  token: https://login.decisiv.net/oauth/token\n  revocation: https://login.decisiv.net/oauth/revoke\n  introspection: https://login.decisiv.net/oauth/introspect\n  userinfo: https://login.decisiv.net/oauth/userinfo\nx-evidence:\n- url: https://login.decisiv.net/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/vnd.api+json\n- url: https://login.decisiv.net/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/vnd.api+json\n- url: https://login.decisiv.net/oauth/discovery/keys\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decisiv/refs/heads/main/scopes/decisiv-scopes.yml
summary_line: 5 scopes · authorizationCode/password
tags:
- Company
- commercial-vehicle
- fleet-management
- service-relationship-management
- telematics
- asset-management
- maintenance-and-repair
- heavy-duty-trucking
- transportation
- dealer-management
- json-api
- webhooks
token_urls:
- https://login.decisiv.net/oauth/token
- https://portal.decisivapps.com/oauth/token
---
