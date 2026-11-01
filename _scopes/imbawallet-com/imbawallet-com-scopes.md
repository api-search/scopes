---
api_specs:
- filename: imbawallet-com-auth-api-openapi.yml
  format: yaml
  label: imbawallet-com Auth API
  slug: imbawallet-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-auth-api-openapi.yml
- filename: imbawallet-com-balance-api-openapi.yml
  format: yaml
  label: imbawallet-com Balance API
  slug: imbawallet-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-balance-api-openapi.yml
- filename: imbawallet-com-cards-api-openapi.yml
  format: yaml
  label: imbawallet-com Cards API
  slug: imbawallet-com-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-cards-api-openapi.yml
- filename: imbawallet-com-catalog-api-openapi.yml
  format: yaml
  label: imbawallet-com Catalog API
  slug: imbawallet-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-catalog-api-openapi.yml
- filename: imbawallet-com-deposit-api-openapi.yml
  format: yaml
  label: imbawallet-com Deposit API
  slug: imbawallet-com-deposit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-deposit-api-openapi.yml
- filename: imbawallet-com-withdrawals-api-openapi.yml
  format: yaml
  label: imbawallet-com Withdrawals API
  slug: imbawallet-com-withdrawals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imbawallet-com/openapi/imbawallet-com-withdrawals-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Imbawallet Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'imbawallet-com publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the imbawallet-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: imbawallet-com
provider_slug: imbawallet-com
schemes: []
scope_count: 16
scope_names:
- balance:read
- deposit_address:read
- withdraw
- cards:issue
- cards:read
- cards:topup
- cards:freeze
- esim:*
- gift:read
- gift:purchase
- gift:*
- reconciliation:read
- document:read
- kyt:read
- kyt:check
- kyt:*
scopes:
- description: Partner balance
  flows: []
  scope: balance:read
- description: Sticky deposit address
  flows: []
  scope: deposit_address:read
- description: Create withdrawals
  flows: []
  scope: withdraw
- description: Issue cards
  flows: []
  scope: cards:issue
- description: Read cards, card balance, billing address, and authorization history
  flows: []
  scope: cards:read
- description: Top up cards
  flows: []
  scope: cards:topup
- description: Freeze and unfreeze cards (unfreeze only if you or the cardholder froze the card)
  flows: []
  scope: cards:freeze
- description: eSIM catalog + purchase + get
  flows: []
  scope: esim:*
- description: Gift catalog + get
  flows: []
  scope: gift:read
- description: Buy gift cards
  flows: []
  scope: gift:purchase
- description: Gift super-scope
  flows: []
  scope: gift:*
- description: Ledger reconciliation
  flows: []
  scope: reconciliation:read
- description: Document by ext_id
  flows: []
  scope: document:read
- description: KYT quote, owned check lookup, and history
  flows: []
  scope: kyt:read
- description: Create a paid crypto-address screening
  flows: []
  scope: kyt:check
- description: Both KYT scopes
  flows: []
  scope: kyt:*
slug: imbawallet-com-scopes
source_filename: imbawallet-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://api-docs.imbawallet.com/guides/authentication.md\nscopes:\n  - name: balance:read\n    description: Partner balance\n  - name: deposit_address:read\n    description: Sticky deposit address\n  - name: withdraw\n    description: Create withdrawals\n  - name: cards:issue\n    description: Issue cards\n  - name: cards:read\n    description: Read cards, card balance, billing address, and authorization history\n  - name: cards:topup\n    description: Top up cards\n  - name: cards:freeze\n    description: Freeze and unfreeze cards (unfreeze only if you or the cardholder froze the card)\n  - name: esim:*\n    description: eSIM catalog + purchase + get\n  - name: gift:read\n    description: Gift catalog + get\n  - name: gift:purchase\n    description: Buy gift cards\n  - name: gift:*\n    description: Gift super-scope\n  - name: reconciliation:read\n    description: Ledger reconciliation\n  - name: document:read\n    description:\
  \ Document by ext_id\n  - name: kyt:read\n    description: KYT quote, owned check lookup, and history\n  - name: kyt:check\n    description: Create a paid crypto-address screening\n  - name: kyt:*\n    description: Both KYT scopes\n"
source_yaml_url: https://artifacts.apis.io/imbawallet-com/scopes/imbawallet-com-scopes.yml
summary_line: 16 scopes
tags:
- FinTech
- Payments
- Cryptocurrency
- VirtualCards
- Wallet
token_bound: false
token_urls: []
---
