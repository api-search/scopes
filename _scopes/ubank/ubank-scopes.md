---
api_specs:
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Product Reference Data API
  slug: ubank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Banking Product Detail API
  slug: ubank-cdr-product-detail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Accounts & Balances API
  slug: ubank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Transactions API
  slug: ubank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Direct Debits & Scheduled Payments API
  slug: ubank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
- filename: ubank-cds-banking-products-openapi.yml
  format: yaml
  label: ubank CDR Payees API
  slug: ubank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/openapi/ubank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://cdr-support.zendesk.com/hc/en-us/articles/6402872869135-Authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ubank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ubank publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ubank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ubank
provider_slug: ubank
schemes:
- grant: authorization_code (with PAR + PKCE, request object, FAPI 1.0 Advanced)
  name: CDR-FAPI-OIDC
  source: DSB Consumer Data Standards security profile
  type: openIdConnect
scope_count: 9
scope_names:
- openid
- profile
- common:customer.basic:read
- common:customer.detail:read
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: OIDC base scope required for the CDR authorisation code flow.
  flows: []
  scope: openid
- description: OIDC profile scope requested as part of the CDR consent flow.
  flows: []
  scope: profile
- description: Read the consumer's basic customer/contact details (name, occupation for individuals; organisation basics for businesses).
  flows: []
  scope: common:customer.basic:read
- description: Read the consumer's detailed customer/contact details (phone, email, residential/mailing address; extended organisation details).
  flows: []
  scope: common:customer.detail:read
- description: Read the list of accounts and basic account attributes and balances.
  flows: []
  scope: bank:accounts.basic:read
- description: Read the full detail for a single account (rates, features, fees, terms, account numbers).
  flows: []
  scope: bank:accounts.detail:read
- description: Read transactions for the consumer's authorised accounts, including transaction detail.
  flows: []
  scope: bank:transactions:read
- description: Read the consumer's saved payees and payee detail.
  flows: []
  scope: bank:payees:read
- description: Read the consumer's authorised direct debits and scheduled/recurring payments.
  flows: []
  scope: bank:regular_payments:read
slug: ubank-scopes
source_filename: ubank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  DSB Consumer Data Standards security profile (authorisation scopes) and the CDR\n  Support authorisation-scopes reference. ubank's harvested OpenAPI declares no\n  securitySchemes because the two operations it exposes publicly are the\n  unauthenticated Product Reference Data endpoints; the authenticated CDR\n  consumer-data surface (accounts, balances, transactions, direct debits,\n  scheduled payments, payees) is authorised only to Accredited Data Recipients\n  (ADRs) under the CDR OAuth2/OpenID Connect (FAPI) model, using the standardised\n  CDS authorisation scopes below. These scopes are defined by the Data Standards\n  Body, not by ubank; every AU banking data holder (including ubank under NAB)\n  implements the same scope set.\ndocs: https://cdr-support.zendesk.com/hc/en-us/articles/6402872869135-Authorisation-scopes\nsecurity_profile: FAPI (Financial-grade API) over CDR OAuth2 / OpenID Connect\npublic_surface_note:\
  \ >-\n  The public Product Reference Data endpoints (listBankingProducts,\n  getBankingProductDetail) require NO scope and NO token - they are open and\n  unauthenticated. Scopes apply only to the consumer-authorised data-sharing\n  surface reached by an ADR after consent.\nschemes:\n- name: CDR-FAPI-OIDC\n  type: openIdConnect\n  grant: authorization_code (with PAR + PKCE, request object, FAPI 1.0 Advanced)\n  source: DSB Consumer Data Standards security profile\nscopes:\n- scope: openid\n  description: OIDC base scope required for the CDR authorisation code flow.\n  category: identity\n- scope: profile\n  description: OIDC profile scope requested as part of the CDR consent flow.\n  category: identity\n- scope: common:customer.basic:read\n  description: >-\n    Read the consumer's basic customer/contact details (name, occupation for\n    individuals; organisation basics for businesses).\n  category: common\n- scope: common:customer.detail:read\n  description: >-\n    Read the consumer's\
  \ detailed customer/contact details (phone, email,\n    residential/mailing address; extended organisation details).\n  category: common\n- scope: bank:accounts.basic:read\n  description: >-\n    Read the list of accounts and basic account attributes and balances.\n  category: banking\n  applies_to: [listBankingAccounts, listBankingBalancesBulk, listBankingBalancesSpecificAccounts, getBankingBalance]\n- scope: bank:accounts.detail:read\n  description: >-\n    Read the full detail for a single account (rates, features, fees, terms,\n    account numbers).\n  category: banking\n  applies_to: [getBankingAccountDetail]\n- scope: bank:transactions:read\n  description: >-\n    Read transactions for the consumer's authorised accounts, including\n    transaction detail.\n  category: banking\n  applies_to: [listBankingTransactions, getBankingTransactionDetail]\n- scope: bank:payees:read\n  description: Read the consumer's saved payees and payee detail.\n  category: banking\n  applies_to: [listBankingPayees,\
  \ getBankingPayeeDetail]\n- scope: bank:regular_payments:read\n  description: >-\n    Read the consumer's authorised direct debits and scheduled/recurring\n    payments.\n  category: banking\n  applies_to: [listDirectDebits, listDirectDebitsBulk, listDirectDebitsSpecificAccounts, listScheduledPayments, listScheduledPaymentsBulk, listScheduledPaymentsSpecificAccounts]\nnotes:\n- >-\n    Per CDS data-minimisation rules an ADR must request the matching basic scope\n    whenever it requests a detail scope; detailed account authorisation is only\n    meaningful when bank:accounts.basic:read is also authorised.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubank/refs/heads/main/scopes/ubank-scopes.yml
summary_line: 9 scopes
tags:
- Financial
- Banks
- Banking
- Open Banking
- CDR
- Consumer Data Right
- Product Reference Data
- Digital Bank
- Consumer Banking
- Australia
token_urls: []
---
