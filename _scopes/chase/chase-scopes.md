---
authorization_urls:
- https://api.chase.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Chase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Chase publishes 11 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chase API on a user''s behalf.


  Tokens are issued from https://api.chase.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chase
provider_slug: chase
schemes:
- flows:
  - authorizationUrl: https://api.chase.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-account-aggregation-user-consent-api-openapi.yml
- flows:
  - authorizationUrl: https://api.chase.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-account-and-customer-information-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.chase.com/oauth2/token
  name: oauth2
  source: openapi/chase-rewards-balance-api-openapi.yml
scope_count: 11
scope_names:
- accounts.read
- consents.read
- consents.write
- customers.read
- enrollments.write
- merchants.write
- orders.write
- rewards.read
- statements.read
- tax-forms.read
- transactions.read
scopes:
- description: Read account data
  flows:
  - authorizationCode
  scope: accounts.read
- description: Read consents
  flows:
  - authorizationCode
  scope: consents.read
- description: Manage consents
  flows:
  - authorizationCode
  scope: consents.write
- description: Read customer profile
  flows:
  - authorizationCode
  scope: customers.read
- description: Manage enrollments
  flows:
  - clientCredentials
  scope: enrollments.write
- description: Manage merchants
  flows:
  - clientCredentials
  scope: merchants.write
- description: Create and modify orders
  flows:
  - clientCredentials
  scope: orders.write
- description: Read rewards balances
  flows:
  - clientCredentials
  scope: rewards.read
- description: Read statements
  flows:
  - authorizationCode
  scope: statements.read
- description: Read tax forms
  flows:
  - authorizationCode
  scope: tax-forms.read
- description: Read transactions
  flows:
  - authorizationCode
  scope: transactions.read
slug: chase-scopes
source_filename: chase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chase-account-aggregation-user-consent-api-openapi.yml, openapi/chase-account-and-customer-information-api-openapi.yml,\n  openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml, openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml,\n  openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml, openapi/chase-rewards-balance-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/chase-account-aggregation-user-consent-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chase.com/oauth2/authorize\n    tokenUrl: https://api.chase.com/oauth2/token\n- name: oauth2\n  source: openapi/chase-account-and-customer-information-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chase.com/oauth2/authorize\n    tokenUrl: https://api.chase.com/oauth2/token\n- name: oauth2\n  source: openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.chase.com/oauth2/token\n- name: oauth2\n  source: openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.chase.com/oauth2/token\n- name: oauth2\n  source: openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.chase.com/oauth2/token\n- name: oauth2\n  source: openapi/chase-rewards-balance-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.chase.com/oauth2/token\nscopes:\n- scope: accounts.read\n  description: Read account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n- scope: consents.read\n  description: Read consents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-aggregation-user-consent-api-openapi.yml\n- scope: consents.write\n  description:\
  \ Manage consents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-aggregation-user-consent-api-openapi.yml\n- scope: customers.read\n  description: Read customer profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n- scope: enrollments.write\n  description: Manage enrollments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/chase-loyalty-pay-with-points-enrollment-service-api-openapi.yml\n- scope: merchants.write\n  description: Manage merchants\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/chase-loyalty-pci-merchant-relationship-manager-api-openapi.yml\n- scope: orders.write\n  description: Create and modify orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/chase-loyalty-pay-with-points-order-service-api-openapi.yml\n- scope: rewards.read\n  description: Read rewards balances\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/chase-rewards-balance-api-openapi.yml\n\
  - scope: statements.read\n  description: Read statements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n- scope: tax-forms.read\n  description: Read tax forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n- scope: transactions.read\n  description: Read transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chase-account-and-customer-information-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chase/refs/heads/main/scopes/chase-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials
tags:
- Account Aggregation
- Banking
- Consent
- Credit Cards
- FDX
- Financial Services
- Loyalty
- Open Banking
- Pay with Points
- Rewards
token_urls:
- https://api.chase.com/oauth2/token
---
