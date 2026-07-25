---
api_specs:
- filename: unit-applications-openapi.json
  format: json
  label: Unit Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-applications-openapi.json
- filename: unit-customers-openapi.json
  format: json
  label: Unit Customers API
  slug: customers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-customers-openapi.json
- filename: unit-accounts-openapi.json
  format: json
  label: Unit Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-accounts-openapi.json
- filename: unit-cards-openapi.json
  format: json
  label: Unit Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-cards-openapi.json
- filename: unit-payments-openapi.json
  format: json
  label: Unit Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-payments-openapi.json
- filename: unit-checks-openapi.json
  format: json
  label: Unit Checks API
  slug: checks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-checks-openapi.json
- filename: unit-authorizations-openapi.json
  format: json
  label: Unit Card Authorizations API
  slug: authorizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-authorizations-openapi.json
- filename: unit-disputes-openapi.json
  format: json
  label: Unit Disputes API
  slug: disputes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-disputes-openapi.json
- filename: unit-transactions-openapi.json
  format: json
  label: Unit Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-transactions-openapi.json
- filename: unit-statements-openapi.json
  format: json
  label: Unit Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-statements-openapi.json
- filename: unit-tax-forms-openapi.json
  format: json
  label: Unit Tax Forms API
  slug: tax-forms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-tax-forms-openapi.json
- filename: unit-fees-rewards-openapi.json
  format: json
  label: Unit Fees and Rewards API
  slug: fees-rewards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-fees-rewards-openapi.json
- filename: unit-credit-openapi.json
  format: json
  label: Unit Credit and Repayments API
  slug: credit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-credit-openapi.json
- filename: unit-stop-payments-openapi.json
  format: json
  label: Unit Stop Payments API
  slug: stop-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-stop-payments-openapi.json
- filename: unit-webhooks-openapi.json
  format: json
  label: Unit Webhooks and Events API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-webhooks-openapi.json
- filename: unit-sandbox-openapi.json
  format: json
  label: Unit Sandbox and Reference API
  slug: sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/openapi/unit-sandbox-openapi.json
authorization_urls: []
description: ''
docs: https://www.unit.co/docs/api/using-the-api#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Unit Scopes
name_suffix: OAuth Scopes
note: Unit authenticates with OAuth 2.0 Bearer tokens (Org API tokens and short-lived Customer tokens). Each token is minted with a set of scopes granting read/write access per resource. The OpenAPI declares the transport as http bearer (JWT); the scope catalog below is documented in the "Scopes" section of the docs, not in the spec's securitySchemes. Fund-movement and PCI-sensitive scopes require Two-Factor Authentication (OTP) within the prior 24 hours; Customer tokens execute the 2FA for you.
overview: 'Unit publishes 46 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Unit API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Unit
provider_slug: unit
schemes: []
scope_count: 46
scope_names:
- applications
- applications-write
- customer-token
- customer-token-write
- customers
- customers-write
- customer-tags-write
- accounts
- accounts-write
- cards
- cards-write
- cards-sensitive
- cards-sensitive-write
- transactions
- transactions-write
- authorizations
- statements
- payments
- payments-write
- payments-write-counterparty
- payments-write-linked-account
- payments-write-ach-debit
- ach-payments-write
- wire-payments-write
- counterparties
- counterparties-write
- events
- events-write
- webhooks
- webhooks-write
- authorization-requests
- authorization-requests-write
- batch-releases
- batch-releases-write
- check-deposits
- check-deposits-write
- check-payments
- check-payments-write
- received-payments
- received-payments-write
- chargebacks
- chargebacks-write
- rewards
- rewards-write
- wire-drawdowns
- wire-drawdowns-write
scopes:
- description: ''
  flows: []
  scope: applications
- description: ''
  flows: []
  scope: applications-write
- description: ''
  flows: []
  scope: customer-token
- description: ''
  flows: []
  scope: customer-token-write
- description: ''
  flows: []
  scope: customers
- description: ''
  flows: []
  scope: customers-write
- description: ''
  flows: []
  scope: customer-tags-write
- description: ''
  flows: []
  scope: accounts
- description: ''
  flows: []
  scope: accounts-write
