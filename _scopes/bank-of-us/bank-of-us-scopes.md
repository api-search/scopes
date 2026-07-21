---
api_specs:
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Product Reference Data API
  slug: bank-of-us-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Accounts & Balances API
  slug: bank-of-us-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Transactions API
  slug: bank-of-us-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Direct Debits & Scheduled Payments API
  slug: bank-of-us-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
- filename: bank-of-us-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of us CDR Payees API
  slug: bank-of-us-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/openapi/bank-of-us-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bank Of Us Scopes
name_suffix: OAuth Scopes
note: The shared DSB CDS banking OpenAPI declares no oauth2 securityScheme (the CDR Security Profile lives outside the spec), so these scopes are derived from the per-operation x-scopes extension in the spec, which mirrors the CDR banking authorisation-scopes registry. Scopes apply ONLY to the authenticated consumer-data endpoints; the public Product Reference Data endpoints require no scope.
overview: 'Bank of us publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank of us API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank of us
provider_slug: bank-of-us
schemes:
- flows:
  - flow: authorizationCode
  name: CDR-OAuth2
  source: CDR Security Profile (FAPI OAuth2 authorization code)
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:regular_payments:read
- bank:payees:read
scopes:
- description: Read basic account information (account list, product category, balances at basic level).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information (account detail, features, addresses, MTLS-protected).
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions and transaction detail.
  flows: []
  scope: bank:transactions:read
- description: Read scheduled payments, direct debits and other regular payment arrangements.
  flows: []
  scope: bank:regular_payments:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
slug: bank-of-us-scopes
source_filename: bank-of-us-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/bank-of-us-cds-banking-products-openapi.yml (x-scopes)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnote: >-\n  The shared DSB CDS banking OpenAPI declares no oauth2 securityScheme (the CDR\n  Security Profile lives outside the spec), so these scopes are derived from the\n  per-operation x-scopes extension in the spec, which mirrors the CDR banking\n  authorisation-scopes registry. Scopes apply ONLY to the authenticated\n  consumer-data endpoints; the public Product Reference Data endpoints require no\n  scope.\nschemes:\n- name: CDR-OAuth2\n  source: CDR Security Profile (FAPI OAuth2 authorization code)\n  flows:\n  - flow: authorizationCode\nscopes:\n- scope: bank:accounts.basic:read\n  description: Read basic account information (account list, product category, balances at basic level).\n  sources: [openapi/bank-of-us-cds-banking-products-openapi.yml]\n- scope: bank:accounts.detail:read\n\
  \  description: Read detailed account information (account detail, features, addresses, MTLS-protected).\n  sources: [openapi/bank-of-us-cds-banking-products-openapi.yml]\n- scope: bank:transactions:read\n  description: Read account transactions and transaction detail.\n  sources: [openapi/bank-of-us-cds-banking-products-openapi.yml]\n- scope: bank:regular_payments:read\n  description: Read scheduled payments, direct debits and other regular payment arrangements.\n  sources: [openapi/bank-of-us-cds-banking-products-openapi.yml]\n- scope: bank:payees:read\n  description: Read saved payees.\n  sources: [openapi/bank-of-us-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-us/refs/heads/main/scopes/bank-of-us-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Tasmania
- Mutual
- Product Reference Data
token_urls: []
---
