---
api_specs:
- filename: paypal-billing-subscriptions-openapi-original.yml
  format: yaml
  label: PayPal Billing Subscriptions API
  slug: paypal-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-billing-subscriptions-openapi-original.yml
- filename: paypal-catalog-products-openapi-original.yml
  format: yaml
  label: PayPal Catalog Products API
  slug: paypal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-catalog-products-openapi-original.yml
- filename: paypal-checkout-orders-openapi-original.yml
  format: yaml
  label: PayPal Orders API
  slug: paypal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-checkout-orders-openapi-original.yml
- filename: paypal-customer-disputes-openapi-original.yml
  format: yaml
  label: PayPal Customer Disputes API
  slug: paypal-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-disputes-openapi-original.yml
- filename: paypal-customer-partner-referrals-openapi-original.yml
  format: yaml
  label: PayPal Partner Referrals API
  slug: paypal-partner-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-partner-referrals-openapi-original.yml
- filename: paypal-invoicing-openapi-original.yml
  format: yaml
  label: PayPal Invoicing API
  slug: paypal-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-invoicing-openapi-original.yml
- filename: paypal-notification-webhooks-openapi-original.yml
  format: yaml
  label: PayPal Notification Webhooks API
  slug: paypal-notification-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-notification-webhooks-openapi-original.yml
- filename: paypal-payment-experience-openapi-original.yml
  format: yaml
  label: PayPal Payment Experience API
  slug: paypal-payment-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payment-experience-openapi-original.yml
- filename: paypal-payments-openapi-original.yml
  format: yaml
  label: PayPal Payments API
  slug: paypal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payments-openapi-original.yml
- filename: paypal-payouts-openapi-original.yml
  format: yaml
  label: PayPal Payouts API
  slug: paypal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payouts-openapi-original.yml
- filename: paypal-reporting-transactions-openapi-original.yml
  format: yaml
  label: PayPal Transaction Search (Reporting) API
  slug: paypal-reporting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-reporting-transactions-openapi-original.yml
- filename: paypal-shipping-tracking-openapi-original.yml
  format: yaml
  label: PayPal Shipping Tracking API
  slug: paypal-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-shipping-tracking-openapi-original.yml
- filename: paypal-vault-payment-tokens-openapi-original.yml
  format: yaml
  label: PayPal Vault Payment Tokens API
  slug: paypal-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-vault-payment-tokens-openapi-original.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Paypal Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PayPal publishes 39 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PayPal API on a user''s behalf.


  Tokens are issued from /v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PayPal
provider_slug: paypal
schemes:
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-billing-subscriptions-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-catalog-products-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-checkout-orders-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-customer-disputes-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-customer-partner-referrals-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-invoicing-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-notification-webhooks-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-payment-experience-openapi-original.yml
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-payments-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-payouts-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: https://api-m.paypal.com/v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-reporting-transactions-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-shipping-tracking-openapi-original.yml
- description: Oauth 2.0 authentication
  flows:
  - flow: clientCredentials
    tokenUrl: /v1/oauth2/token
  name: Oauth2
  source: openapi/paypal-vault-payment-tokens-openapi-original.yml
