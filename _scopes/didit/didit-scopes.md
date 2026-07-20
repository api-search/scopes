---
api_specs:
- filename: didit-openapi-original.json
  format: json
  label: Didit Verification API
  slug: didit-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.didit.me/integration/programmatic-registration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Didit Scopes
name_suffix: OAuth Scopes
note: 'The verification REST API authenticates with an x-api-key header (no OAuth scopes). OAuth 2.1 applies to the Business Console / Management surface and the hosted MCP server, whose authorization-server metadata advertises these scopes. Flow: authorization_code + refresh_token, PKCE S256, public clients.'
overview: 'Didit publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Didit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Didit
provider_slug: didit
schemes:
- authorization_url: https://business.didit.me/authorize
  flows:
  - flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
  issuer: https://business.didit.me
  name: OAuth2
  registration_url: https://business.didit.me/api/auth/oauth-register
  token_url: https://business.didit.me/api/auth/oauth-token
scope_count: 5
scope_names:
- openid
- profile
- email
- didit:management
- didit:verification
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access to the signed-in user's profile.
  flows: []
  scope: profile
- description: Access to the signed-in user's email address.
  flows: []
  scope: email
- description: Management API access — workflows, lists, webhooks, users, businesses, billing.
  flows: []
  scope: didit:management
- description: Verification API access — sessions and standalone verification operations.
  flows: []
  scope: didit:verification
slug: didit-scopes
source_filename: didit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://business.didit.me/.well-known/oauth-authorization-server\ndocs: https://docs.didit.me/integration/programmatic-registration\nnote: >-\n  The verification REST API authenticates with an x-api-key header (no OAuth\n  scopes). OAuth 2.1 applies to the Business Console / Management surface and\n  the hosted MCP server, whose authorization-server metadata advertises these\n  scopes. Flow: authorization_code + refresh_token, PKCE S256, public clients.\nschemes:\n  - name: OAuth2\n    issuer: https://business.didit.me\n    authorization_url: https://business.didit.me/authorize\n    token_url: https://business.didit.me/api/auth/oauth-token\n    registration_url: https://business.didit.me/api/auth/oauth-register\n    flows:\n      - flow: authorizationCode\n        pkce: S256\n        grant_types: [authorization_code, refresh_token]\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication.\n  - scope: profile\n\
  \    description: Access to the signed-in user's profile.\n  - scope: email\n    description: Access to the signed-in user's email address.\n  - scope: \"didit:management\"\n    description: Management API access — workflows, lists, webhooks, users, businesses, billing.\n  - scope: \"didit:verification\"\n    description: Verification API access — sessions and standalone verification operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/scopes/didit-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Compliance
- Biometrics
- Transaction Monitoring
- Crypto
token_urls: []
---
