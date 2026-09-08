---
authorization_urls:
- https://auth.adaptiveinsurance.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Adaptive Insurance Scopes
name_suffix: OAuth Scopes
note: These are the scopes the Adaptive Insurance identity tenant advertises in its own OIDC discovery document. They are the standard OpenID Connect claim scopes exposed by the tenant, not a documented API permission model — Adaptive publishes no public API and no scope/permission reference page. Recorded because they were fetched, not because they constitute an authorization contract for third-party integrators.
overview: 'Adaptive Insurance publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adaptive Insurance API on a user''s behalf.


  Tokens are issued from https://auth.adaptiveinsurance.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adaptive Insurance
provider_slug: adaptive-insurance
schemes:
- flows:
  - authorizationUrl: https://auth.adaptiveinsurance.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.adaptiveinsurance.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.adaptiveinsurance.com/oauth/token
  - deviceAuthorizationUrl: https://auth.adaptiveinsurance.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.adaptiveinsurance.com/oauth/token
  name: adaptive-auth0-tenant
  source: well-known/adaptive-insurance-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OpenID Connect authentication; issues an ID token
  flows: []
  scope: openid
- description: Basic profile claims
  flows: []
  scope: profile
- description: Issue a refresh token
  flows: []
  scope: offline_access
- description: Full name claim
  flows: []
  scope: name
- description: Given name claim
  flows: []
  scope: given_name
- description: Family name claim
  flows: []
  scope: family_name
- description: Nickname claim
  flows: []
  scope: nickname
- description: Email address claim
  flows: []
  scope: email
- description: Email verification status claim
  flows: []
  scope: email_verified
- description: Profile picture claim
  flows: []
  scope: picture
- description: Account creation timestamp claim
  flows: []
  scope: created_at
- description: Linked identity provider records
  flows: []
  scope: identities
- description: Phone number claim
  flows: []
  scope: phone
- description: Address claim
  flows: []
  scope: address
slug: adaptive-insurance-scopes
source_filename: adaptive-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://auth.adaptiveinsurance.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes the Adaptive Insurance identity tenant advertises in its own\n  OIDC discovery document. They are the standard OpenID Connect claim scopes exposed by\n  the tenant, not a documented API permission model — Adaptive publishes no public API\n  and no scope/permission reference page. Recorded because they were fetched, not\n  because they constitute an authorization contract for third-party integrators.\nschemes:\n  - name: adaptive-auth0-tenant\n    source: well-known/adaptive-insurance-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.adaptiveinsurance.com/authorize\n        tokenUrl: https://auth.adaptiveinsurance.com/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://auth.adaptiveinsurance.com/oauth/token\n      - flow: deviceCode\n        deviceAuthorizationUrl:\
  \ https://auth.adaptiveinsurance.com/oauth/device/code\n        tokenUrl: https://auth.adaptiveinsurance.com/oauth/token\nscopes:\n  - {scope: openid, description: 'OpenID Connect authentication; issues an ID token', standard: true}\n  - {scope: profile, description: 'Basic profile claims', standard: true}\n  - {scope: offline_access, description: 'Issue a refresh token', standard: true}\n  - {scope: name, description: 'Full name claim', standard: true}\n  - {scope: given_name, description: 'Given name claim', standard: true}\n  - {scope: family_name, description: 'Family name claim', standard: true}\n  - {scope: nickname, description: 'Nickname claim', standard: true}\n  - {scope: email, description: 'Email address claim', standard: true}\n  - {scope: email_verified, description: 'Email verification status claim', standard: true}\n  - {scope: picture, description: 'Profile picture claim', standard: true}\n  - {scope: created_at, description: 'Account creation timestamp claim', standard:\
  \ false}\n  - {scope: identities, description: 'Linked identity provider records', standard: false}\n  - {scope: phone, description: 'Phone number claim', standard: true}\n  - {scope: address, description: 'Address claim', standard: true}\nscope_count: 14\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-insurance/refs/heads/main/scopes/adaptive-insurance-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Insurance
- Insurtech
- Parametric Insurance
- Specialty Insurance
- Climate Risk
- Weather Data
- Managing General Agent
- Flood
- Power Outage
token_urls:
- https://auth.adaptiveinsurance.com/oauth/token
---
