---
api_specs:
- filename: candis-openapi.json
  format: json
  label: Candis API
  slug: candis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/openapi/candis-openapi.json
authorization_urls:
- https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/auth
description: ''
docs: https://developer.candis.io/docs/access-token-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Candis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Candis publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Candis API on a user''s behalf.


  Tokens are issued from https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Candis
provider_slug: candis
schemes:
- flows:
  - authorizationUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token
  name: oauth2
  source: https://developer.candis.io/docs/how-to-authenticate
scope_count: 13
scope_names:
- exports
- core_data
- offline_access
- service_account
- openid
- email
- profile
- address
- phone
- roles
- acr
- microprofile-jwt
- web-origins
scopes:
- description: Access to the Export API (create/read exports and exported postings, download export files).
  flows:
  - authorizationCode
  scope: exports
- description: Access to the Core Data API (import/update general ledger accounts, cost dimensions, additional delivery costs, contacts).
  flows:
  - authorizationCode
  scope: core_data
- description: Issues long-lived refresh tokens so token exchanges remain valid for an extended period (~6-24 months) without re-login; for long-running/background services.
  flows:
  - authorizationCode
  - clientCredentials
  scope: offline_access
- description: Service-account (client-credentials) scope for machine-to-machine access.
  flows:
  - clientCredentials
  scope: service_account
- description: Standard OpenID Connect scope (ID token).
  flows:
  - authorizationCode
  scope: openid
- description: User email claim. Core scope, enabled by default.
  flows: []
  scope: email
- description: User profile claims. Core scope, enabled by default.
  flows: []
  scope: profile
- description: User address claims (OIDC).
  flows: []
  scope: address
- description: User phone claims (OIDC).
  flows: []
  scope: phone
- description: Realm/client role claims (Keycloak).
  flows: []
  scope: roles
- description: Authentication Context Class Reference (OIDC).
  flows: []
  scope: acr
- description: MicroProfile JWT claims (Keycloak).
  flows: []
  scope: microprofile-jwt
- description: Allowed web origins claim (Keycloak).
  flows: []
  scope: web-origins
slug: candis-scopes
source_filename: candis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.candis.io/docs/access-token-scopes\ndocs: https://developer.candis.io/docs/access-token-scopes\noidc_discovery: https://id.my.candis.io/auth/realms/candis/.well-known/openid-configuration\nschemes:\n- name: oauth2\n  source: https://developer.candis.io/docs/how-to-authenticate\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/auth\n    tokenUrl: https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token\nnotes: >-\n  Scopes are requested as a space-delimited value in the OAuth scope parameter, e.g.\n  \"scope=offline_access core_data exports\". The exports and core_data scopes are marked\n  experimental (strict validation not yet enforced). email and profile are core scopes\n  enabled by default and need not be requested explicitly.\nscopes:\n- scope: exports\n  description: Access to the Export API (create/read exports\
  \ and exported postings, download export files).\n  status: experimental\n  flows: [authorizationCode]\n- scope: core_data\n  description: Access to the Core Data API (import/update general ledger accounts, cost dimensions, additional delivery costs, contacts).\n  status: experimental\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issues long-lived refresh tokens so token exchanges remain valid for an extended period (~6-24 months) without re-login; for long-running/background services.\n  flows: [authorizationCode, clientCredentials]\n- scope: service_account\n  description: Service-account (client-credentials) scope for machine-to-machine access.\n  flows: [clientCredentials]\n- scope: openid\n  description: Standard OpenID Connect scope (ID token).\n  flows: [authorizationCode]\n- scope: email\n  description: User email claim. Core scope, enabled by default.\n  default: true\n- scope: profile\n  description: User profile claims. Core scope, enabled by default.\n\
  \  default: true\n- scope: address\n  description: User address claims (OIDC).\n- scope: phone\n  description: User phone claims (OIDC).\n- scope: roles\n  description: Realm/client role claims (Keycloak).\n- scope: acr\n  description: Authentication Context Class Reference (OIDC).\n- scope: microprofile-jwt\n  description: MicroProfile JWT claims (Keycloak).\n- scope: web-origins\n  description: Allowed web origins claim (Keycloak).\nscopes_supported_from_discovery:\n- openid\n- basic\n- service_account\n- acr\n- microprofile-jwt\n- offline_access\n- core_data\n- roles\n- address\n- exports\n- phone\n- web-origins\n- email\n- profile\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candis/refs/heads/main/scopes/candis-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Company
- Fintech
- Accounts Payable
- Spend Management
- Invoice Management
- Financial Process Automation
- Accounting
- DATEV
- OCR
- Germany
token_urls:
- https://id.my.candis.io/auth/realms/candis/protocol/openid-connect/token
---
