---
authorization_urls:
- https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Allwork Scopes
name_suffix: OAuth Scopes
note: Scopes are taken verbatim from scopes_supported in AllWork's live OpenID Connect discovery document for Keycloak realm AWN1. These are the standard OIDC/Keycloak client scopes — AllWork publishes no application-specific (workforce, payroll, scheduling) scope vocabulary, and no scopes reference page exists on allworknow.com.
overview: 'AllWork publishes 10 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AllWork API on a user''s behalf.


  Tokens are issued from https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AllWork
provider_slug: allwork
schemes:
- flows:
  - authorizationUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token
  - deviceAuthorizationUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth/device
    flow: deviceCode
    tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token
  name: allworkOAuth2
  source: well-known/allwork-openid-configuration.json
scope_count: 10
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- roles
- acr
- web-origins
- microprofile-jwt
scopes:
- description: Standard OpenID Connect scope; requests an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, preferred_username).
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Address claim.
  flows: []
  scope: address
- description: Phone number claim.
  flows: []
  scope: phone
- description: Requests a refresh token usable while the user is offline.
  flows: []
  scope: offline_access
- description: Keycloak client scope carrying realm and client role mappings.
  flows: []
  scope: roles
- description: Keycloak client scope carrying the authentication context class reference.
  flows: []
  scope: acr
- description: Keycloak client scope carrying allowed CORS web origins.
  flows: []
  scope: web-origins
- description: Keycloak client scope emitting MicroProfile JWT claims (upn, groups).
  flows: []
  scope: microprofile-jwt
slug: allwork-scopes
source_filename: allwork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration\nnote: >-\n  Scopes are taken verbatim from scopes_supported in AllWork's live OpenID\n  Connect discovery document for Keycloak realm AWN1. These are the standard\n  OIDC/Keycloak client scopes — AllWork publishes no application-specific\n  (workforce, payroll, scheduling) scope vocabulary, and no scopes reference\n  page exists on allworknow.com.\ndocs: null\nschemes:\n  - name: allworkOAuth2\n    source: well-known/allwork-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth\n        tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token\n      - flow: clientCredentials\n        tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token\n      - flow: deviceCode\n        deviceAuthorizationUrl:\
  \ https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/auth/device\n        tokenUrl: https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    flows: [authorizationCode]\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: profile\n    description: Basic profile claims (name, given_name, family_name, preferred_username).\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: email\n    description: Email address claim.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: address\n    description: Address claim.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: phone\n    description: Phone number claim.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: offline_access\n    description: Requests a refresh token usable while the user is offline.\n    sources: [well-known/allwork-openid-configuration.json]\n\
  \  - scope: roles\n    description: Keycloak client scope carrying realm and client role mappings.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: acr\n    description: Keycloak client scope carrying the authentication context class reference.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: web-origins\n    description: Keycloak client scope carrying allowed CORS web origins.\n    sources: [well-known/allwork-openid-configuration.json]\n  - scope: microprofile-jwt\n    description: Keycloak client scope emitting MicroProfile JWT claims (upn, groups).\n    sources: [well-known/allwork-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.allworknow.com/realms/AWN1/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allwork/refs/heads/main/scopes/allwork-scopes.yml
summary_line: 10 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Workforce Management
- Human Resources
- Staffing
- Payroll
- Employer of Record
- Contingent Workforce
- Gig Economy
- Scheduling
- Time and Attendance
- Compliance
token_urls:
- https://auth.allworknow.com/realms/AWN1/protocol/openid-connect/token
---
