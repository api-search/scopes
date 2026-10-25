---
api_specs:
- filename: anz-banking-account-balances-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Balances API
  slug: anz-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-balances-api-openapi.yml
- filename: anz-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Direct Debits API
  slug: anz-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-direct-debits-api-openapi.yml
- filename: anz-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Scheduled Payments API
  slug: anz-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-scheduled-payments-api-openapi.yml
- filename: anz-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Account Transactions API
  slug: anz-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-account-transactions-api-openapi.yml
- filename: anz-banking-accounts-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Accounts API
  slug: anz-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-accounts-api-openapi.yml
- filename: anz-banking-payees-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Payees API
  slug: anz-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-payees-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) Banking Products API
  slug: anz-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
- filename: anz-banking-products-api-openapi.yml
  format: yaml
  label: Australia and New Zealand Banking Group (ANZ) ANZ Plus Banking Products API
  slug: anz-plus-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/openapi/anz-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Anz Scopes
name_suffix: OAuth Scopes
note: The public ANZ Product Reference Data endpoints require NO OAuth scope (they are unauthenticated). The scopes below govern the CDR consumer-data-sharing operations in the shared DSB Consumer Data Standards banking contract, which ANZ exposes only to CDR-accredited Data Recipients under consumer consent. Scope strings are captured verbatim from the spec's per-operation x-scopes extension and the Consumer Data Standards authorisation-scopes reference.
overview: 'Australia and New Zealand Banking Group (ANZ) publishes 34 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Australia and New Zealand Banking Group (ANZ) API on a user''s behalf.


  Tokens are issued from https://api.fileactive.anz.com/auth/v2/oauth2/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Australia and New Zealand Banking Group (ANZ)
provider_slug: anz
schemes:
- flows:
  - flow: authorizationCode
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced
  source: openapi/anz-cds-banking-products-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.fileactive.anz.com/auth/v2/oauth2/access_token
  name: Fileactive-OAuth2
  source: https://developer.online.anz.com/product/PayTo/build (embedded OpenAPI securitySchemes)
scope_count: 34
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
- AU.INSTO.PAYTO.MANDATE.WRITE
- AU.INSTO.PAYTO.MANDATE.READ
- AU.INSTO.PAYTO.MPIR.WRITE
- AU.INSTO.ACCOUNT.CHECK
- AU.INSTO.NPP.PAYID.READ
- GBL.INSTO.FX.RFQ
- GBL.INSTO.ACCOUNTS.STATEMENT.READ
- AU.INSTO.PAYMENT.NPP.CREATE
- AU.INSTO.PAYMENT.NPP.RETURN
- AU.INSTO.PAYMENT.NPP.READ
- AU.INSTO.PAYMENT.CBFT.CREATE
- AU.INSTO.PAYMENT.READ
- HK.INSTO.PAYMENT.FAST.CREATE
- HK.INSTO.PAYMENT.ACH.CREATE
- HK.INSTO.PAYMENT.CBFT.CREATE
- HK.INSTO.PAYMENT.RTGS.CREATE
- HK.INSTO.PAYMENT.READ
- IN.INSTO.PAYMENT.ACH.CREATE
- IN.INSTO.PAYMENT.READ
- SG.INSTO.PAYMENT.ACH.CREATE
- SG.INSTO.PAYMENT.CBFT.CREATE
- SG.INSTO.PAYMENT.FAST.CREATE
- SG.INSTO.PAYMENT.RTGS.CREATE
- SG.INSTO.PAYMENT.READ
- VN.INSTO.PAYMENT.ACH.CREATE
- VN.INSTO.PAYMENT.READ
- AU.INSTO.TESTING.NPP.RTN.CREATE
- AU.INSTO.TESTING.PAYTO.NOTIFICATION.CREATE
- AU.INSTO.TESTING.PAYTO.QUERY.CREATE
scopes:
- description: Read basic account information (account list, masked numbers, product category).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers and features.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read direct debits, scheduled payments and recurring/instalment payment arrangements.
  flows: []
  scope: bank:regular_payments:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: ''
  flows: []
  scope: AU.INSTO.PAYTO.MANDATE.WRITE
