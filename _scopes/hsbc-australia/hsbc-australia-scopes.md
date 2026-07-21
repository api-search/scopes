---
api_specs:
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Product Reference Data API
  slug: hsbc-australia-cdr-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Accounts & Balances API
  slug: hsbc-australia-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Transactions API
  slug: hsbc-australia-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Direct Debits & Scheduled Payments API
  slug: hsbc-australia-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
- filename: hsbc-australia-cds-banking-products-openapi.yml
  format: yaml
  label: HSBC Bank Australia CDR Payees API
  slug: hsbc-australia-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/openapi/hsbc-australia-cds-banking-products-openapi.yml
authorization_urls:
- https://public.ob.hsbc.com.au/cds-au/v1/oauth2/authorize
description: ''
docs: https://consumerdatastandardsaustralia.github.io/standards/#end-points
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Hsbc Australia Scopes
name_suffix: OAuth Scopes
note: Scopes are published live in the HSBC Australia CDR OpenID Connect discovery document (scopes_supported). They govern the AUTHENTICATED consumer data sharing surface, which is restricted to Accredited Data Recipients (ADRs) under the CDR register - not the public unauthenticated Product Reference Data endpoints, which require no scopes. Scope semantics follow the DSB Consumer Data Standards (Australia).
overview: 'HSBC Bank Australia publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HSBC Bank Australia API on a user''s behalf.


  Tokens are issued from https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HSBC Bank Australia
provider_slug: hsbc-australia
schemes:
- flows:
  - authorizationUrl: https://public.ob.hsbc.com.au/cds-au/v1/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token
  name: CDR OpenID Connect (FAPI)
  source: https://public.ob.hsbc.com.au/.well-known/openid-configuration
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
- description: OpenID Connect authentication (required).
  flows: []
  scope: openid
- description: CDR profile claims (name and related identity claims).
  flows: []
  scope: profile
- description: Read basic account data - account name, type, and balance.
  flows: []
  scope: bank:accounts.basic:read
- description: Read detailed account data - account numbers and features.
  flows: []
  scope: bank:accounts.detail:read
- description: Read account transactions.
  flows: []
  scope: bank:transactions:read
- description: Read saved payees.
  flows: []
  scope: bank:payees:read
- description: Read direct debits and scheduled/recurring payments.
  flows: []
  scope: bank:regular_payments:read
- description: Read basic customer data - name and occupation.
  flows: []
  scope: common:customer.basic:read
- description: Read detailed customer data - contact details.
  flows: []
  scope: common:customer.detail:read
- description: Dynamic client registration against the CDR register.
  flows: []
  scope: cdr:registration
slug: hsbc-australia-scopes
source_filename: hsbc-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://public.ob.hsbc.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#end-points\nnote: |\n  Scopes are published live in the HSBC Australia CDR OpenID Connect discovery\n  document (scopes_supported). They govern the AUTHENTICATED consumer data\n  sharing surface, which is restricted to Accredited Data Recipients (ADRs)\n  under the CDR register - not the public unauthenticated Product Reference\n  Data endpoints, which require no scopes. Scope semantics follow the DSB\n  Consumer Data Standards (Australia).\nschemes:\n- name: CDR OpenID Connect (FAPI)\n  source: https://public.ob.hsbc.com.au/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public.ob.hsbc.com.au/cds-au/v1/oauth2/authorize\n    tokenUrl: https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\
  \ (required).\n- scope: profile\n  description: CDR profile claims (name and related identity claims).\n- scope: bank:accounts.basic:read\n  description: Read basic account data - account name, type, and balance.\n- scope: bank:accounts.detail:read\n  description: Read detailed account data - account numbers and features.\n- scope: bank:transactions:read\n  description: Read account transactions.\n- scope: bank:payees:read\n  description: Read saved payees.\n- scope: bank:regular_payments:read\n  description: Read direct debits and scheduled/recurring payments.\n- scope: common:customer.basic:read\n  description: Read basic customer data - name and occupation.\n- scope: common:customer.detail:read\n  description: Read detailed customer data - contact details.\n- scope: cdr:registration\n  description: Dynamic client registration against the CDR register.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hsbc-australia/refs/heads/main/scopes/hsbc-australia-scopes.yml
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
token_urls:
- https://mtls.ob.hsbc.com.au/cds-au/v1/oauth2/token
---
