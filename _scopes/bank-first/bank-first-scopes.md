---
api_specs:
- filename: bank-first-banking-account-balances-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Balances API
  slug: bank-first-banking-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-balances-api-openapi.yml
- filename: bank-first-banking-account-direct-debits-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Direct Debits API
  slug: bank-first-banking-account-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-direct-debits-api-openapi.yml
- filename: bank-first-banking-account-scheduled-payments-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Scheduled Payments API
  slug: bank-first-banking-account-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-scheduled-payments-api-openapi.yml
- filename: bank-first-banking-account-transactions-api-openapi.yml
  format: yaml
  label: Bank First Banking Account Transactions API
  slug: bank-first-banking-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-account-transactions-api-openapi.yml
- filename: bank-first-banking-accounts-api-openapi.yml
  format: yaml
  label: Bank First Banking Accounts API
  slug: bank-first-banking-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-accounts-api-openapi.yml
- filename: bank-first-banking-payees-api-openapi.yml
  format: yaml
  label: Bank First Banking Payees API
  slug: bank-first-banking-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-payees-api-openapi.yml
- filename: bank-first-banking-products-api-openapi.yml
  format: yaml
  label: Bank First Banking Products API
  slug: bank-first-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/openapi/bank-first-banking-products-api-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bank First Scopes
name_suffix: OAuth Scopes
note: The public PRD API requires NO scopes (unauthenticated). These scopes govern the CDR consumer data sharing surface, which only Accredited Data Recipients may request via the CDR consent flow. The scope set below is the CDR banking + common scope family referenced by the x-scopes extension on the standard's operations.
overview: 'Bank First publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank First API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank First
provider_slug: bank-first
schemes:
- authorizationUrl: (per-holder, discovered via CDR Register / OIDC configuration)
  flow: authorizationCode
  name: CDR-OAuth2-OIDC
  source: openapi/bank-first-cds-banking-products-openapi.yml
  tokenUrl: (per-holder, discovered via CDR Register / OIDC configuration)
  type: oauth2
scope_count: 7
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
- common:customer.basic:read
- common:customer.detail:read
scopes:
- description: Read basic account information (masked account numbers, product category, balances context).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information including account numbers and terms.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments.
  flows: []
  scope: bank:regular_payments:read
- description: Read basic customer identity (name, organisation).
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer identity (contact details).
  flows: []
  scope: common:customer.detail:read
slug: bank-first-scopes
source_filename: bank-first-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/bank-first-cds-banking-products-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The public PRD API requires NO scopes (unauthenticated). These scopes govern the\n  CDR consumer data sharing surface, which only Accredited Data Recipients may\n  request via the CDR consent flow. The scope set below is the CDR banking + common\n  scope family referenced by the x-scopes extension on the standard's operations.\nschemes:\n  - name: CDR-OAuth2-OIDC\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: (per-holder, discovered via CDR Register / OIDC configuration)\n    tokenUrl: (per-holder, discovered via CDR Register / OIDC configuration)\n    source: openapi/bank-first-cds-banking-products-openapi.yml\nscopes:\n  - scope: bank:accounts.basic:read\n    description: Read basic account information (masked account numbers, product category, balances\
  \ context).\n    sources: [openapi/bank-first-cds-banking-products-openapi.yml]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account information including account numbers and terms.\n    sources: [openapi/bank-first-cds-banking-products-openapi.yml]\n  - scope: bank:transactions:read\n    description: Read account transactions.\n    sources: [openapi/bank-first-cds-banking-products-openapi.yml]\n  - scope: bank:payees:read\n    description: Read saved payees.\n    sources: [openapi/bank-first-cds-banking-products-openapi.yml]\n  - scope: bank:regular_payments:read\n    description: Read direct debits and scheduled/regular payments.\n    sources: [openapi/bank-first-cds-banking-products-openapi.yml]\n  - scope: common:customer.basic:read\n    description: Read basic customer identity (name, organisation).\n    sources: [Consumer Data Standards]\n  - scope: common:customer.detail:read\n    description: Read detailed customer identity (contact details).\n    sources:\
  \ [Consumer Data Standards]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-first/refs/heads/main/scopes/bank-first-scopes.yml
summary_line: 7 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Mutual Bank
- Product Reference Data
token_urls: []
---