scope_count: 39
scope_names:
- https://uri.paypal.com/payments/payouts
- https://uri.paypal.com/services/applications/verify-webhook-signature
- https://uri.paypal.com/services/applications/webhooks
- https://uri.paypal.com/services/customer/partner
- https://uri.paypal.com/services/customer/partner-referrals
- https://uri.paypal.com/services/customer/partner-referrals/readwrite
- https://uri.paypal.com/services/disputes/create
- https://uri.paypal.com/services/disputes/read
- https://uri.paypal.com/services/disputes/read-buyer
- https://uri.paypal.com/services/disputes/read-ebay
- https://uri.paypal.com/services/disputes/read-partner
- https://uri.paypal.com/services/disputes/read-seller
- https://uri.paypal.com/services/disputes/update-buyer
- https://uri.paypal.com/services/disputes/update-partner
- https://uri.paypal.com/services/disputes/update-seller
- https://uri.paypal.com/services/disputes/webhooks
- https://uri.paypal.com/services/invoicing/internal
- https://uri.paypal.com/services/invoicing/invoices/read
- https://uri.paypal.com/services/invoicing/invoices/readwrite
- https://uri.paypal.com/services/payments/initiatepayment
- https://uri.paypal.com/services/payments/non-referenced-credit
- https://uri.paypal.com/services/payments/orders/client-side-integration
- https://uri.paypal.com/services/payments/payment
- https://uri.paypal.com/services/payments/payment/authcapture
- https://uri.paypal.com/services/payments/payment/reference-transaction
- https://uri.paypal.com/services/payments/payouts-item/reverse
- https://uri.paypal.com/services/payments/realtimepayment
- https://uri.paypal.com/services/payments/refund
- https://uri.paypal.com/services/payments/reversepayment
- https://uri.paypal.com/services/referred-disputes/readwrite
- https://uri.paypal.com/services/reporting/balances/read
- https://uri.paypal.com/services/reporting/search/read
- https://uri.paypal.com/services/shipping/trackers/read
- https://uri.paypal.com/services/shipping/trackers/readwrite
- https://uri.paypal.com/services/subscriptions
- https://uri.paypal.com/services/vault/customers/read
- https://uri.paypal.com/services/vault/customers/readwrite
- https://uri.paypal.com/services/vault/payment-tokens/read
- https://uri.paypal.com/services/vault/payment-tokens/readwrite
scopes:
- description: Payout to a list of recipients.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/payments/payouts
- description: Verify Webhook Signature
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/applications/verify-webhook-signature
- description: Access/update Webhooks.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/applications/webhooks
- description: Manage seller resources.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/customer/partner
- description: Manage referral data shared by Partner with PayPal. To be used by only internal apps
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/customer/partner-referrals
- description: Manage external referral data with PayPal
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/customer/partner-referrals/readwrite
- description: This privilege allows client to validate eligibility and create a dispute on his transaction(s).
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/create
- description: This privilege allows client to read and search a dispute of an user with all fields.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/read
- description: This privilege allows client to read and search disputes but returns a limited and allowed set of fields back.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/read-buyer
- description: This privilege allows client to read and search a disputes of an user but gets only a limited and allowed set of fields back to ebay.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/read-ebay
- description: This privilege allows client to read and search disputes but returns a limited and allowed set of fields back.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/read-partner
- description: This privilege allows client to read and search a disputes of a merchant but gets only a limited and allowed set of fields back .
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/read-seller
- description: This privilege allows client to update a dispute (customer actions).
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/update-buyer
- description: This privilege allows client to update a dispute (Partner actions).
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/update-partner
- description: This privilege allows client to update a dispute (Merchant actions).
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/update-seller
- description: This privilege allows webhook platform to read a dispute event
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/disputes/webhooks
- description: Manage invoice resource internal clients.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/invoicing/internal
- description: For Reading the invoice details.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/invoicing/invoices/read
- description: For managing (Create, Update, Delete) invoice.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/invoicing/invoices/readwrite
- description: Initiates payments and checkout workflows.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/initiatepayment
- description: Permission to initiate non referenced credit
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/non-referenced-credit
- description: Allows client-side integration on Create, Get, Patch, Authorize & Capture Order endpoints.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/orders/client-side-integration
- description: Manage payments and checkout workflow.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/payment
- description: Permission to do non-real time payments like capture on authorization
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/payment/authcapture
- description: Permission to initiate reference transaction
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/payment/reference-transaction
- description: For reversing a completed payout item.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/payouts-item/reverse
- description: Permission to do any real-time payment and manage-payment experience profiles with support for sale, authorize, and order intents.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/realtimepayment
- description: Permission to initiate a refund on a capture transaction
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/refund
- description: Permission to do any reverse payment
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/payments/reversepayment
- description: This privilege allows client to read and update a referred dispute.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/referred-disputes/readwrite
- description: List Balances
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/reporting/balances/read
- description: Transactions Search
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/reporting/search/read
- description: Retrieve tracking information
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/shipping/trackers/read
- description: Create or update tracking information
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/shipping/trackers/readwrite
- description: Manage plan & subscription
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/subscriptions
- description: Permission to read customer information.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/vault/customers/read
- description: Permission to create/update customer information.
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/vault/customers/readwrite
- description: Permission to only read from vault
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/vault/payment-tokens/read
- description: Manage payment instruments
  flows:
  - clientCredentials
  scope: https://uri.paypal.com/services/vault/payment-tokens/readwrite
