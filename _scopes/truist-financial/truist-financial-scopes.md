---
api_specs:
- filename: truist-personal-small-business-accounts-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Accounts API
  slug: truist-personal-small-business-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-accounts-openapi.yml
- filename: truist-personal-small-business-transactions-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Transactions API
  slug: truist-personal-small-business-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-personal-small-business-transactions-openapi.yml
- filename: truist-commercial-accounts-openapi.yml
  format: yaml
  label: Truist Commercial Accounts API
  slug: truist-commercial-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-accounts-openapi.yml
- filename: truist-commercial-account-transactions-openapi.yml
  format: yaml
  label: Truist Commercial Account Transactions API
  slug: truist-commercial-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/openapi/truist-commercial-account-transactions-openapi.yml
authorization_urls:
- https://api.truist.com/oauth2/authorize
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Truist Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Truist Financial publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Truist Financial API on a user''s behalf.


  Tokens are issued from https://api.truist.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Truist Financial
provider_slug: truist-financial
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  source: openapi/truist-commercial-account-transactions-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  source: openapi/truist-commercial-accounts-openapi.yml
- flows:
  - authorizationUrl: https://api.truist.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  source: openapi/truist-personal-small-business-accounts-openapi.yml
- flows:
  - authorizationUrl: https://api.truist.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.truist.com/oauth2/token
  name: OAuth2
  source: openapi/truist-personal-small-business-transactions-openapi.yml
scope_count: 4
scope_names:
- accounts:read
- commercial.accounts:read
- commercial.transactions:read
- transactions:read
scopes:
- description: Read access to account information
  flows:
  - authorizationCode
  scope: accounts:read
- description: Read access to commercial account information
  flows:
  - clientCredentials
  scope: commercial.accounts:read
- description: Read access to commercial transaction data
  flows:
  - clientCredentials
  scope: commercial.transactions:read
- description: Read access to transaction data
  flows:
  - authorizationCode
  scope: transactions:read
slug: truist-financial-scopes
source_filename: truist-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truist-commercial-account-transactions-openapi.yml, openapi/truist-commercial-accounts-openapi.yml,\n  openapi/truist-personal-small-business-accounts-openapi.yml, openapi/truist-personal-small-business-transactions-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/truist-commercial-account-transactions-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.truist.com/oauth2/token\n- name: OAuth2\n  source: openapi/truist-commercial-accounts-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.truist.com/oauth2/token\n- name: OAuth2\n  source: openapi/truist-personal-small-business-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.truist.com/oauth2/authorize\n    tokenUrl: https://api.truist.com/oauth2/token\n- name: OAuth2\n  source: openapi/truist-personal-small-business-transactions-openapi.yml\n  flows:\n  - flow:\
  \ authorizationCode\n    authorizationUrl: https://api.truist.com/oauth2/authorize\n    tokenUrl: https://api.truist.com/oauth2/token\nscopes:\n- scope: accounts:read\n  description: Read access to account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/truist-personal-small-business-accounts-openapi.yml\n- scope: commercial.accounts:read\n  description: Read access to commercial account information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/truist-commercial-accounts-openapi.yml\n- scope: commercial.transactions:read\n  description: Read access to commercial transaction data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/truist-commercial-account-transactions-openapi.yml\n- scope: transactions:read\n  description: Read access to transaction data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/truist-personal-small-business-transactions-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truist-financial/refs/heads/main/scopes/truist-financial-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Banking
- Financial Services
- Open Banking
- Commercial Banking
- Personal Banking
- Payments
- Accounts
- Transactions
- Fortune 500
token_urls:
- https://api.truist.com/oauth2/token
---
