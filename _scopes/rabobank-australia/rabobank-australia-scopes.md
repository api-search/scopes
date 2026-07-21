---
api_specs:
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Product Reference Data API
  slug: rabobank-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Accounts & Balances API
  slug: rabobank-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Transactions API
  slug: rabobank-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Direct Debits & Scheduled Payments API
  slug: rabobank-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
- filename: rabobank-australia-cds-banking-products-openapi.yml
  format: yaml
  label: Rabobank Australia CDR Payees API
  slug: rabobank-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/openapi/rabobank-australia-cds-banking-products-openapi.yml
authorization_urls: []
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rabobank Australia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rabobank Australia publishes 10 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rabobank Australia API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rabobank Australia
provider_slug: rabobank-australia
schemes:
- name: cdr-oauth2-oidc-fapi
  scheme_detail: OpenID Connect Hybrid flow, FAPI 1.0 Advanced security profile, PAR + PKCE, mTLS-bound (sender-constrained) access tokens. Authorization/token endpoints are discovered per data holder through the CDR Register, not published as a self-serve developer endpoint.
  type: oauth2
scope_count: 10
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
- cdr:registration
scopes:
- description: OpenID Connect authentication; required to obtain an ID token for the consent.
  flows: []
  scope: openid
- description: OpenID Connect end-user profile claims permitted under the CDR.
  flows: []
  scope: profile
- description: Read basic customer information (name, occupation for individuals; agent/organisation basics for businesses).
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer information (contact details — phone, email, addresses — in addition to basic).
  flows: []
  scope: common:customer.detail:read
- description: Read the list of accounts and basic account information (masked number, product category, balance).
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account information (full account attributes, features, rates, fees, deposit/lending detail).
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions, including detail and description.
  flows: []
  scope: bank:transactions:read
- description: Read the consumer's saved payees (domestic, international, biller).
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/regular payments configured on the consumer's accounts.
  flows: []
  scope: bank:regular_payments:read
- description: Dynamic Client Registration (admin) scope used by accredited data recipients to manage their registration with the data holder.
  flows: []
  scope: cdr:registration
slug: rabobank-australia-scopes
source_filename: rabobank-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  Data Standards Body (DSB) Consumer Data Standards — Authorisation Scopes +\n  authentication/rabobank-australia-authentication.yml. The harvested CDS\n  Banking OpenAPI declares no securitySchemes (resource-endpoint spec), so\n  scopes are taken from the standardized CDR authorisation model that every\n  Australian banking data holder (including Rabobank Australia) implements.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#authorisation-scopes\nnotes: >-\n  These scopes apply ONLY to the consumer-AUTHORIZED CDR surface (accounts,\n  balances, transactions, direct debits, scheduled payments, payees), reached by\n  accredited data recipients (ADRs) via the CDR OAuth2 / OpenID Connect (FAPI 1.0\n  Advanced) authorization flow over mTLS. The public Product Reference Data\n  endpoints (GET /banking/products, /banking/products/{productId}) require NO\n  scope. Rabobank Australia does not self-serve these\
  \ scopes; access is governed\n  by the CDR Register and accreditation regime.\nschemes:\n- name: cdr-oauth2-oidc-fapi\n  type: oauth2\n  scheme_detail: >-\n    OpenID Connect Hybrid flow, FAPI 1.0 Advanced security profile, PAR + PKCE,\n    mTLS-bound (sender-constrained) access tokens. Authorization/token endpoints\n    are discovered per data holder through the CDR Register, not published as a\n    self-serve developer endpoint.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to obtain an ID token for the consent.\n  category: openid\n- scope: profile\n  description: OpenID Connect end-user profile claims permitted under the CDR.\n  category: openid\n- scope: common:customer.basic:read\n  description: Read basic customer information (name, occupation for individuals; agent/organisation basics for businesses).\n  category: common\n- scope: common:customer.detail:read\n  description: Read detailed customer information (contact details — phone, email, addresses\
  \ — in addition to basic).\n  category: common\n- scope: bank:accounts.basic:read\n  description: Read the list of accounts and basic account information (masked number, product category, balance).\n  category: banking\n- scope: bank:accounts.detail:read\n  description: Read detailed account information (full account attributes, features, rates, fees, deposit/lending detail).\n  category: banking\n- scope: bank:transactions:read\n  description: Read account transactions, including detail and description.\n  category: banking\n- scope: bank:payees:read\n  description: Read the consumer's saved payees (domestic, international, biller).\n  category: banking\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/regular payments configured on the consumer's accounts.\n  category: banking\n- scope: cdr:registration\n  description: Dynamic Client Registration (admin) scope used by accredited data recipients to manage their registration with the data holder.\n \
  \ category: admin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rabobank-australia/refs/heads/main/scopes/rabobank-australia-scopes.yml
summary_line: 10 scopes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Agribusiness
- Product Reference Data
token_urls: []
---
