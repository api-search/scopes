---
authorization_urls:
- https://api.healthex.io/oauth/authorize
description: ''
docs: https://docs.healthex.io/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Healthex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HealthEx publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HealthEx API on a user''s behalf.


  Tokens are issued from https://api.healthex.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HealthEx
provider_slug: healthex
schemes:
- flows:
  - authorizationUrl: https://api.healthex.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://api.healthex.io/oauth/token
  name: patientOAuth2
  source: https://api.healthex.io/.well-known/oauth-authorization-server
scope_count: 5
scope_names:
- patient/*.read
- offline_access
- openid
- profile
- email
scopes:
- description: SMART-on-FHIR wildcard read scope granting read access to all FHIR resource types for a patient who has consented to share their record.
  flows:
  - authorizationCode
  scope: patient/*.read
- description: Issue a refresh token for long-lived, offline access.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim.
  flows:
  - authorizationCode
  scope: email
slug: healthex-scopes
source_filename: healthex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.healthex.io/.well-known/oauth-authorization-server\ndocs: https://docs.healthex.io/authentication\nschemes:\n  - name: patientOAuth2\n    source: https://api.healthex.io/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.healthex.io/oauth/authorize\n        tokenUrl: https://api.healthex.io/oauth/token\n        pkce: S256\nscopes:\n  - scope: patient/*.read\n    description: >-\n      SMART-on-FHIR wildcard read scope granting read access to all FHIR\n      resource types for a patient who has consented to share their record.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server, oauth-protected-resource]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived, offline access.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server]\n  - scope: openid\n    description: OpenID Connect\
  \ authentication.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server]\n  - scope: profile\n    description: Basic profile claims.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server]\n  - scope: email\n    description: Email address claim.\n    flows: [authorizationCode]\n    sources: [oauth-authorization-server]\nnotes: >-\n  Patient data access is scope-gated via SMART-on-FHIR patient/*.read. The\n  organization-level API (JWT from apiKey/apiSecret) is not scoped — HealthEx\n  states none of the currently supported organization APIs require additional\n  permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthex/refs/heads/main/scopes/healthex-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Company
- Healthcare
- Health Records
- FHIR
- Patient Consent
- Data Sharing
- Interoperability
- TEFCA
- MCP
- Agents
token_urls:
- https://api.healthex.io/oauth/token
---