- description: ''
  flows: []
  scope: cards
- description: ''
  flows: []
  scope: cards-write
- description: ''
  flows: []
  scope: cards-sensitive
- description: ''
  flows: []
  scope: cards-sensitive-write
- description: ''
  flows: []
  scope: transactions
- description: ''
  flows: []
  scope: transactions-write
- description: ''
  flows: []
  scope: authorizations
- description: ''
  flows: []
  scope: statements
- description: ''
  flows: []
  scope: payments
- description: ''
  flows: []
  scope: payments-write
- description: ''
  flows: []
  scope: payments-write-counterparty
- description: ''
  flows: []
  scope: payments-write-linked-account
- description: ''
  flows: []
  scope: payments-write-ach-debit
- description: ''
  flows: []
  scope: ach-payments-write
- description: ''
  flows: []
  scope: wire-payments-write
- description: ''
  flows: []
  scope: counterparties
- description: ''
  flows: []
  scope: counterparties-write
- description: ''
  flows: []
  scope: events
- description: ''
  flows: []
  scope: events-write
- description: ''
  flows: []
  scope: webhooks
- description: ''
  flows: []
  scope: webhooks-write
- description: ''
  flows: []
  scope: authorization-requests
- description: ''
  flows: []
  scope: authorization-requests-write
- description: ''
  flows: []
  scope: batch-releases
- description: ''
  flows: []
  scope: batch-releases-write
- description: ''
  flows: []
  scope: check-deposits
- description: ''
  flows: []
  scope: check-deposits-write
- description: ''
  flows: []
  scope: check-payments
- description: ''
  flows: []
  scope: check-payments-write
- description: ''
  flows: []
  scope: received-payments
- description: ''
  flows: []
  scope: received-payments-write
- description: ''
  flows: []
  scope: chargebacks
- description: ''
  flows: []
  scope: chargebacks-write
- description: ''
  flows: []
  scope: rewards
- description: ''
  flows: []
  scope: rewards-write
- description: ''
  flows: []
  scope: wire-drawdowns
- description: ''
  flows: []
  scope: wire-drawdowns-write
