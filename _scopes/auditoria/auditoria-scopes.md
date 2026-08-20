---
authorization_urls:
- https://auth.auditoria.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
- refreshToken
kind: oauth-scopes
layout: scope
method: probed
name: Auditoria Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Auditoria.AI publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, implicit, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Auditoria.AI API on a user''s behalf.


  Tokens are issued from https://auth.auditoria.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Auditoria.AI
provider_slug: auditoria
schemes:
- flows:
  - authorizationUrl: https://auth.auditoria.ai/authorize
    flow: authorizationCode
    tokenUrl: https://auth.auditoria.ai/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.auditoria.ai/oauth/token
  - deviceAuthorizationUrl: https://auth.auditoria.ai/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.auditoria.ai/oauth/token
  - authorizationUrl: https://auth.auditoria.ai/authorize
    flow: implicit
  - flow: refreshToken
    tokenUrl: https://auth.auditoria.ai/oauth/token
  issuer: https://auth.auditoria.ai/
  name: Auth0OIDC
  source: well-known/auditoria-openid-configuration.json
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
- description: Request an OpenID Connect ID token
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
- description: Linked identity-provider identities claim
  flows: []
  scope: identities
- description: Phone number claim
  flows: []
  scope: phone
- description: Address claim
  flows: []
  scope: address
slug: auditoria-scopes
source_filename: auditoria-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://auth.auditoria.ai/.well-known/openid-configuration\nscope_note: >-\n  These are the scopes the Auditoria Auth0 tenant advertises for signing in to the customer\n  application. They are the standard OpenID Connect identity/claim scopes - Auditoria\n  publishes no public API and therefore no resource-permission scope surface. There is no\n  scopes reference page in the documentation; nothing here was authored by API Evangelist.\nschemes:\n  - name: Auth0OIDC\n    source: well-known/auditoria-openid-configuration.json\n    issuer: https://auth.auditoria.ai/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://auth.auditoria.ai/authorize\n        tokenUrl: https://auth.auditoria.ai/oauth/token\n      - flow: clientCredentials\n        tokenUrl: https://auth.auditoria.ai/oauth/token\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://auth.auditoria.ai/oauth/device/code\n        tokenUrl:\
  \ https://auth.auditoria.ai/oauth/token\n      - flow: implicit\n        authorizationUrl: https://auth.auditoria.ai/authorize\n      - flow: refreshToken\n        tokenUrl: https://auth.auditoria.ai/oauth/token\nscopes:\n  - {scope: openid, description: 'Request an OpenID Connect ID token', kind: oidc-standard}\n  - {scope: profile, description: 'Basic profile claims', kind: oidc-standard}\n  - {scope: offline_access, description: 'Issue a refresh token', kind: oidc-standard}\n  - {scope: name, description: 'Full name claim', kind: oidc-claim}\n  - {scope: given_name, description: 'Given name claim', kind: oidc-claim}\n  - {scope: family_name, description: 'Family name claim', kind: oidc-claim}\n  - {scope: nickname, description: 'Nickname claim', kind: oidc-claim}\n  - {scope: email, description: 'Email address claim', kind: oidc-claim}\n  - {scope: email_verified, description: 'Email verification status claim', kind: oidc-claim}\n  - {scope: picture, description: 'Profile picture claim',\
  \ kind: oidc-claim}\n  - {scope: created_at, description: 'Account creation timestamp claim', kind: oidc-claim}\n  - {scope: identities, description: 'Linked identity-provider identities claim', kind: auth0-extension}\n  - {scope: phone, description: 'Phone number claim', kind: oidc-standard}\n  - {scope: address, description: 'Address claim', kind: oidc-standard}\nresource_scopes: []\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://auth.auditoria.ai/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auditoria/refs/heads/main/scopes/auditoria-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode/implicit/refreshToken
tags:
- Company
- Artificial Intelligence
- Finance
- Accounting
- Accounts Payable
- Accounts Receivable
- Automation
- ERP
- Agents
- Software-as-a-Service
- Invoicing
- Procurement
token_urls:
- https://auth.auditoria.ai/oauth/token
---
