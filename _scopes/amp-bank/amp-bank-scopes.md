---
api_specs:
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Product Reference Data API
  slug: amp-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank GO CDR Product Reference Data API
  slug: amp-bank-go-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Accounts & Balances API
  slug: amp-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Transactions API
  slug: amp-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Direct Debits & Scheduled Payments API
  slug: amp-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
- filename: amp-bank-cds-banking-products-openapi.yml
  format: yaml
  label: AMP Bank CDR Payees API
  slug: amp-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/openapi/amp-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Amp Bank Scopes
name_suffix: OAuth Scopes
note: Scope descriptions follow the DSB Consumer Data Standards authorisation-scopes reference. AMP Bank implements the standard CDR banking scope set; it does not define bank-proprietary scopes. The PRD product endpoints (listBankingProducts, getBankingProductDetail) require no scope.
overview: 'AMP Bank publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the AMP Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AMP Bank
provider_slug: amp-bank
schemes: []
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information (account list, masked account numbers, product category, balances) for accounts the consumer has authorised.
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information (full account number, features, terms, rates, addresses) for authorised accounts.
  flows: []
  scope: bank:accounts.detail:read
- description: Read transaction data for authorised accounts.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments and instalment plans for authorised accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Read the consumer's saved payee list for authorised accounts.
  flows: []
  scope: bank:payees:read
slug: amp-bank-scopes
source_filename: amp-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/amp-bank-cds-banking-products-openapi.yml (x-scopes per operation) + DSB Consumer Data Standards\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nsummary: >-\n  OAuth 2.0 authorisation scopes governing the accredited CDR consumer\n  data-sharing surface (accounts, balances, transactions, direct debits,\n  scheduled payments, payees). These are the standard DSB Consumer Data\n  Standards banking scopes, declared per-operation in the OpenAPI via the\n  x-scopes extension. They apply to the FAPI 1.0 Advanced / OpenID Connect\n  authorisation flow brokered by an Accredited Data Recipient (ADR) - NOT to\n  the public, unauthenticated Product Reference Data (PRD) surface, which needs\n  no scope. See authentication/amp-bank-authentication.yml for the auth profile.\nflow:\n  grant: authorization_code (FAPI 1.0 Advanced, OIDC, PAR, PKCE, mTLS-bound tokens)\n  registry: CDR Register / Data\
  \ Standards Body InfoSec profile\nscopes:\n- scope: bank:accounts.basic:read\n  description: >-\n    Read basic account information (account list, masked account numbers,\n    product category, balances) for accounts the consumer has authorised.\n  operations:\n  - listBankingAccounts\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n  - getBankingBalance\n- scope: bank:accounts.detail:read\n  description: >-\n    Read detailed account information (full account number, features, terms,\n    rates, addresses) for authorised accounts.\n  operations:\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: Read transaction data for authorised accounts.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:regular_payments:read\n  description: >-\n    Read direct debits, scheduled payments and instalment plans for authorised\n    accounts.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n\
  \  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n  - listInstalmentPlans\n  - listInstalmentPlansBulk\n- scope: bank:payees:read\n  description: Read the consumer's saved payee list for authorised accounts.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\nnote: >-\n  Scope descriptions follow the DSB Consumer Data Standards authorisation-scopes\n  reference. AMP Bank implements the standard CDR banking scope set; it does not\n  define bank-proprietary scopes. The PRD product endpoints (listBankingProducts,\n  getBankingProductDetail) require no scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp-bank/refs/heads/main/scopes/amp-bank-scopes.yml
summary_line: 5 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
token_urls: []
---
