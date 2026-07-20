---
authorization_urls:
- https://auth.request.finance/authorize
description: ''
docs: https://docs.request.finance/going-live
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Consola Finance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Consola Finance publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Consola Finance API on a user''s behalf.


  Tokens are issued from https://auth.request.finance/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Consola Finance
provider_slug: consola-finance
schemes:
- audience: accounts
  flows:
  - authorizationUrl: https://auth.request.finance/authorize
    flow: authorizationCode
    tokenUrl: https://auth.request.finance/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.request.finance/oauth/token
  issuer: https://auth.request.finance/
  name: OAuth2
  source: well-known/consola-finance-openid-configuration.json
scope_count: 5
scope_names:
- openid
- profile
- email
- offline_access
- user:read
scopes:
- description: OIDC authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived access (Authorization Code Flow only).
  flows:
  - authorizationCode
  scope: offline_access
- description: Request Finance application scope to read the user and the organizations they belong to (see the Organizations docs).
  flows:
  - authorizationCode
  scope: user:read
slug: consola-finance-scopes
source_filename: consola-finance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.request.finance/.well-known/openid-configuration\ndocs: https://docs.request.finance/going-live\nnotes: >-\n  Request Finance OAuth (Auth0-backed) scopes. Standard OIDC scopes come from\n  the live discovery document (scopes_supported); user:read is documented on the\n  Going Live page as a Request Finance application scope. No OpenAPI is published\n  so scopes are not tied to specific operations.\nschemes:\n- name: OAuth2\n  source: well-known/consola-finance-openid-configuration.json\n  issuer: https://auth.request.finance/\n  audience: accounts\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.request.finance/authorize\n    tokenUrl: https://auth.request.finance/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.request.finance/oauth/token\nscopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token.\n  flows: [authorizationCode]\n- scope: profile\n\
  \  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email and email_verified claims.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access (Authorization Code Flow only).\n  flows: [authorizationCode]\n- scope: user:read\n  description: >-\n    Request Finance application scope to read the user and the organizations they\n    belong to (see the Organizations docs).\n  flows: [authorizationCode]\n  source: https://docs.request.finance/going-live\noidc_scopes_supported:\n- openid\n- profile\n- offline_access\n- name\n- given_name\n- family_name\n- nickname\n- email\n- email_verified\n- picture\n- created_at\n- identities\n- phone\n- address\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consola-finance/refs/heads/main/scopes/consola-finance-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Company
- Crypto Accounting
- Digital Assets
- Web3 Finance
- Accounts Payable
- Accounts Receivable
- Invoicing
- Payroll
- Bookkeeping
- Blockchain
token_urls:
- https://auth.request.finance/oauth/token
---
