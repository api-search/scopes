---
api_specs:
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Product Reference Data API
  slug: bank-of-queensland-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Accounts & Balances API
  slug: bank-of-queensland-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Transactions API
  slug: bank-of-queensland-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Direct Debits & Scheduled Payments API
  slug: bank-of-queensland-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
- filename: bank-of-queensland-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Queensland (BOQ) CDR Payees API
  slug: bank-of-queensland-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/openapi/bank-of-queensland-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bank Of Queensland Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bank of Queensland publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank of Queensland API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank of Queensland
provider_slug: bank-of-queensland
schemes:
- fapi_profile: FAPI 1.0 Advanced (Australia CDR security profile)
  flow: authorizationCode
  name: CDRAuthorizationCode
  source: docs
  type: oauth2
scope_count: 9
scope_names:
- openid
- profile
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: OpenID Connect authentication (required for the CDR authorization flow).
  flows:
  - authorizationCode
  scope: openid
- description: CDR consumer profile scope requested alongside the data scopes.
  flows:
  - authorizationCode
  scope: profile
- description: Read basic account information (account list and masked identifiers).
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account information including full account numbers and features.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read account transaction history and transaction detail.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read saved payees for the consumer's accounts.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
- description: Read basic customer information (name and contact type).
  flows:
  - authorizationCode
  scope: common:customer.basic:read
- description: Read detailed customer information including contact details.
  flows:
  - authorizationCode
  scope: common:customer.detail:read
slug: bank-of-queensland-scopes
source_filename: bank-of-queensland-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/bank-of-queensland-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\n# The harvested DSB CDS Banking contract declares no oauth2 securitySchemes, so the\n# derive pass returned empty. These authorisation scopes are the mandated Australian\n# Consumer Data Right (CDR) banking scopes that BOQ, as an accredited data holder,\n# implements verbatim. The public Product Reference Data (PRD) surface needs NO scope\n# (unauthenticated); every scope below gates the consumer-authorized data-sharing APIs\n# accessed through the CDR / Accredited Data Recipient (ADR) model (OAuth2 + OIDC/FAPI,\n# authorization_code, MTLS-bound tokens). Authorization and token endpoints are the\n# holder's per-brand CDR InfoSec endpoints discovered via OIDC (not openly published).\nschemes:\n  - name: CDRAuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    fapi_profile:\
  \ FAPI 1.0 Advanced (Australia CDR security profile)\n    source: docs\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication (required for the CDR authorization flow).\n    flows: [authorizationCode]\n  - scope: profile\n    description: CDR consumer profile scope requested alongside the data scopes.\n    flows: [authorizationCode]\n  - scope: bank:accounts.basic:read\n    description: Read basic account information (account list and masked identifiers).\n    grants: [listBankingAccounts, getBankingBalance]\n    flows: [authorizationCode]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information including full account numbers and features.\n    grants: [getBankingAccountDetail]\n    flows: [authorizationCode]\n  - scope: bank:transactions:read\n    description: Read account transaction history and transaction detail.\n    grants: [listBankingTransactions, getBankingTransactionDetail]\n    flows: [authorizationCode]\n  - scope: bank:payees:read\n\
  \    description: Read saved payees for the consumer's accounts.\n    grants: [listBankingPayees]\n    flows: [authorizationCode]\n  - scope: bank:regular_payments:read\n    description: Read direct debits and scheduled/regular payments.\n    grants: [listDirectDebits, listScheduledPayments]\n    flows: [authorizationCode]\n  - scope: common:customer.basic:read\n    description: Read basic customer information (name and contact type).\n    flows: [authorizationCode]\n  - scope: common:customer.detail:read\n    description: Read detailed customer information including contact details.\n    flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-queensland/refs/heads/main/scopes/bank-of-queensland-scopes.yml
summary_line: 9 scopes
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
