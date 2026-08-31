---
api_specs:
- filename: pinch-payments-connect-api-openapi.yml
  format: yaml
  label: Pinch Payments Connect API
  slug: pinch-payments-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-connect-api-openapi.yml
- filename: pinch-payments-contacts-api-openapi.yml
  format: yaml
  label: Pinch Payments Contacts API
  slug: pinch-payments-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-contacts-api-openapi.yml
- filename: pinch-payments-events-api-openapi.yml
  format: yaml
  label: Pinch Payments Events API
  slug: pinch-payments-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-events-api-openapi.yml
- filename: pinch-payments-fees-api-openapi.yml
  format: yaml
  label: Pinch Payments Fees API
  slug: pinch-payments-fees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-fees-api-openapi.yml
- filename: pinch-payments-health-api-openapi.yml
  format: yaml
  label: Pinch Payments Health API
  slug: pinch-payments-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-health-api-openapi.yml
- filename: pinch-payments-merchant-financial-data-api-openapi.yml
  format: yaml
  label: Pinch Payments Merchant Financial Data API
  slug: pinch-payments-merchant-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchant-financial-data-api-openapi.yml
- filename: pinch-payments-merchants-api-openapi.yml
  format: yaml
  label: Pinch Payments Merchants API
  slug: pinch-payments-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-merchants-api-openapi.yml
- filename: pinch-payments-payers-api-openapi.yml
  format: yaml
  label: Pinch Payments Payers API
  slug: pinch-payments-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payers-api-openapi.yml
- filename: pinch-payments-payment-links-api-openapi.yml
  format: yaml
  label: Pinch Payments Payment Links API
  slug: pinch-payments-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payment-links-api-openapi.yml
- filename: pinch-payments-payments-api-openapi.yml
  format: yaml
  label: Pinch Payments Payments API
  slug: pinch-payments-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-payments-api-openapi.yml
- filename: pinch-payments-plans-api-openapi.yml
  format: yaml
  label: Pinch Payments Plans API
  slug: pinch-payments-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-plans-api-openapi.yml
- filename: pinch-payments-refund-api-openapi.yml
  format: yaml
  label: Pinch Payments Refund API
  slug: pinch-payments-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-refund-api-openapi.yml
- filename: pinch-payments-refunds-api-openapi.yml
  format: yaml
  label: Pinch Payments Refunds API
  slug: pinch-payments-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-refunds-api-openapi.yml
- filename: pinch-payments-subscriptions-api-openapi.yml
  format: yaml
  label: Pinch Payments Subscriptions API
  slug: pinch-payments-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-subscriptions-api-openapi.yml
- filename: pinch-payments-tokens-api-openapi.yml
  format: yaml
  label: Pinch Payments Tokens API
  slug: pinch-payments-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-tokens-api-openapi.yml
- filename: pinch-payments-transfers-api-openapi.yml
  format: yaml
  label: Pinch Payments Transfers API
  slug: pinch-payments-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-transfers-api-openapi.yml
- filename: pinch-payments-webhooks-api-openapi.yml
  format: yaml
  label: Pinch Payments Webhooks API
  slug: pinch-payments-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/openapi/pinch-payments-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.getpinch.com.au/docs/application-authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Pinch Payments Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pinch Payments publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pinch Payments API on a user''s behalf.


  Tokens are issued from https://auth.getpinch.com.au/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pinch Payments
provider_slug: pinch-payments
schemes:
- flows:
  - flow: clientCredentials
    scopes:
      api1: Full access to the Pinch REST API (v2020.1)
    tokenUrl: https://auth.getpinch.com.au/connect/token
  name: OAuth2 (client-credentials)
  source: openapi/pinch-payments-authentication.yml
scope_count: 1
scope_names:
- api1
scopes:
- description: The single documented scope. Requested as scope=api1 in the client-credentials grant; grants access to the Pinch API surface. Must be set to "api1".
  flows:
  - clientCredentials
  scope: api1
slug: pinch-payments-scopes
source_filename: pinch-payments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/pinch-payments-authentication.yml\ndocs: https://docs.getpinch.com.au/docs/application-authentication\nsummary: >-\n  The Pinch API uses OAuth 2.0 client-credentials. A single coarse scope, \"api1\",\n  grants access to the whole Pinch REST API; Pinch does not publish a fine-grained\n  per-resource scope surface. Tokens are obtained from the auth.getpinch.com.au\n  token endpoint using an Application ID + Secret Key (Merchant ID as client_id is\n  deprecated) and are short-lived (3600s Bearer JWT). Applications can be\n  \"restricted to specific permissions\" per the docs, but the named permission set\n  is not published in the machine-readable spec.\nschemes:\n- name: OAuth2 (client-credentials)\n  source: openapi/pinch-payments-authentication.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.getpinch.com.au/connect/token\n    scopes:\n      api1: Full access to the Pinch REST API (v2020.1)\nscopes:\n\
  - scope: api1\n  description: >-\n    The single documented scope. Requested as scope=api1 in the client-credentials\n    grant; grants access to the Pinch API surface. Must be set to \"api1\".\n  flows: [clientCredentials]\n  sources: [openapi/pinch-payments-authentication.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinch-payments/refs/heads/main/scopes/pinch-payments-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Direct Debit
- Card Payments
- Subscription
- Billing
- Payment Facilitator
- Account-to-Account
- New Zealand
token_urls:
- https://auth.getpinch.com.au/connect/token
---