- description: ''
  flows: []
  scope: AU.INSTO.PAYTO.MANDATE.READ
- description: ''
  flows: []
  scope: AU.INSTO.PAYTO.MPIR.WRITE
- description: ''
  flows: []
  scope: AU.INSTO.ACCOUNT.CHECK
- description: ''
  flows: []
  scope: AU.INSTO.NPP.PAYID.READ
- description: ''
  flows: []
  scope: GBL.INSTO.FX.RFQ
- description: ''
  flows: []
  scope: GBL.INSTO.ACCOUNTS.STATEMENT.READ
- description: ''
  flows: []
  scope: AU.INSTO.PAYMENT.NPP.CREATE
- description: ''
  flows: []
  scope: AU.INSTO.PAYMENT.NPP.RETURN
- description: ''
  flows: []
  scope: AU.INSTO.PAYMENT.NPP.READ
- description: ''
  flows: []
  scope: AU.INSTO.PAYMENT.CBFT.CREATE
- description: ''
  flows: []
  scope: AU.INSTO.PAYMENT.READ
- description: ''
  flows: []
  scope: HK.INSTO.PAYMENT.FAST.CREATE
- description: ''
  flows: []
  scope: HK.INSTO.PAYMENT.ACH.CREATE
- description: ''
  flows: []
  scope: HK.INSTO.PAYMENT.CBFT.CREATE
- description: ''
  flows: []
  scope: HK.INSTO.PAYMENT.RTGS.CREATE
- description: ''
  flows: []
  scope: HK.INSTO.PAYMENT.READ
- description: ''
  flows: []
  scope: IN.INSTO.PAYMENT.ACH.CREATE
- description: ''
  flows: []
  scope: IN.INSTO.PAYMENT.READ
- description: ''
  flows: []
  scope: SG.INSTO.PAYMENT.ACH.CREATE
- description: ''
  flows: []
  scope: SG.INSTO.PAYMENT.CBFT.CREATE
- description: ''
  flows: []
  scope: SG.INSTO.PAYMENT.FAST.CREATE
- description: ''
  flows: []
  scope: SG.INSTO.PAYMENT.RTGS.CREATE
- description: ''
  flows: []
  scope: SG.INSTO.PAYMENT.READ
- description: ''
  flows: []
  scope: VN.INSTO.PAYMENT.ACH.CREATE
- description: ''
  flows: []
  scope: VN.INSTO.PAYMENT.READ
- description: ''
  flows: []
  scope: AU.INSTO.TESTING.NPP.RTN.CREATE
- description: ''
  flows: []
  scope: AU.INSTO.TESTING.PAYTO.NOTIFICATION.CREATE
- description: ''
  flows: []
  scope: AU.INSTO.TESTING.PAYTO.QUERY.CREATE
