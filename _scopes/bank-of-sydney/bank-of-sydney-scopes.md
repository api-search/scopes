---
api_specs:
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Product Reference Data API
  slug: bank-of-sydney-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Accounts & Balances API
  slug: bank-of-sydney-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Transactions API
  slug: bank-of-sydney-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Direct Debits & Scheduled Payments API
  slug: bank-of-sydney-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
- filename: bank-of-sydney-cds-banking-products-openapi.yml
  format: yaml
  label: Bank of Sydney CDR Payees API
  slug: bank-of-sydney-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/openapi/bank-of-sydney-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Bank Of Sydney Scopes
name_suffix: OAuth Scopes
note: The harvested CDS banking spec declares scopes on each operation via the x-scopes extension (not an OpenAPI oauth2 securityScheme), so the standard derive-oauth-scopes pass yields nothing; these five CDR banking scopes are extracted from those x-scopes values. Product Reference Data operations are public and require no scope. Scopes are granted through the CDR authorisation server to Accredited Data Recipients under consumer consent.
overview: 'Bank of Sydney publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank of Sydney API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank of Sydney
provider_slug: bank-of-sydney
schemes:
- flow: authorizationCode
  name: cdrOAuth2
  source: openapi/bank-of-sydney-cds-banking-products-openapi.yml
  type: oauth2
scope_count: 5
scope_names:
- bank:accounts.basic:read
- bank:accounts.detail:read
- bank:transactions:read
- bank:payees:read
- bank:regular_payments:read
scopes:
- description: Read basic account data - the list of accounts and their balances.
  flows:
  - authorizationCode
  scope: bank:accounts.basic:read
- description: Read detailed account data, including account numbers and product details for a specific account.
  flows:
  - authorizationCode
  scope: bank:accounts.detail:read
- description: Read transaction data for authorised accounts.
  flows:
  - authorizationCode
  scope: bank:transactions:read
- description: Read the consumer's saved payees.
  flows:
  - authorizationCode
  scope: bank:payees:read
- description: Read regular payments - direct debits and scheduled payments.
  flows:
  - authorizationCode
  scope: bank:regular_payments:read
slug: bank-of-sydney-scopes
source_filename: bank-of-sydney-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/bank-of-sydney-cds-banking-products-openapi.yml (x-scopes extension per operation)\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  The harvested CDS banking spec declares scopes on each operation via the x-scopes\n  extension (not an OpenAPI oauth2 securityScheme), so the standard derive-oauth-scopes\n  pass yields nothing; these five CDR banking scopes are extracted from those x-scopes\n  values. Product Reference Data operations are public and require no scope. Scopes are\n  granted through the CDR authorisation server to Accredited Data Recipients under\n  consumer consent.\nschemes:\n  - name: cdrOAuth2\n    type: oauth2\n    flow: authorizationCode\n    source: openapi/bank-of-sydney-cds-banking-products-openapi.yml\nscopes:\n  - scope: bank:accounts.basic:read\n    description: Read basic account data - the list of accounts and their balances.\n    flows: [authorizationCode]\n\
  \    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - scope: bank:accounts.detail:read\n    description: Read detailed account data, including account numbers and product details for a specific account.\n    flows: [authorizationCode]\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - scope: bank:transactions:read\n    description: Read transaction data for authorised accounts.\n    flows: [authorizationCode]\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - scope: bank:payees:read\n    description: Read the consumer's saved payees.\n    flows: [authorizationCode]\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n  - scope: bank:regular_payments:read\n    description: Read regular payments - direct debits and scheduled payments.\n    flows: [authorizationCode]\n    sources: [openapi/bank-of-sydney-cds-banking-products-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-sydney/refs/heads/main/scopes/bank-of-sydney-scopes.yml
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
