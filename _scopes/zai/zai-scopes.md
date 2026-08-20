---
api_specs:
- filename: zai-assembly-api.json
  format: json
  label: Zai Assembly API
  slug: zai-assembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-assembly-api.json
- filename: zai-virtual-accounts-payid.json
  format: json
  label: Zai Virtual Accounts and PayIDs API
  slug: zai-virtual-accounts-payid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-virtual-accounts-payid.json
- filename: zai-payto.json
  format: json
  label: Zai PayTo API
  slug: zai-payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-payto.json
- filename: zai-async-api.json
  format: json
  label: Zai Asynchronous API
  slug: zai-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/openapi/zai-async-api.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Zai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://au-0000.sandbox.auth.assemblypay.com/tokens.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zai
provider_slug: zai
schemes:
- description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens
  name: oAuth2ClientCredentials
  source: openapi/zai-assembly-api.json
- description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens
  name: oAuth2ClientCredentials
  source: openapi/zai-async-api.json
scope_count: 0
scope_names: []
scopes: []
slug: zai-scopes
source_filename: zai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/zai-assembly-api.json, openapi/zai-async-api.json\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/zai-assembly-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens\n  description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication\n- name: oAuth2ClientCredentials\n  source: openapi/zai-async-api.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://au-0000.sandbox.auth.assemblypay.com/tokens\n  description: Please refer to Authentication section within https://developer.assemblypayments.com/reference#authentication\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zai/refs/heads/main/scopes/zai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Marketplace Payments
- Payments-as-a-Service
- Real-Time Payments
- Account-to-Account
- Open Banking
- PayTo
- PayID
- NPP
- Direct Debit
- Digital Wallet
- Payouts
token_urls:
- https://au-0000.sandbox.auth.assemblypay.com/tokens
---
