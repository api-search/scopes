---
api_specs:
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Product Reference Data API
  slug: macquarie-bank-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Discovery Status API
  slug: macquarie-bank-cdr-discovery-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Accounts & Balances API
  slug: macquarie-bank-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Transactions API
  slug: macquarie-bank-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Direct Debits & Scheduled Payments API
  slug: macquarie-bank-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
- filename: macquarie-bank-cds-banking-products-openapi.yml
  format: yaml
  label: Macquarie Bank CDR Payees API
  slug: macquarie-bank-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/openapi/macquarie-bank-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Macquarie Bank Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Macquarie Bank publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Macquarie Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Macquarie Bank
provider_slug: macquarie-bank
schemes:
- flows:
  - flow: authorizationCode
  name: cdr-oidc
  profile: FAPI 1.0 Advanced
scope_count: 10
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
- cdr:registration
scopes:
- description: OpenID Connect authentication; required for CDR consent flows.
  flows: []
  scope: openid
- description: Standard OIDC profile claim scope.
  flows: []
  scope: profile
- description: Read masked account numbers and basic account details.
  flows: []
  scope: bank:accounts.basic:read
- description: Read full account and product-specific detail, including unmasked account numbers.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled payments.
  flows: []
  scope: bank:regular_payments:read
- description: Read basic customer (name, occupation) or organisation profile.
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer contact and identity information.
  flows: []
  scope: common:customer.detail:read
- description: Dynamic client registration under the CDR Register (ADR onboarding).
  flows: []
  scope: cdr:registration
slug: macquarie-bank-scopes
source_filename: macquarie-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: |\n  Australian Consumer Data Right (CDR) authorisation scopes, DSB Consumer Data\n  Standards. Applies to the authenticated CDR Banking Data Sharing surface. The\n  harvested CDS OpenAPI declares no inline oauth2 securitySchemes (CDR scopes are\n  defined by the standards, not per data holder), so scopes are authored from the\n  Consumer Data Standards authorisation-scopes reference.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\napplies_to: Macquarie Bank CDR Banking Data Sharing API\nschemes:\n- name: cdr-oidc\n  profile: FAPI 1.0 Advanced\n  flows:\n  - flow: authorizationCode\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required for CDR consent flows.\n- scope: profile\n  description: Standard OIDC profile claim scope.\n- scope: bank:accounts.basic:read\n  description: Read masked account numbers and basic account details.\n- scope: bank:accounts.detail:read\n\
  \  description: Read full account and product-specific detail, including unmasked account numbers.\n- scope: bank:transactions:read\n  description: Read account transactions.\n- scope: bank:payees:read\n  description: Read saved payees.\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled payments.\n- scope: common:customer.basic:read\n  description: Read basic customer (name, occupation) or organisation profile.\n- scope: common:customer.detail:read\n  description: Read detailed customer contact and identity information.\n- scope: cdr:registration\n  description: Dynamic client registration under the CDR Register (ADR onboarding).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macquarie-bank/refs/heads/main/scopes/macquarie-bank-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Data Right
- Consumer Banking
- Australia
- Product Reference Data
- Payments
token_urls: []
---