slug: paypal-scopes
source_filename: paypal-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paypal-billing-subscriptions-openapi-original.yml, openapi/paypal-catalog-products-openapi-original.yml,\n  openapi/paypal-checkout-orders-openapi-original.yml, openapi/paypal-customer-disputes-openapi-original.yml,\n  openapi/paypal-customer-partner-referrals-openapi-original.yml, openapi/paypal-invoicing-openapi-original.yml,\n  openapi/paypal-notification-webhooks-openapi-original.yml, openapi/paypal-payment-experience-openapi-original.yml,\n  openapi/paypal-payments-openapi-original.yml, openapi/paypal-payouts-openapi-original.yml,\n  openapi/paypal-reporting-transactions-openapi-original.yml, openapi/paypal-shipping-tracking-openapi-original.yml,\n  openapi/paypal-vault-payment-tokens-openapi-original.yml\nschemes:\n- name: Oauth2\n  source: openapi/paypal-billing-subscriptions-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n-\
  \ name: Oauth2\n  source: openapi/paypal-catalog-products-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-checkout-orders-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-customer-disputes-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-customer-partner-referrals-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-invoicing-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-notification-webhooks-openapi-original.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-payment-experience-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-payments-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: OAuth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-payouts-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-reporting-transactions-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-m.paypal.com/v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-shipping-tracking-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\n- name: Oauth2\n  source: openapi/paypal-vault-payment-tokens-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth2/token\n  description: Oauth 2.0 authentication\nscopes:\n- scope: https://uri.paypal.com/payments/payouts\n  description: Payout to a list of recipients.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payouts-openapi-original.yml\n- scope: https://uri.paypal.com/services/applications/verify-webhook-signature\n  description: Verify Webhook Signature\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-notification-webhooks-openapi-original.yml\n- scope: https://uri.paypal.com/services/applications/webhooks\n  description: Access/update Webhooks.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-notification-webhooks-openapi-original.yml\n- scope: https://uri.paypal.com/services/customer/partner\n  description: Manage seller\
  \ resources.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-partner-referrals-openapi-original.yml\n- scope: https://uri.paypal.com/services/customer/partner-referrals\n  description: Manage referral data shared by Partner with PayPal. To be used by only internal\n    apps\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-partner-referrals-openapi-original.yml\n- scope: https://uri.paypal.com/services/customer/partner-referrals/readwrite\n  description: Manage external referral data with PayPal\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-partner-referrals-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/create\n  description: This privilege allows client to validate eligibility and create a dispute on\n    his transaction(s).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/read\n\
  \  description: This privilege allows client to read and search a dispute of an user with all\n    fields.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/read-buyer\n  description: This privilege allows client to read and search disputes but returns a limited\n    and allowed set of fields back.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/read-ebay\n  description: This privilege allows client to read and search a disputes of an user but gets\n    only a limited and allowed set of fields back to ebay.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/read-partner\n  description: This privilege allows client to read and search disputes but returns a limited\n    and allowed\
  \ set of fields back.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/read-seller\n  description: This privilege allows client to read and search a disputes of a merchant but\n    gets only a limited and allowed set of fields back .\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/update-buyer\n  description: This privilege allows client to update a dispute (customer actions).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/update-partner\n  description: This privilege allows client to update a dispute (Partner actions).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/update-seller\n\
  \  description: This privilege allows client to update a dispute (Merchant actions).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/disputes/webhooks\n  description: This privilege allows webhook platform to read a dispute event\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/invoicing/internal\n  description: Manage invoice resource internal clients.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-invoicing-openapi-original.yml\n- scope: https://uri.paypal.com/services/invoicing/invoices/read\n  description: For Reading the invoice details.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-invoicing-openapi-original.yml\n- scope: https://uri.paypal.com/services/invoicing/invoices/readwrite\n  description: For managing (Create, Update, Delete) invoice.\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/paypal-invoicing-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/initiatepayment\n  description: Initiates payments and checkout workflows.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-checkout-orders-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/non-referenced-credit\n  description: Permission to initiate non referenced credit\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payments-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/orders/client-side-integration\n  description: Allows client-side integration on Create, Get, Patch, Authorize & Capture Order\n    endpoints.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-checkout-orders-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/payment\n  description: Manage payments and checkout workflow.\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/paypal-checkout-orders-openapi-original.yml\n  - openapi/paypal-payment-experience-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/payment/authcapture\n  description: Permission to do non-real time payments like capture on authorization\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payments-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/payment/reference-transaction\n  description: Permission to initiate reference transaction\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-checkout-orders-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/payouts-item/reverse\n  description: For reversing a completed payout item.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payouts-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/realtimepayment\n  description: Permission to do any real-time payment and manage-payment experience profiles\n   \
  \ with support for sale, authorize, and order intents.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payment-experience-openapi-original.yml\n  - openapi/paypal-payments-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/refund\n  description: Permission to initiate a refund on a capture transaction\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payments-openapi-original.yml\n- scope: https://uri.paypal.com/services/payments/reversepayment\n  description: Permission to do any reverse payment\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-payments-openapi-original.yml\n- scope: https://uri.paypal.com/services/referred-disputes/readwrite\n  description: This privilege allows client to read and update a referred dispute.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-customer-disputes-openapi-original.yml\n- scope: https://uri.paypal.com/services/reporting/balances/read\n  description: List Balances\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-reporting-transactions-openapi-original.yml\n- scope: https://uri.paypal.com/services/reporting/search/read\n  description: Transactions Search\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-reporting-transactions-openapi-original.yml\n- scope: https://uri.paypal.com/services/shipping/trackers/read\n  description: Retrieve tracking information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-shipping-tracking-openapi-original.yml\n- scope: https://uri.paypal.com/services/shipping/trackers/readwrite\n  description: Create or update tracking information\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-shipping-tracking-openapi-original.yml\n- scope: https://uri.paypal.com/services/subscriptions\n  description: Manage plan & subscription\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-billing-subscriptions-openapi-original.yml\n  - openapi/paypal-catalog-products-openapi-original.yml\n\
  - scope: https://uri.paypal.com/services/vault/customers/read\n  description: Permission to read customer information.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-vault-payment-tokens-openapi-original.yml\n- scope: https://uri.paypal.com/services/vault/customers/readwrite\n  description: Permission to create/update customer information.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-vault-payment-tokens-openapi-original.yml\n- scope: https://uri.paypal.com/services/vault/payment-tokens/read\n  description: Permission to only read from vault\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-vault-payment-tokens-openapi-original.yml\n- scope: https://uri.paypal.com/services/vault/payment-tokens/readwrite\n  description: Manage payment instruments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paypal-vault-payment-tokens-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/scopes/paypal-scopes.yml
summary_line: 39 scopes · clientCredentials
tags:
- Billing
- Commerce
- Disputes
- Invoices
- Orders
- Payments
- Payouts
- Subscriptions
- Tokens
- Webhooks
token_urls:
- /v1/oauth2/token
- https://api-m.paypal.com/v1/oauth2/token
---
