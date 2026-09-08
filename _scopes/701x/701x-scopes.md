---
api_specs:
- filename: 701x-api-v1-openapi.json
  format: json
  label: 701x API V1
  slug: 701x-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/openapi/701x-api-v1-openapi.json
authorization_urls:
- https://login.701x.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 701X Scopes
name_suffix: OAuth Scopes
note: ''
overview: '701x publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 701x API on a user''s behalf.


  Tokens are issued from https://login.701x.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 701x
provider_slug: 701x
schemes:
- flows:
  - authorizationUrl: https://login.701x.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://login.701x.com/connect/token
  name: oauth2
  source: openapi/701x-api-v1-openapi.json
scope_count: 6
scope_names:
- API701x
- api1
- openid
- profile
- email
- offline_access
scopes:
- description: The scope the API enforces. Required by 1,158 of 1,391 operations across every resource family. Not described anywhere by the provider and not listed in the authorization server's scopes_supported.
  flows:
  - authorizationCode
  scope: API701x
- description: '"Demo API - full access" — the only scope described in the OpenAPI securityScheme, and one of the five scopes the authorization server advertises. No operation in the contract requires it.'
  flows:
  - authorizationCode
  scope: api1
- description: OpenID Connect base scope; returns an id_token.
  flows: []
  scope: openid
- description: Standard OIDC profile claims (name, family_name, given_name, picture, locale, and role).
  flows: []
  scope: profile
- description: Standard OIDC email and email_verified claims.
  flows: []
  scope: email
- description: Issues a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: 701x-scopes
source_filename: 701x-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  openapi/701x-api-v1-openapi.json (securitySchemes + per-operation security requirements) +\n  https://login.701x.com/.well-known/openid-configuration (HTTP 200, fetched 2026-09-05)\ndocs: null\ndocs_note: >-\n  701x publishes no scopes or permissions reference page. The scope set below is what the contract\n  and the authorization server's own discovery document actually declare — nothing is inferred.\nschemes:\n- name: oauth2\n  source: openapi/701x-api-v1-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.701x.com/connect/authorize\n    tokenUrl: https://login.701x.com/connect/token\ngranularity: coarse\ngranularity_note: >-\n  There is exactly one API scope for the entire 1,391-operation surface. A token that can read a\n  herd inventory can also mass-delete animals, cancel subscriptions and run every admin\n  controller. There is no read/write split, no per-resource scope, and no\
  \ way for an integrator or\n  an agent to hold least privilege.\nscopes:\n- scope: API701x\n  description: >-\n    The scope the API enforces. Required by 1,158 of 1,391 operations across every resource\n    family. Not described anywhere by the provider and not listed in the authorization server's\n    scopes_supported.\n  flows:\n  - authorizationCode\n  operations: 1158\n  sources:\n  - openapi/701x-api-v1-openapi.json\n- scope: api1\n  description: >-\n    \"Demo API - full access\" — the only scope described in the OpenAPI securityScheme, and one of\n    the five scopes the authorization server advertises. No operation in the contract requires it.\n  flows:\n  - authorizationCode\n  operations: 0\n  sources:\n  - openapi/701x-api-v1-openapi.json\n  - https://login.701x.com/.well-known/openid-configuration\n- scope: openid\n  description: OpenID Connect base scope; returns an id_token.\n  sources:\n  - https://login.701x.com/.well-known/openid-configuration\n- scope: profile\n  description:\
  \ Standard OIDC profile claims (name, family_name, given_name, picture, locale, and role).\n  sources:\n  - https://login.701x.com/.well-known/openid-configuration\n- scope: email\n  description: Standard OIDC email and email_verified claims.\n  sources:\n  - https://login.701x.com/.well-known/openid-configuration\n- scope: offline_access\n  description: Issues a refresh token for long-lived access.\n  sources:\n  - https://login.701x.com/.well-known/openid-configuration\nfindings:\n- >-\n  Scope mismatch: the enforced scope (API701x) is absent from scopes_supported, while the\n  documented scope (api1) is enforced by nothing. Integrators must discover API701x by reading the\n  per-operation security requirements in the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/701x/refs/heads/main/scopes/701x-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Agriculture
- AgTech
- Livestock
- Cattle Management
- Ranch Management
- Animal Health
- IoT
- GPS Tracking
- Traceability
- Beef Production
token_urls:
- https://login.701x.com/connect/token
---
