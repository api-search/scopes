---
api_specs:
- filename: td-bank-account-basic-api-openapi.yml
  format: yaml
  label: TD Bank Account Basic API
  slug: account-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-account-basic-api-openapi.yml
- filename: td-bank-account-detailed-api-openapi.yml
  format: yaml
  label: TD Bank Account Detailed API
  slug: account-detailed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-account-detailed-api-openapi.yml
- filename: td-bank-customer-api-openapi.yml
  format: yaml
  label: TD Bank Customer API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-customer-api-openapi.yml
- filename: td-bank-transactions-api-openapi.yml
  format: yaml
  label: TD Bank Transactions API
  slug: transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-transactions-api-openapi.yml
- filename: td-bank-statements-api-openapi.yml
  format: yaml
  label: TD Bank Statements API
  slug: statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-statements-api-openapi.yml
- filename: td-bank-tax-forms-api-openapi.yml
  format: yaml
  label: TD Bank Tax Forms API
  slug: tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-tax-forms-api-openapi.yml
- filename: td-bank-bill-payment-api-openapi.yml
  format: yaml
  label: TD Bank Bill Payment API
  slug: bill-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-bill-payment-api-openapi.yml
- filename: td-bank-rewards-api-openapi.yml
  format: yaml
  label: TD Bank Rewards API
  slug: rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-rewards-api-openapi.yml
- filename: td-bank-consent-api-openapi.yml
  format: yaml
  label: TD Bank Consent API
  slug: consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-consent-api-openapi.yml
- filename: td-bank-token-api-openapi.yml
  format: yaml
  label: TD Bank Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-token-api-openapi.yml
- filename: td-bank-service-token-api-openapi.yml
  format: yaml
  label: TD Bank Service Token API
  slug: service-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-service-token-api-openapi.yml
- filename: td-bank-apps-management-api-openapi.yml
  format: yaml
  label: TD Bank Apps Management API
  slug: apps-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-apps-management-api-openapi.yml
- filename: td-bank-notifications-api-openapi.yml
  format: yaml
  label: TD Bank Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-notifications-api-openapi.yml
authorization_urls:
- https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Td Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TD Bank publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TD Bank API on a user''s behalf.


  Tokens are issued from https://api.openbanking.amcb.developer.td.com/oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TD Bank
provider_slug: td-bank
schemes:
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-account-basic-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-account-detailed-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-bill-payment-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-consent-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-customer-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-rewards-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-statements-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-tax-forms-api-openapi.yml
- flows:
  - authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token
  name: oauth2
  source: openapi/td-bank-transactions-api-openapi.yml
scope_count: 9
scope_names:
- accounts_basic_read
- accounts_detailed_read
- bill_payments_read
- consents_manage
- customer_contact_read
- rewards_read
- statements_read
- tax_forms_read
- transactions_read
scopes:
- description: Read basic account info
  flows:
  - authorizationCode
  scope: accounts_basic_read
- description: Read detailed account info
  flows:
  - authorizationCode
  scope: accounts_detailed_read
- description: Read bill payment activity
  flows:
  - authorizationCode
  scope: bill_payments_read
- description: Manage consents
  flows:
  - authorizationCode
  scope: consents_manage
- description: Read customer contact
  flows:
  - authorizationCode
  scope: customer_contact_read
- description: Read rewards info
  flows:
  - authorizationCode
  scope: rewards_read
- description: Read statements
  flows:
  - authorizationCode
  scope: statements_read
- description: Read tax forms
  flows:
  - authorizationCode
  scope: tax_forms_read
- description: Read transactions
  flows:
  - authorizationCode
  scope: transactions_read
slug: td-bank-scopes
source_filename: td-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/td-bank-account-basic-api-openapi.yml, openapi/td-bank-account-detailed-api-openapi.yml,\n  openapi/td-bank-bill-payment-api-openapi.yml, openapi/td-bank-consent-api-openapi.yml, openapi/td-bank-customer-api-openapi.yml,\n  openapi/td-bank-rewards-api-openapi.yml, openapi/td-bank-statements-api-openapi.yml, openapi/td-bank-tax-forms-api-openapi.yml,\n  openapi/td-bank-transactions-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/td-bank-account-basic-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-account-detailed-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n\
  - name: oauth2\n  source: openapi/td-bank-bill-payment-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-consent-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-customer-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-rewards-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n\
  \    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-statements-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-tax-forms-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\n- name: oauth2\n  source: openapi/td-bank-transactions-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/authorize\n    tokenUrl: https://api.openbanking.amcb.developer.td.com/oauth/v1/token\nscopes:\n- scope: accounts_basic_read\n  description: Read basic account info\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/td-bank-account-basic-api-openapi.yml\n- scope: accounts_detailed_read\n  description: Read detailed account info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-account-detailed-api-openapi.yml\n- scope: bill_payments_read\n  description: Read bill payment activity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-bill-payment-api-openapi.yml\n- scope: consents_manage\n  description: Manage consents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-consent-api-openapi.yml\n- scope: customer_contact_read\n  description: Read customer contact\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-customer-api-openapi.yml\n- scope: rewards_read\n  description: Read rewards info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-rewards-api-openapi.yml\n- scope: statements_read\n  description: Read statements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-statements-api-openapi.yml\n\
  - scope: tax_forms_read\n  description: Read tax forms\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-tax-forms-api-openapi.yml\n- scope: transactions_read\n  description: Read transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/td-bank-transactions-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/scopes/td-bank-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Account Aggregation
- AML
- Akoya
- Banking
- Bank Secrecy Act
- Bill Payment
- Consent
- Consumer Banking
- FDX
- Financial Services
- Merchant Solutions
- Notifications
- Open Banking
- Payments
- Rewards
- Tax Forms
- Token Management
- Transactions
token_urls:
- https://api.openbanking.amcb.developer.td.com/oauth/v1/token
---