slug: anz-scopes
source_filename: anz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: openapi/anz-cds-banking-products-openapi.yml (x-scopes extension)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: 'The public ANZ Product Reference Data endpoints require NO OAuth scope (they are unauthenticated). The scopes\n  below govern the CDR consumer-data-sharing operations in the shared DSB Consumer Data Standards banking contract,\n  which ANZ exposes only to CDR-accredited Data Recipients under consumer consent. Scope strings are captured verbatim\n  from the spec''s per-operation x-scopes extension and the Consumer Data Standards authorisation-scopes reference.\n\n  '\nschemes:\n- name: CDR-FAPI-OAuth2\n  profile: FAPI 1.0 Advanced\n  source: openapi/anz-cds-banking-products-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: Fileactive-OAuth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.fileactive.anz.com/auth/v2/oauth2/access_token\n  source:\
  \ https://developer.online.anz.com/product/PayTo/build (embedded OpenAPI securitySchemes)\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list, masked numbers, product category).\n  operations:\n  - listBankingAccounts\n  - listBankingBalancesBulk\n  - listBankingBalancesSpecificAccounts\n  - getBankingBalance\n- scope: bank:accounts.detail:read\n  description: Read detailed account information including account numbers and features.\n  operations:\n  - getBankingAccountDetail\n- scope: bank:transactions:read\n  description: Read account transactions.\n  operations:\n  - listBankingTransactions\n  - getBankingTransactionDetail\n- scope: bank:regular_payments:read\n  description: Read direct debits, scheduled payments and recurring/instalment payment arrangements.\n  operations:\n  - listDirectDebits\n  - listDirectDebitsBulk\n  - listDirectDebitsSpecificAccounts\n  - listScheduledPayments\n  - listScheduledPaymentsBulk\n  - listScheduledPaymentsSpecificAccounts\n\
  \  - listInstalmentPlans\n  - listInstalmentPlansBulk\n- scope: bank:payees:read\n  description: Read saved payees.\n  operations:\n  - listBankingPayees\n  - getBankingPayeeDetail\n- scope: AU.INSTO.PAYTO.MANDATE.WRITE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n  operations:\n  - amendMandate\n  - changeMandateStatus\n  - createMandate\n  - recallMandateAction\n- scope: AU.INSTO.PAYTO.MANDATE.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n  operations:\n  - getMandate\n  - getMandateActions\n  - getMandateList\n  - queryResolution\n- scope: AU.INSTO.PAYTO.MPIR.WRITE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n  operations:\n  - createMPIR\n  - retryMPIR\n- scope: AU.INSTO.ACCOUNT.CHECK\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com\
  \ product Build pages\n  operations:\n  - checkAccountName\n- scope: AU.INSTO.NPP.PAYID.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n  operations:\n  - checkPayID\n- scope: GBL.INSTO.FX.RFQ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: GBL.INSTO.ACCOUNTS.STATEMENT.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.PAYMENT.NPP.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.PAYMENT.NPP.RETURN\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.PAYMENT.NPP.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n-\
  \ scope: AU.INSTO.PAYMENT.CBFT.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.PAYMENT.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: HK.INSTO.PAYMENT.FAST.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: HK.INSTO.PAYMENT.ACH.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: HK.INSTO.PAYMENT.CBFT.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: HK.INSTO.PAYMENT.RTGS.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: HK.INSTO.PAYMENT.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents\
  \ embedded in developer.online.anz.com product Build pages\n- scope: IN.INSTO.PAYMENT.ACH.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: IN.INSTO.PAYMENT.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: SG.INSTO.PAYMENT.ACH.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: SG.INSTO.PAYMENT.CBFT.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: SG.INSTO.PAYMENT.FAST.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: SG.INSTO.PAYMENT.RTGS.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: SG.INSTO.PAYMENT.READ\n\
  \  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: VN.INSTO.PAYMENT.ACH.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: VN.INSTO.PAYMENT.READ\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.TESTING.NPP.RTN.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.TESTING.PAYTO.NOTIFICATION.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\n- scope: AU.INSTO.TESTING.PAYTO.QUERY.CREATE\n  scheme: Fileactive-OAuth2\n  source: OpenAPI documents embedded in developer.online.anz.com product Build pages\nfileactive_docs: https://developer.online.anz.com/How-it-works?path=FAQ\nfileactive_note: 'Developer\
  \ portal (Fileactive) scopes: \"A scope is a mechanism in OAuth 2.0 to define what an application\n  can access (such as payments) and whether the access is read or write.\" Operation lists are given only where the\n  embedded spec binds the scope per operation in a form we could parse.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anz/refs/heads/main/scopes/anz-scopes.yml
summary_line: 34 scopes · authorizationCode/clientCredentials
tags:
- Finance
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
token_bound: false
token_urls:
- https://api.fileactive.anz.com/auth/v2/oauth2/access_token
---