slug: unit-scopes
source_filename: unit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://www.unit.co/docs/api/using-the-api\ndocs: https://www.unit.co/docs/api/using-the-api#scopes\nnote: >-\n  Unit authenticates with OAuth 2.0 Bearer tokens (Org API tokens and short-lived\n  Customer tokens). Each token is minted with a set of scopes granting read/write\n  access per resource. The OpenAPI declares the transport as http bearer (JWT); the\n  scope catalog below is documented in the \"Scopes\" section of the docs, not in the\n  spec's securitySchemes. Fund-movement and PCI-sensitive scopes require Two-Factor\n  Authentication (OTP) within the prior 24 hours; Customer tokens execute the 2FA for you.\ntoken_types:\n  - name: Org API token\n    role: org\n    description: Broad, system-level token not restricted to a specific end customer.\n  - name: Customer token\n    role: customer\n    description: >-\n      End-customer specific, scoped to a single customer's resources, with built-in\n      OTP 2FA and\
  \ a customizable expiry up to 24 hours. Required for PCI-sensitive\n      card data/actions unless the client is PCI Level 1 compliant.\nscopes:\n  - {scope: applications, access: read, resource: Application, accessible_using: [org]}\n  - {scope: applications-write, access: write, resource: Application, accessible_using: [org]}\n  - {scope: customer-token, access: read, resource: Customer Token, accessible_using: [org]}\n  - {scope: customer-token-write, access: write, resource: Customer Token, accessible_using: [org]}\n  - {scope: customers, access: read, resource: Customers, accessible_using: [org, customer]}\n  - {scope: customers-write, access: write, resource: Customers, accessible_using: [org, customer]}\n  - {scope: customer-tags-write, access: write, resource: Customer Tags, accessible_using: [org, customer]}\n  - {scope: accounts, access: read, resource: Accounts, accessible_using: [org, customer]}\n  - {scope: accounts-write, access: write, resource: Accounts, accessible_using:\
  \ [org, customer], note: \"Close Account requires Org API token\"}\n  - {scope: cards, access: read, resource: Cards, accessible_using: [org, customer]}\n  - {scope: cards-write, access: write, resource: Cards, accessible_using: [org, customer]}\n  - {scope: cards-sensitive, access: read, resource: Cards Sensitive, accessible_using: [customer], sensitive: pci}\n  - {scope: cards-sensitive-write, access: write, resource: Cards Sensitive, accessible_using: [customer], sensitive: pci}\n  - {scope: transactions, access: read, resource: Transactions, accessible_using: [org, customer]}\n  - {scope: transactions-write, access: write, resource: Transactions, accessible_using: [org, customer]}\n  - {scope: authorizations, access: read, resource: Authorizations, accessible_using: [org, customer]}\n  - {scope: statements, access: read, resource: Statements, accessible_using: [org, customer]}\n  - {scope: payments, access: read, resource: Payments, accessible_using: [org, customer]}\n  - {scope: payments-write,\
  \ access: write, resource: Payments, accessible_using: [org, customer], sensitive: funds}\n  - {scope: payments-write-counterparty, access: write, resource: Payments to a counterparty, accessible_using: [org, customer], sensitive: funds}\n  - {scope: payments-write-linked-account, access: write, resource: Payments to a linked account, accessible_using: [org, customer], sensitive: funds}\n  - {scope: payments-write-ach-debit, access: write, resource: Payments ACH Debit, accessible_using: [org, customer], sensitive: funds}\n  - {scope: ach-payments-write, access: write, resource: Payments ACH, accessible_using: [org, customer], sensitive: funds}\n  - {scope: wire-payments-write, access: write, resource: Payments Wire, accessible_using: [org, customer], sensitive: funds}\n  - {scope: counterparties, access: read, resource: Counterparties, accessible_using: [org, customer]}\n  - {scope: counterparties-write, access: write, resource: Counterparties, accessible_using: [org, customer]}\n  - {scope:\
  \ events, access: read, resource: Events, accessible_using: [org, customer]}\n  - {scope: events-write, access: write, resource: Events, accessible_using: [org, customer]}\n  - {scope: webhooks, access: read, resource: Webhooks, accessible_using: [org]}\n  - {scope: webhooks-write, access: write, resource: Webhooks, accessible_using: [org]}\n  - {scope: authorization-requests, access: read, resource: Authorization Requests, accessible_using: [org]}\n  - {scope: authorization-requests-write, access: write, resource: Authorization Requests, accessible_using: [org]}\n  - {scope: batch-releases, access: read, resource: Batch Releases, accessible_using: [org]}\n  - {scope: batch-releases-write, access: write, resource: Batch Releases, accessible_using: [org]}\n  - {scope: check-deposits, access: read, resource: Check Deposits, accessible_using: [org, customer]}\n  - {scope: check-deposits-write, access: write, resource: Check Deposits, accessible_using: [org, customer]}\n  - {scope: check-payments,\
  \ access: read, resource: Check Payments, accessible_using: [org, customer]}\n  - {scope: check-payments-write, access: write, resource: Check Payments, accessible_using: [org, customer]}\n  - {scope: received-payments, access: read, resource: Received Payment, accessible_using: [org]}\n  - {scope: received-payments-write, access: write, resource: Received Payment, accessible_using: [org]}\n  - {scope: chargebacks, access: read, resource: Chargeback, accessible_using: [org]}\n  - {scope: chargebacks-write, access: write, resource: Chargeback, accessible_using: [org]}\n  - {scope: rewards, access: read, resource: Reward, accessible_using: [org]}\n  - {scope: rewards-write, access: write, resource: Reward, accessible_using: [org]}\n  - {scope: wire-drawdowns, access: read, resource: Wire Drawdowns, accessible_using: [org, customer]}\n  - {scope: wire-drawdowns-write, access: write, resource: Wire Drawdowns, accessible_using: [org, customer]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit/refs/heads/main/scopes/unit-scopes.yml
summary_line: 46 scopes
tags:
- FinTech
- BaaS
- Banking
- Payments
- Card Issuing
- ACH
- United States
- Embedded Finance
- Deposit Accounts
- Open Finance
token_urls: []
---
