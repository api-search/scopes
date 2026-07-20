---
api_specs:
- filename: fullview-bug-report-openapi.yml
  format: yaml
  label: Fullview Bug Report API
  slug: fullview-bug-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullview/refs/heads/main/openapi/fullview-bug-report-openapi.yml
authorization_urls:
- https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/auth
description: ''
docs: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Fullview Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fullview publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fullview API on a user''s behalf.


  Tokens are issued from https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fullview
provider_slug: fullview
schemes:
- flows:
  - authorizationUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token
  name: fullviewOIDC
  source: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration
scope_count: 12
scope_names:
- openid
- profile
- email
- address
- phone
- roles
- offline_access
- microprofile-jwt
- service_account
- web-origins
- acr
- basic
scopes:
- description: OpenID Connect authentication; required to receive an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email claim.
  flows: []
  scope: email
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Access to the user's phone claim.
  flows: []
  scope: phone
- description: Include realm/client role mappings in the token.
  flows: []
  scope: roles
- description: Issue a refresh token for offline access.
  flows: []
  scope: offline_access
- description: MicroProfile JWT claims (groups, upn) for service authorization.
  flows: []
  scope: microprofile-jwt
- description: Scope associated with client-credentials service accounts.
  flows: []
  scope: service_account
- description: Allowed web origins claim for CORS.
  flows: []
  scope: web-origins
- description: Authentication Context Class Reference handling.
  flows: []
  scope: acr
- description: Keycloak basic client scope (sub, auth_time claims).
  flows: []
  scope: basic
slug: fullview-scopes
source_filename: fullview-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration\ndocs: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration\nschemes:\n  - name: fullviewOIDC\n    source: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/.well-known/openid-configuration\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/auth\n        tokenUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token\n      - flow: clientCredentials\n        tokenUrl: https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; required to receive an ID token.\n  - scope: profile\n    description: Access to the user's basic profile claims.\n  - scope:\
  \ email\n    description: Access to the user's email claim.\n  - scope: address\n    description: Access to the user's address claim.\n  - scope: phone\n    description: Access to the user's phone claim.\n  - scope: roles\n    description: Include realm/client role mappings in the token.\n  - scope: offline_access\n    description: Issue a refresh token for offline access.\n  - scope: microprofile-jwt\n    description: MicroProfile JWT claims (groups, upn) for service authorization.\n  - scope: service_account\n    description: Scope associated with client-credentials service accounts.\n  - scope: web-origins\n    description: Allowed web origins claim for CORS.\n  - scope: acr\n    description: Authentication Context Class Reference handling.\n  - scope: basic\n    description: Keycloak basic client scope (sub, auth_time claims).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullview/refs/heads/main/scopes/fullview-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Company
- Customer Support
- Cobrowsing
- Session Replay
- Customer Experience
- Developer Tools
- Help Desk
- SaaS
token_urls:
- https://auth.eu1.fullview.io/realms/fullview-idp-users-eu1/protocol/openid-connect/token
---
