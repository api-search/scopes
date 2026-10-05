---
api_specs:
- filename: plaid-plaid-api-openapi.yml
  format: yaml
  label: Plaid API
  slug: plaid-plaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-plaid-api-openapi.yml
- filename: plaid-account-information-api-openapi.yml
  format: yaml
  label: Plaid Account Information API
  slug: plaid-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-information-api-openapi.yml
- filename: plaid-account-statements-api-openapi.yml
  format: yaml
  label: Plaid Account Statements API
  slug: plaid-account-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-statements-api-openapi.yml
- filename: plaid-account-transactions-api-openapi.yml
  format: yaml
  label: Plaid Account Transactions API
  slug: plaid-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-account-transactions-api-openapi.yml
- filename: plaid-asset-transfer-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Asset Transfer Networks Information API
  slug: plaid-asset-transfer-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-asset-transfer-networks-information-api-openapi.yml
- filename: plaid-payment-networks-information-api-openapi.yml
  format: yaml
  label: Plaid Payment Networks Information API
  slug: plaid-payment-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-payment-networks-information-api-openapi.yml
- filename: plaid-personal-information-api-openapi.yml
  format: yaml
  label: Plaid Personal Information API
  slug: plaid-personal-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/openapi/plaid-personal-information-api-openapi.yml
authorization_urls:
- https://www.your-organization.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Plaid Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Plaid publishes 5 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Plaid API on a user''s behalf.


  Tokens are issued from https://www.your-organization.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Plaid
provider_slug: plaid
schemes:
- description: 'This API uses an [OAuth 2.0 authorization code flow](https://plaid.com/core-exchange/docs/authentication/oauth-flow) and accepts the resulting access token as a bearer token. For example, `curl -H ''Authorization: Bearer <ACCESS&#95;TOKEN>''`.'
  flows:
  - authorizationUrl: https://www.your-organization.com/authorize
    flow: authorizationCode
    tokenUrl: https://www.your-organization.com/token
  name: oauth2
  source: openapi/plaid-core-exchange-openapi.yml
- description: The Plaid API supports client credentials, authorization code, and custom delegation flows.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.plaid.com/oauth2/apiv2/token
  name: oauth2
  source: openapi/plaid-plaid-api-openapi.yml
scope_count: 5
scope_names:
- Account
- Customer
- Transactions
- cra:read
- user:write
scopes:
- description: (optional) Read account data
  flows:
  - authorizationCode
  scope: Account
- description: (optional) Read customer data
  flows:
  - authorizationCode
  scope: Customer
- description: (optional) Read transaction data
  flows:
  - authorizationCode
  scope: Transactions
- description: Read CRA report data.
  flows:
  - clientCredentials
  scope: cra:read
- description: Write user data.
  flows:
  - clientCredentials
  scope: user:write
slug: plaid-scopes
source_filename: plaid-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: derived\nsource: openapi/plaid-core-exchange-openapi.yml, openapi/plaid-plaid-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/plaid-core-exchange-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.your-organization.com/authorize\n    tokenUrl: https://www.your-organization.com/token\n  description: 'This API uses an [OAuth 2.0 authorization code flow](https://plaid.com/core-exchange/docs/authentication/oauth-flow)\n    and accepts the resulting access token as a bearer token. For example, `curl -H ''Authorization:\n    Bearer <ACCESS&#95;TOKEN>''`.'\n- name: oauth2\n  source: openapi/plaid-plaid-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.plaid.com/oauth2/apiv2/token\n  description: The Plaid API supports client credentials, authorization code, and custom delegation\n    flows.\nscopes:\n- scope: Account\n  description: (optional) Read account data\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/plaid-core-exchange-openapi.yml\n- scope: Customer\n  description: (optional) Read customer data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/plaid-core-exchange-openapi.yml\n- scope: Transactions\n  description: (optional) Read transaction data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/plaid-core-exchange-openapi.yml\n- scope: cra:read\n  description: Read CRA report data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/plaid-plaid-api-openapi.yml\n- scope: user:write\n  description: Write user data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/plaid-plaid-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plaid/refs/heads/main/scopes/plaid-scopes.yml
summary_line: 5 scopes · authorizationCode/clientCredentials
tags:
- Finance
- Fintech
- Open Banking
- Bank Accounts
- Data Aggregation
- Payments
- United States
token_bound: false
token_urls:
- https://www.your-organization.com/token
- https://api.plaid.com/oauth2/apiv2/token
---
