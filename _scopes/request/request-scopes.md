---
api_specs:
- filename: 24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
  format: yaml
  label: Request Finance AP and AR API
  slug: request-finance-ap-and-ar-api
  spec_type: Postman
  url: https://www.postman.com/request-finance/workspace/request-finance-api-public/documentation/24913360-b5105a65-a6bd-4247-b3b1-ed60e5c8f5cb
authorization_urls: []
description: ''
docs: https://docs.request.finance/going-live
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Request Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Request Finance publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Request Finance API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Request Finance
provider_slug: request
schemes:
- audience: accounts
  authorizationUrl: https://auth.request.finance/authorize
  flows:
  - authorizationCode
  - clientCredentials
  issuer: https://auth.request.finance
  name: oauth2
  tokenUrl: https://auth.request.finance/oauth/token
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- user:read
scopes:
- description: Standard OpenID Connect scope; enables ID token issuance.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Issues a refresh token so the app can obtain new access tokens after the 24-hour access-token expiry. Required for long-lived Authorization Code Flow integrations; not used in Client Credentials Flow.
  flows:
  - authorizationCode
  scope: offline_access
- description: Read access to user data, including listing the organizations a user belongs to (GET /users/organizations).
  flows:
  - authorizationCode
  scope: user:read
slug: request-scopes
source_filename: request-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.request.finance/going-live\ndocs: https://docs.request.finance/going-live\nschemes:\n- name: oauth2\n  issuer: https://auth.request.finance\n  audience: accounts\n  authorizationUrl: https://auth.request.finance/authorize\n  tokenUrl: https://auth.request.finance/oauth/token\n  flows: [authorizationCode, clientCredentials]\nscopes:\n- scope: openid\n  description: Standard OpenID Connect scope; enables ID token issuance.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access to the user's email address.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: >-\n    Issues a refresh token so the app can obtain new access tokens after the 24-hour\n    access-token expiry. Required for long-lived Authorization Code Flow integrations;\n    not used in Client Credentials Flow.\n  flows:\
  \ [authorizationCode]\n- scope: user:read\n  description: >-\n    Read access to user data, including listing the organizations a user belongs to\n    (GET /users/organizations).\n  flows: [authorizationCode]\n  source: https://docs.request.finance/organizations\nnotes: >-\n  The docs enumerate a baseline scope set (openid profile email offline_access) plus\n  additional scopes such as user:read. Use prompt=consent on the authorization URL to\n  force re-consent when a user is missing a scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/request/refs/heads/main/scopes/request-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Payments
- Invoicing
- Crypto
- Web3
- Payroll
- Stablecoins
- Accounts Payable
- Accounts Receivable
- Fintech
- Blockchain
- REST API
token_urls: []
---
