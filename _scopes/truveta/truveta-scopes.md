---
authorization_urls:
- https://login.truveta.com/authorize
description: Truveta publishes no OpenAPI and no product-level permission or scope reference. The scopes below are the ones its Auth0 identity tenant advertises in `scopes_supported` on the anonymous OIDC discovery document — standard OpenID Connect and Auth0 scopes governing identity and profile claims for the Truveta Studio application. They are NOT Truveta product/data scopes; no such reference is published publicly.
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Truveta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Truveta publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Truveta API on a user''s behalf.


  Tokens are issued from https://login.truveta.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Truveta
provider_slug: truveta
schemes:
- flows:
  - authorizationUrl: https://login.truveta.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.truveta.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.truveta.com/oauth/token
  - deviceAuthorizationUrl: https://login.truveta.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://login.truveta.com/oauth/token
  issuer: https://login.truveta.com/
  name: TruvetaOIDC
  source: well-known/truveta-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- address
- phone
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
scopes:
- description: Request an ID token and authenticate the end user via OpenID Connect.
  flows: []
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows: []
  scope: profile
- description: The end user's email address.
  flows: []
  scope: email
- description: Whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: The end user's postal address claim.
  flows: []
  scope: address
- description: The end user's phone number claim.
  flows: []
  scope: phone
- description: Issue a refresh token for long-lived access without re-authentication.
  flows: []
  scope: offline_access
- description: Full name claim.
  flows: []
  scope: name
- description: Given name claim.
  flows: []
  scope: given_name
- description: Family name claim.
  flows: []
  scope: family_name
- description: Nickname claim.
  flows: []
  scope: nickname
- description: Profile picture URL claim.
  flows: []
  scope: picture
- description: Timestamp the user account was created in the Auth0 tenant.
  flows: []
  scope: created_at
- description: Linked identity-provider identities for the user account.
  flows: []
  scope: identities
slug: truveta-scopes
source_filename: truveta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://login.truveta.com/.well-known/openid-configuration\ndescription: >-\n  Truveta publishes no OpenAPI and no product-level permission or scope\n  reference. The scopes below are the ones its Auth0 identity tenant advertises\n  in `scopes_supported` on the anonymous OIDC discovery document — standard\n  OpenID Connect and Auth0 scopes governing identity and profile claims for the\n  Truveta Studio application. They are NOT Truveta product/data scopes; no such\n  reference is published publicly.\nscheme_type: openIdConnect\nschemes:\n  - name: TruvetaOIDC\n    source: well-known/truveta-openid-configuration.json\n    issuer: https://login.truveta.com/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://login.truveta.com/authorize\n        tokenUrl: https://login.truveta.com/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://login.truveta.com/oauth/token\n      - flow: deviceCode\n\
  \        deviceAuthorizationUrl: https://login.truveta.com/oauth/device/code\n        tokenUrl: https://login.truveta.com/oauth/token\nscopes:\n  - scope: openid\n    description: Request an ID token and authenticate the end user via OpenID Connect.\n    standard: oidc-core\n  - scope: profile\n    description: Basic profile claims (name, given_name, family_name, nickname, picture).\n    standard: oidc-core\n  - scope: email\n    description: The end user's email address.\n    standard: oidc-core\n  - scope: email_verified\n    description: Whether the end user's email address has been verified.\n    standard: auth0\n  - scope: address\n    description: The end user's postal address claim.\n    standard: oidc-core\n  - scope: phone\n    description: The end user's phone number claim.\n    standard: oidc-core\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access without re-authentication.\n    standard: oidc-core\n  - scope: name\n    description: Full\
  \ name claim.\n    standard: auth0\n  - scope: given_name\n    description: Given name claim.\n    standard: auth0\n  - scope: family_name\n    description: Family name claim.\n    standard: auth0\n  - scope: nickname\n    description: Nickname claim.\n    standard: auth0\n  - scope: picture\n    description: Profile picture URL claim.\n    standard: auth0\n  - scope: created_at\n    description: Timestamp the user account was created in the Auth0 tenant.\n    standard: auth0\n  - scope: identities\n    description: Linked identity-provider identities for the user account.\n    standard: auth0\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://login.truveta.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truveta/refs/heads/main/scopes/truveta-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Healthcare
- Health Data
- Electronic Health Records
- Real-World Evidence
- Clinical Research
- Life Sciences
- Genomics
- Analytics
- Artificial Intelligence
- Data Platform
token_urls:
- https://login.truveta.com/oauth/token
---
