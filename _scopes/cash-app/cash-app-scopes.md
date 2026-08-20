---
api_specs:
- filename: cash-app-network-api-openapi.json
  format: json
  label: Cash App Pay Network API
  slug: cash-app-pay-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-network-api-openapi.json
- filename: cash-app-customer-request-api-openapi.json
  format: json
  label: Cash App Pay Customer Request API
  slug: cash-app-pay-customer-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-customer-request-api-openapi.json
- filename: cash-app-management-api-openapi.json
  format: json
  label: Cash App Pay Management API
  slug: cash-app-pay-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-management-api-openapi.json
- filename: cash-app-payments-openapi.json
  format: json
  label: Afterpay Payments API
  slug: afterpay-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-payments-openapi.json
- filename: cash-app-checkouts-openapi.json
  format: json
  label: Afterpay Checkouts API
  slug: afterpay-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-checkouts-openapi.json
- filename: cash-app-orders-openapi.json
  format: json
  label: Afterpay Orders API
  slug: afterpay-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-orders-openapi.json
- filename: cash-app-configuration-openapi.json
  format: json
  label: Afterpay Configuration API
  slug: afterpay-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-configuration-openapi.json
- filename: cash-app-disputes-openapi.json
  format: json
  label: Afterpay Disputes API
  slug: afterpay-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-disputes-openapi.json
- filename: cash-app-grants-afterpay-openapi.json
  format: json
  label: Afterpay Grants API
  slug: afterpay-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-grants-afterpay-openapi.json
- filename: cash-app-grants-cash-app-pay-openapi.json
  format: json
  label: Add Cash App Pay to Your Site (Grants) API
  slug: cash-app-pay-site-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-grants-cash-app-pay-openapi.json
- filename: cash-app-service-status-openapi.json
  format: json
  label: Afterpay Service Status API
  slug: afterpay-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-service-status-openapi.json
- filename: cash-app-billing-agreements-deprecated-openapi.json
  format: json
  label: Afterpay Billing Agreements API (Deprecated)
  slug: afterpay-billing-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/openapi/cash-app-billing-agreements-deprecated-openapi.json
authorization_urls: []
description: ''
docs: https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/using-api-keys
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Cash App Scopes
name_suffix: OAuth Scopes
note: Cash App Pay is not OAuth2 - permissions are attached to API keys as scopes at key-creation time (via the Management API create-api-key). Cash App recommends provisioning multiple least-privilege keys. An INSUFFICIENT_SCOPES (HTTP 403) error is returned when a key lacks the scope for an action. The docs enumerate the read/write scope pairs by resource family; the full set follows the {RESOURCE}_READ / {RESOURCE}_WRITE convention.
overview: 'Cash App publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cash App API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cash App
provider_slug: cash-app
schemes:
- applies_to:
  - Network API
  - Management API
  - Customer Request API
  enforced_by: 'Authorization: Client {CLIENT_ID} {KEY_ID}'
  granted_via: Management API create-api-key
  name: cash-app-pay-api-key-scopes
scope_count: 4
scope_names:
- API_KEYS_READ
- API_KEYS_WRITE
- PAYMENTS_READ
- PAYMENTS_WRITE
scopes:
- description: Read API keys via the Management API.
  flows: []
  scope: API_KEYS_READ
- description: Create, rotate, and delete API keys via the Management API (bootstrap + rotation scope).
  flows: []
  scope: API_KEYS_WRITE
- description: Read payments, authorizations, captures, and payment state.
  flows: []
  scope: PAYMENTS_READ
- description: Create, capture, void payments and payment authorizations.
  flows: []
  scope: PAYMENTS_WRITE
slug: cash-app-scopes
source_filename: cash-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/using-api-keys\ndocs: https://developers.cash.app/cash-app-pay-partner-api/guides/technical-guides/api-fundamentals/requests/using-api-keys\nmodel: scoped-api-keys\nnote: |\n  Cash App Pay is not OAuth2 - permissions are attached to API keys as scopes at key-creation time\n  (via the Management API create-api-key). Cash App recommends provisioning multiple least-privilege\n  keys. An INSUFFICIENT_SCOPES (HTTP 403) error is returned when a key lacks the scope for an action.\n  The docs enumerate the read/write scope pairs by resource family; the full set follows the\n  {RESOURCE}_READ / {RESOURCE}_WRITE convention.\nschemes:\n- name: cash-app-pay-api-key-scopes\n  applies_to: [Network API, Management API, Customer Request API]\n  granted_via: Management API create-api-key\n  enforced_by: 'Authorization: Client {CLIENT_ID} {KEY_ID}'\n\
  scopes:\n- scope: API_KEYS_READ\n  description: Read API keys via the Management API.\n- scope: API_KEYS_WRITE\n  description: Create, rotate, and delete API keys via the Management API (bootstrap + rotation scope).\n- scope: PAYMENTS_READ\n  description: Read payments, authorizations, captures, and payment state.\n- scope: PAYMENTS_WRITE\n  description: Create, capture, void payments and payment authorizations.\nscope_convention:\n  pattern: '{RESOURCE}_READ / {RESOURCE}_WRITE'\n  resource_families_documented: [API_KEYS, PAYMENTS]\n  note: |\n    Only API_KEYS and PAYMENTS scope names are quoted verbatim in the Using API Keys guide (as the\n    worked bootstrap example). Other resource families (refunds, payouts, merchants, brands, grants,\n    disputes, webhooks) follow the same READ/WRITE convention; their exact scope strings are issued\n    with partner credentials and are not enumerated in the public docs, so they are not listed here\n    to avoid fabrication.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cash-app/refs/heads/main/scopes/cash-app-scopes.yml
summary_line: 4 scopes
tags:
- Financial-Services
- Payments
- United States
- Fintech
- Neobank
- Buy Now Pay Later
- Payment Acceptance
- Digital Wallet
token_urls: []
---
