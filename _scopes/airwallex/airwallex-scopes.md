---
api_specs:
- filename: airwallex-authentication-api-openapi.yml
  format: yaml
  label: Airwallex Authentication API
  slug: airwallex-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-authentication-api-openapi.yml
- filename: airwallex-balances-api-openapi.yml
  format: yaml
  label: Airwallex Balances API
  slug: airwallex-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-balances-api-openapi.yml
- filename: airwallex-beneficiaries-api-openapi.yml
  format: yaml
  label: Airwallex Beneficiaries API
  slug: airwallex-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-beneficiaries-api-openapi.yml
- filename: airwallex-customers-api-openapi.yml
  format: yaml
  label: Airwallex Customers API
  slug: airwallex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-customers-api-openapi.yml
- filename: airwallex-payment-intents-api-openapi.yml
  format: yaml
  label: Airwallex Payment Intents API
  slug: airwallex-payment-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payment-intents-api-openapi.yml
- filename: airwallex-payouts-api-openapi.yml
  format: yaml
  label: Airwallex Payouts API
  slug: airwallex-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-payouts-api-openapi.yml
- filename: airwallex-refunds-api-openapi.yml
  format: yaml
  label: Airwallex Refunds API
  slug: airwallex-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-refunds-api-openapi.yml
- filename: airwallex-transfers-api-openapi.yml
  format: yaml
  label: Airwallex Transfers API
  slug: airwallex-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/openapi/airwallex-transfers-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Airwallex Scopes
name_suffix: OAuth Scopes
note: Airwallex exposes TWO distinct OAuth scope vocabularies and both are real. (1) The partner-connections scope reference documents 98 `<resource>:<read|write>` scopes for third-party applications, each row mapping the scope to the REST operations it authorizes and the webhook events it may subscribe to. (2) The hosted MCP servers advertise a different, coarser `<r|w>:<awx_action|org_action>:<permission>` vocabulary in their RFC 9728 protected-resource metadata — 35 scopes on production, 48 in sandbox — fetched anonymously and saved verbatim under well-known/. No oauth2 securityScheme appears in the OpenAPI held in this repo, so none of this is derivable from the spec; every scope below was read off a provider surface.
overview: 'Airwallex publishes 180 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Airwallex API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Airwallex
provider_slug: airwallex
schemes:
- audience: third-party applications connecting to a merchant Airwallex account
  consent_roles:
  - Owner
  - Admin
  - Finance Admin
  name: Airwallex Partner Connections OAuth
  scope_count: 98
  source: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes
- authorization_servers:
  - https://mcp.airwallex.com/mcp
  bearer_methods_supported:
  - header
  name: Airwallex AgentOS MCP (production)
  resource: https://mcp.airwallex.com/mcp
  scope_count: 35
  source: https://mcp.airwallex.com/.well-known/oauth-protected-resource/mcp/
- authorization_servers:
  - https://mcp.sandbox.airwallex.com/developer
  bearer_methods_supported:
  - header
  name: Airwallex Developer MCP (sandbox)
  resource: https://mcp.sandbox.airwallex.com/developer
  scope_count: 47
  source: https://mcp.sandbox.airwallex.com/.well-known/oauth-protected-resource/developer/
scope_count: 180
scope_names:
- account_details:read
- billing.checkout:read
- billing.checkout:write
- billing.customer:read
- billing.customer:write
- billing.transaction:read
- billing.credit_note:read
- billing.credit_note:write
- billing.discount:read
- billing.discount:write
- billing.invoice:read
- billing.invoice:write
- billing.payment_source:read
- billing.payment_source:write
- billing.price:read
- billing.price:write
- billing.product:read
- billing.product:write
- billing.subscription:read
- billing.subscription:write
- billing.usage_metering:read
- billing.usage_metering:write
- balance:read
- global_account:read
- global_account:write
- issuing.card:read
- issuing.card:write
- issuing.cardholder:read
- issuing.cardholder:write
- issuing.transaction:read
- issuing.merchant_brand:read
- financial_report:read
- financial_report:write
- financial_transaction:read
- payment_link:read
- payment_link:write
- payment_acceptance:read
- payment_acceptance:write
- payment_dispute:read
- payment_dispute:write
- pos_terminal:read
- pos_terminal:write
- funds_split:write
- funds_split:read
- beneficiary:read
- beneficiary:write
- transfer:read
- transfer:write
- risk.rfi:read
- risk.rfi:write
- simulation:write
- spend.bill:read
- spend.bill:write
- spend.expense:read
- spend.expense:write
- spend.purchase_order:read
- spend.purchase_order:write
- spend.vendor:read
- spend.vendor:write
- reference.order_item:read
- reference.order_item:write
- commerce_store:read
- file:upload
- fx.conversion:read
- fx.conversion:write
- Product
- Accounts
- Business Accounts
- Business Accounts
- Business Accounts
- Cards
- Cards
- Cards
- Cards
- Cards
- Cards
- Finance
- Payments
- Payments
- Payments
- Payments
- Payments
- Payments
- Payments
- Payments
- Payments
- Payments
- Payouts
- Payouts
- Payouts
- Payouts
- Simulations
- Supporting Services
- Supporting Services
- Supporting Services
- Supporting Services
- Transactional FX
- Transactional FX
- r:awx_action:balances_view
- r:awx_action:contact_management_view
- r:awx_action:conversions_view
- r:awx_action:global_accounts_view
- r:awx_action:issuing_cardholders_view
- r:awx_action:issuing_cards_view
- r:awx_action:issuing_transactions_view
- r:awx_action:pa_view
- r:awx_action:payment_links_view
- r:awx_action:settings.account_details_view
- r:awx_action:transfers_view
- r:org_action:billing.customer_view
- r:org_action:billing.discount_view
- r:org_action:billing.invoice_view
- r:org_action:billing.payment_source_view
- r:org_action:billing.price_view
- r:org_action:billing.product_view
- r:org_action:billing.subscription_view
- r:org_action:billing.transaction_view
- r:org_action:billing.usage_metering_view
- r:org_action:expense_management.expense:api_view
- r:org_action:spend.bills:api_view
- r:org_action:spend.vendors:api_view
- w:awx_action:contact_management_edit
- w:awx_action:devx.feedback_write
- w:awx_action:issuing_cardholders_edit
- w:awx_action:issuing_cards_edit
- w:awx_action:payment_links_edit
- w:org_action:billing.customer_edit
- w:org_action:billing.discount_edit
- w:org_action:billing.invoice_edit
- w:org_action:billing.price_edit
- w:org_action:billing.product_edit
- w:org_action:billing.subscription_edit
- w:org_action:billing.usage_metering_edit
- r:awx_action:balances_view
- r:awx_action:contact_management_view
- r:awx_action:conversions_view
- r:awx_action:deposits_view
- r:awx_action:direct_debits_view
- r:awx_action:global_accounts_view
- r:awx_action:issuing_cardholders_view
- r:awx_action:issuing_cards_view
- r:awx_action:issuing_transactions_view
- r:awx_action:linked_accounts_view
- r:awx_action:pa_view
- r:awx_action:payment_dispute_view
- r:awx_action:payment_links_view
- r:awx_action:settings.account_details_view
- r:awx_action:transfers_view
- r:org_action:billing.customer_view
- r:org_action:billing.discount_view
- r:org_action:billing.invoice_view
- r:org_action:billing.payment_source_view
- r:org_action:billing.price_view
- r:org_action:billing.product_view
- r:org_action:billing.subscription_view
- r:org_action:billing.transaction_view
- r:org_action:billing.usage_metering_view
- r:org_action:expense_management.expense:api_view
- r:org_action:spend.bills:api_view
- r:org_action:spend.vendors:api_view
- w:awx_action:contact_management_edit
- w:awx_action:conversions_edit
- w:awx_action:deposits_create
- w:awx_action:devx.feedback_write
- w:awx_action:issuing_cardholders_edit
- w:awx_action:issuing_cards_edit
- w:awx_action:linked_accounts_edit
- w:awx_action:pa_edit
- w:awx_action:payment_dispute_edit
- w:awx_action:payment_links_edit
- w:awx_action:simulation_edit
- w:awx_action:transfers_edit
- w:org_action:billing.checkout_edit
- w:org_action:billing.customer_edit
- w:org_action:billing.discount_edit
- w:org_action:billing.invoice_edit
- w:org_action:billing.price_edit
- w:org_action:billing.product_edit
- w:org_action:billing.subscription_edit
- w:org_action:billing.usage_metering_edit
scopes:
- description: ''
  flows: []
  scope: account_details:read
- description: ''
  flows: []
  scope: billing.checkout:read
- description: ''
  flows: []
  scope: billing.checkout:write
- description: ''
  flows: []
  scope: billing.customer:read
- description: ''
  flows: []
  scope: billing.customer:write
- description: ''
  flows: []
  scope: billing.transaction:read
- description: ''
  flows: []
  scope: billing.credit_note:read
- description: ''
  flows: []
  scope: billing.credit_note:write
- description: ''
  flows: []
  scope: billing.discount:read
- description: ''
  flows: []
  scope: billing.discount:write
- description: ''
  flows: []
  scope: billing.invoice:read
- description: ''
  flows: []
  scope: billing.invoice:write
- description: ''
  flows: []
  scope: billing.payment_source:read
- description: ''
  flows: []
  scope: billing.payment_source:write
- description: ''
  flows: []
  scope: billing.price:read
- description: ''
  flows: []
  scope: billing.price:write
- description: ''
  flows: []
  scope: billing.product:read
- description: ''
  flows: []
  scope: billing.product:write
- description: ''
  flows: []
  scope: billing.subscription:read
- description: ''
  flows: []
  scope: billing.subscription:write
- description: ''
  flows: []
  scope: billing.usage_metering:read
- description: ''
  flows: []
  scope: billing.usage_metering:write
- description: ''
  flows: []
  scope: balance:read
- description: ''
  flows: []
  scope: global_account:read
- description: ''
  flows: []
  scope: global_account:write
- description: ''
  flows: []
  scope: issuing.card:read
- description: ''
  flows: []
  scope: issuing.card:write
- description: ''
  flows: []
  scope: issuing.cardholder:read
- description: ''
  flows: []
  scope: issuing.cardholder:write
- description: ''
  flows: []
  scope: issuing.transaction:read
- description: ''
  flows: []
  scope: issuing.merchant_brand:read
- description: ''
  flows: []
  scope: financial_report:read
- description: ''
  flows: []
  scope: financial_report:write
- description: ''
  flows: []
  scope: financial_transaction:read
- description: ''
  flows: []
  scope: payment_link:read
- description: ''
  flows: []
  scope: payment_link:write
- description: ''
  flows: []
  scope: payment_acceptance:read
- description: ''
  flows: []
  scope: payment_acceptance:write
- description: ''
  flows: []
  scope: payment_dispute:read
- description: ''
  flows: []
  scope: payment_dispute:write
- description: ''
  flows: []
  scope: pos_terminal:read
- description: ''
  flows: []
  scope: pos_terminal:write
- description: ''
  flows: []
  scope: funds_split:write
- description: ''
  flows: []
  scope: funds_split:read
- description: ''
  flows: []
  scope: beneficiary:read
- description: ''
  flows: []
  scope: beneficiary:write
- description: ''
  flows: []
  scope: transfer:read
- description: ''
  flows: []
  scope: transfer:write
- description: ''
  flows: []
  scope: risk.rfi:read
- description: ''
  flows: []
  scope: risk.rfi:write
- description: ''
  flows: []
  scope: simulation:write
- description: ''
  flows: []
  scope: spend.bill:read
- description: ''
  flows: []
  scope: spend.bill:write
- description: ''
  flows: []
  scope: spend.expense:read
- description: ''
  flows: []
  scope: spend.expense:write
- description: ''
  flows: []
  scope: spend.purchase_order:read
- description: ''
  flows: []
  scope: spend.purchase_order:write
- description: ''
  flows: []
  scope: spend.vendor:read
- description: ''
  flows: []
  scope: spend.vendor:write
- description: ''
  flows: []
  scope: reference.order_item:read
- description: ''
  flows: []
  scope: reference.order_item:write
- description: ''
  flows: []
  scope: commerce_store:read
- description: ''
  flows: []
  scope: file:upload
- description: ''
  flows: []
  scope: fx.conversion:read
- description: ''
  flows: []
  scope: fx.conversion:write
- description: ''
  flows: []
  scope: Product
- description: ''
  flows: []
  scope: Accounts
- description: ''
  flows: []
  scope: Business Accounts
- description: ''
  flows: []
  scope: Business Accounts
- description: ''
  flows: []
  scope: Business Accounts
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Cards
- description: ''
  flows: []
  scope: Finance
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payments
- description: ''
  flows: []
  scope: Payouts
- description: ''
  flows: []
  scope: Payouts
- description: ''
  flows: []
  scope: Payouts
- description: ''
  flows: []
  scope: Payouts
- description: ''
  flows: []
  scope: Simulations
- description: ''
  flows: []
  scope: Supporting Services
- description: ''
  flows: []
  scope: Supporting Services
- description: ''
  flows: []
  scope: Supporting Services
- description: ''
  flows: []
  scope: Supporting Services
- description: ''
  flows: []
  scope: Transactional FX
- description: ''
  flows: []
  scope: Transactional FX
- description: ''
  flows: []
  scope: r:awx_action:balances_view
- description: ''
  flows: []
  scope: r:awx_action:contact_management_view
- description: ''
  flows: []
  scope: r:awx_action:conversions_view
- description: ''
  flows: []
  scope: r:awx_action:global_accounts_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_cardholders_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_cards_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_transactions_view
- description: ''
  flows: []
  scope: r:awx_action:pa_view
- description: ''
  flows: []
  scope: r:awx_action:payment_links_view
- description: ''
  flows: []
  scope: r:awx_action:settings.account_details_view
- description: ''
  flows: []
  scope: r:awx_action:transfers_view
- description: ''
  flows: []
  scope: r:org_action:billing.customer_view
- description: ''
  flows: []
  scope: r:org_action:billing.discount_view
- description: ''
  flows: []
  scope: r:org_action:billing.invoice_view
- description: ''
  flows: []
  scope: r:org_action:billing.payment_source_view
- description: ''
  flows: []
  scope: r:org_action:billing.price_view
- description: ''
  flows: []
  scope: r:org_action:billing.product_view
- description: ''
  flows: []
  scope: r:org_action:billing.subscription_view
- description: ''
  flows: []
  scope: r:org_action:billing.transaction_view
- description: ''
  flows: []
  scope: r:org_action:billing.usage_metering_view
- description: ''
  flows: []
  scope: r:org_action:expense_management.expense:api_view
- description: ''
  flows: []
  scope: r:org_action:spend.bills:api_view
- description: ''
  flows: []
  scope: r:org_action:spend.vendors:api_view
- description: ''
  flows: []
  scope: w:awx_action:contact_management_edit
- description: ''
  flows: []
  scope: w:awx_action:devx.feedback_write
- description: ''
  flows: []
  scope: w:awx_action:issuing_cardholders_edit
- description: ''
  flows: []
  scope: w:awx_action:issuing_cards_edit
- description: ''
  flows: []
  scope: w:awx_action:payment_links_edit
- description: ''
  flows: []
  scope: w:org_action:billing.customer_edit
- description: ''
  flows: []
  scope: w:org_action:billing.discount_edit
- description: ''
  flows: []
  scope: w:org_action:billing.invoice_edit
- description: ''
  flows: []
  scope: w:org_action:billing.price_edit
- description: ''
  flows: []
  scope: w:org_action:billing.product_edit
- description: ''
  flows: []
  scope: w:org_action:billing.subscription_edit
- description: ''
  flows: []
  scope: w:org_action:billing.usage_metering_edit
- description: ''
  flows: []
  scope: r:awx_action:balances_view
- description: ''
  flows: []
  scope: r:awx_action:contact_management_view
- description: ''
  flows: []
  scope: r:awx_action:conversions_view
- description: ''
  flows: []
  scope: r:awx_action:deposits_view
- description: ''
  flows: []
  scope: r:awx_action:direct_debits_view
- description: ''
  flows: []
  scope: r:awx_action:global_accounts_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_cardholders_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_cards_view
- description: ''
  flows: []
  scope: r:awx_action:issuing_transactions_view
- description: ''
  flows: []
  scope: r:awx_action:linked_accounts_view
- description: ''
  flows: []
  scope: r:awx_action:pa_view
- description: ''
  flows: []
  scope: r:awx_action:payment_dispute_view
- description: ''
  flows: []
  scope: r:awx_action:payment_links_view
- description: ''
  flows: []
  scope: r:awx_action:settings.account_details_view
- description: ''
  flows: []
  scope: r:awx_action:transfers_view
- description: ''
  flows: []
  scope: r:org_action:billing.customer_view
- description: ''
  flows: []
  scope: r:org_action:billing.discount_view
- description: ''
  flows: []
  scope: r:org_action:billing.invoice_view
- description: ''
  flows: []
  scope: r:org_action:billing.payment_source_view
- description: ''
  flows: []
  scope: r:org_action:billing.price_view
- description: ''
  flows: []
  scope: r:org_action:billing.product_view
- description: ''
  flows: []
  scope: r:org_action:billing.subscription_view
- description: ''
  flows: []
  scope: r:org_action:billing.transaction_view
- description: ''
  flows: []
  scope: r:org_action:billing.usage_metering_view
- description: ''
  flows: []
  scope: r:org_action:expense_management.expense:api_view
- description: ''
  flows: []
  scope: r:org_action:spend.bills:api_view
- description: ''
  flows: []
  scope: r:org_action:spend.vendors:api_view
- description: ''
  flows: []
  scope: w:awx_action:contact_management_edit
- description: ''
  flows: []
  scope: w:awx_action:conversions_edit
- description: ''
  flows: []
  scope: w:awx_action:deposits_create
- description: ''
  flows: []
  scope: w:awx_action:devx.feedback_write
- description: ''
  flows: []
  scope: w:awx_action:issuing_cardholders_edit
- description: ''
  flows: []
  scope: w:awx_action:issuing_cards_edit
- description: ''
  flows: []
  scope: w:awx_action:linked_accounts_edit
- description: ''
  flows: []
  scope: w:awx_action:pa_edit
- description: ''
  flows: []
  scope: w:awx_action:payment_dispute_edit
- description: ''
  flows: []
  scope: w:awx_action:payment_links_edit
- description: ''
  flows: []
  scope: w:awx_action:simulation_edit
- description: ''
  flows: []
  scope: w:awx_action:transfers_edit
- description: ''
  flows: []
  scope: w:org_action:billing.checkout_edit
- description: ''
  flows: []
  scope: w:org_action:billing.customer_edit
- description: ''
  flows: []
  scope: w:org_action:billing.discount_edit
- description: ''
  flows: []
  scope: w:org_action:billing.invoice_edit
- description: ''
  flows: []
  scope: w:org_action:billing.price_edit
- description: ''
  flows: []
  scope: w:org_action:billing.product_edit
- description: ''
  flows: []
  scope: w:org_action:billing.subscription_edit
- description: ''
  flows: []
  scope: w:org_action:billing.usage_metering_edit
slug: airwallex-scopes
source_filename: airwallex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes.md\ndocs: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes\nnote: Airwallex exposes TWO distinct OAuth scope vocabularies and both are real. (1) The partner-connections scope\n  reference documents 98 `<resource>:<read|write>` scopes for third-party applications, each row mapping the scope\n  to the REST operations it authorizes and the webhook events it may subscribe to. (2) The hosted MCP servers advertise\n  a different, coarser `<r|w>:<awx_action|org_action>:<permission>` vocabulary in their RFC 9728 protected-resource\n  metadata — 35 scopes on production, 48 in sandbox — fetched anonymously and saved verbatim under well-known/.\n  No oauth2 securityScheme appears in the OpenAPI held in this repo, so none of this is derivable from the spec;\n  every scope below was read off a provider surface.\nschemes:\n- name:\
  \ Airwallex Partner Connections OAuth\n  source: https://www.airwallex.com/docs/developer-tools/partner-connections/oauth-scopes\n  audience: third-party applications connecting to a merchant Airwallex account\n  consent_roles:\n  - Owner\n  - Admin\n  - Finance Admin\n  scope_count: 98\n- name: Airwallex AgentOS MCP (production)\n  source: https://mcp.airwallex.com/.well-known/oauth-protected-resource/mcp/\n  resource: https://mcp.airwallex.com/mcp\n  authorization_servers:\n  - https://mcp.airwallex.com/mcp\n  bearer_methods_supported:\n  - header\n  scope_count: 35\n- name: Airwallex Developer MCP (sandbox)\n  source: https://mcp.sandbox.airwallex.com/.well-known/oauth-protected-resource/developer/\n  resource: https://mcp.sandbox.airwallex.com/developer\n  authorization_servers:\n  - https://mcp.sandbox.airwallex.com/developer\n  bearer_methods_supported:\n  - header\n  scope_count: 47\nscopes:\n- scope: account_details:read\n  group: Accounts\n  scheme: Airwallex Partner Connections\
  \ OAuth\n  access: read\n  operations:\n  - Retrieve account details\n  webhook_events:\n  - account.active\n  - account.connected\n  - account.suspended\n  - account.action_required\n  - account.submitted\n- scope: billing.checkout:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Billing Checkout\n  - Get list of Billing Checkouts\n  webhook_events:\n  - billing_checkout.cancelled\n  - billing_checkout.completed\n  - billing_checkout.created\n- scope: billing.checkout:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Billing Checkout\n  - Retrieve a Billing Checkout\n  - Get list of Billing Checkouts\n  - Update a Billing Checkout\n  - Cancel a Billing Checkout\n  webhook_events:\n  - billing_checkout.cancelled\n  - billing_checkout.completed\n  - billing_checkout.created\n- scope: billing.customer:read\n  group: Billing\n  scheme: Airwallex Partner Connections\
  \ OAuth\n  access: read\n  operations:\n  - Retrieve a Billing Customer\n  - Get list of Billing Customers\n- scope: billing.customer:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Billing Customer\n  - Retrieve a Billing Customer\n  - Update a Billing Customer\n  - Get list of Billing Customers\n- scope: billing.transaction:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Billing Transaction\n  - Get list of Billing Transactions\n  webhook_events:\n  - billing_transaction.cancelled\n  - billing_transaction.created\n  - billing_transaction.succeeded\n- scope: billing.credit_note:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Credit Note\n  - Get list of Credit Notes\n  - Retrieve a Credit Note Line Item\n  - Get list of Credit Note Line Items\n  webhook_events:\n  - credit_note.created\n\
  \  - credit_note.finalized\n  - credit_note.voided\n- scope: billing.credit_note:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Credit Note\n  - Retrieve a Credit Note\n  - Get list of Credit Notes\n  - Update a Credit Note\n  - Finalize a Credit Note\n  - Delete a Credit Note\n  - Void a Credit Note\n  - Create Credit Note Line Items and add them to a Credit Note\n  - Retrieve a Credit Note Line Item\n  - Get list of Credit Note Line Items\n  - Update Credit Note Line Items in a Credit Note\n  - Delete Credit Note Line Items from a Credit Note\n  webhook_events:\n  - credit_note.created\n  - credit_note.finalized\n  - credit_note.voided\n- scope: billing.discount:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Coupon\n  - Get list of Coupons\n- scope: billing.discount:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access:\
  \ write\n  operations:\n  - Create a Coupon\n  - Update a Coupon\n  - Retrieve a Coupon\n  - Get list of Coupons\n- scope: billing.invoice:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve an Invoice\n  - Get list of Invoices\n  - Retrieve an Invoice Line Item\n  - Get list of Invoice Line Items\n  webhook_events:\n  - invoice.created\n  - invoice.finalized\n  - invoice.paid\n  - invoice.payment.paid\n  - invoice.payment_attempt_failed\n  - invoice.payment_failed\n  - invoice.sent\n  - invoice.voided\n- scope: billing.invoice:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create an Invoice\n  - Preview an Invoice\n  - Update an Invoice\n  - Delete a draft Invoice\n  - Retrieve an Invoice\n  - Get list of Invoices\n  - Finalize an Invoice\n  - Mark an Invoice as paid\n  - Void an Invoice\n  - Create Invoice Line Items and add them to an Invoice\n  - Retrieve an Invoice\
  \ Line Item\n  - Get list of Invoice Line Items\n  - Update Invoice Line Items in an Invoice\n  - Delete Invoice Line Items within an Invoice\n  webhook_events:\n  - invoice.created\n  - invoice.finalized\n  - invoice.paid\n  - invoice.payment.paid\n  - invoice.payment_attempt_failed\n  - invoice.payment_failed\n  - invoice.sent\n  - invoice.voided\n- scope: billing.payment_source:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Payment Source\n  - Get List of Payment Sources\n- scope: billing.payment_source:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Payment Source\n  - Retrieve a Payment Source\n  - Get List of Payment Sources\n- scope: billing.price:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Price\n  - Get list of Prices\n- scope: billing.price:write\n  group: Billing\n \
  \ scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Price\n  - Retrieve a Price\n  - Update a Price\n  - Get list of Prices\n- scope: billing.product:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Product\n  - Get list of Products\n- scope: billing.product:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Product\n  - Retrieve a Product\n  - Update a Product\n  - Get list of Products\n- scope: billing.subscription:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Subscription\n  - Get list of Subscriptions\n  - Retrieve a Subscription Item\n  - Get list of Subscription Items\n  webhook_events:\n  - subscription.active\n  - subscription.cancelled\n  - subscription.created\n  - subscription.in_trial\n  - subscription.modified\n  - subscription.unpaid\n\
  \  - subscription.updated\n- scope: billing.subscription:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Subscription\n  - Retrieve a Subscription\n  - Update a Subscription\n  - Cancel a Subscription\n  - Get list of Subscriptions\n  - Retrieve a Subscription Item\n  - Get list of Subscription Items\n  webhook_events:\n  - subscription.active\n  - subscription.cancelled\n  - subscription.created\n  - subscription.in_trial\n  - subscription.modified\n  - subscription.unpaid\n  - subscription.updated\n- scope: billing.usage_metering:read\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Meter\n  - Get list of Meters\n  - Get summaries of a Meter\n- scope: billing.usage_metering:write\n  group: Billing\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Meter\n  - Retrieve a Meter\n  - Update a Meter\n  - Archive a Meter\n\
  \  - Restore a Meter\n  - Get list of Meters\n  - Get summaries of a Meter\n  - Ingest a Usage Event\n  - Batch Ingest Usage Events\n  - Void a Usage Event\n  webhook_events:\n  - usage_event.aggregation_failed\n- scope: balance:read\n  group: Business Accounts\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get current balances\n  - Get balance history\n  webhook_events:\n  - balance.va.top_up\n  - balance.ga.top_up\n  - balance.adjustment\n- scope: global_account:read\n  group: Business Accounts\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get a list of global accounts\n  - Get a List of Direct Debit Payout Mandates\n  - Get a Direct Debit Payout Mandate by ID\n  - Get global account by ID\n  - Generate global account statement\n  - Get global account transactions\n  webhook_events:\n  - ga.new\n- scope: global_account:write\n  group: Business Accounts\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n\
  \  operations:\n  - Get a list of global accounts\n  - Create a global account\n  - Get a List of Direct Debit Payout Mandates\n  - Get a Direct Debit Payout Mandate by ID\n  - Cancel a Direct Debit Payout Mandate by ID\n  - Get global account by ID\n  - Close a global account\n  - Generate global account statement\n  - Get global account transactions\n  - Update existing global account\n  webhook_events:\n  - ga.new\n- scope: issuing.card:read\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get all cards\n  - Get card remaining limits\n  - Get issuing config\n  - Get card details\n  - Get sensitive card details\n  webhook_events:\n  - issuing.card_notification.created\n  - issuing.card_notification.physical_activated\n  - issuing.card.modified\n  - issuing.card.pending\n  - issuing.card.failed\n  - issuing.card.inactive\n  - issuing.card.active\n  - issuing.card.lost\n  - issuing.card.stolen\n  - issuing.card.closed\n  - issuing.card.blocked\n\
  \  - issuing.card.expired\n  - issuing.card.low_remaining_transaction_limit\n- scope: issuing.card:write\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a card\n  - Update a card\n  - Activate a card\n- scope: issuing.cardholder:read\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get all cardholders\n  - Get cardholder details\n  webhook_events:\n  - issuing.cardholder.deleted\n  - issuing.cardholder.disabled\n  - issuing.cardholder.incomplete\n  - issuing.cardholder.pending\n  - issuing.cardholder.ready\n- scope: issuing.cardholder:write\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a cardholder\n  - Update a cardholder\n  - Delete cardholder\n- scope: issuing.transaction:read\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get transactions\n  - Get single transaction\n\
  \  - Get authorization status\n  - Get single authorization status\n  - Get card transactions\n  - Get single card transaction\n  - Get card transaction events\n  - Get single card transaction event\n  - Get card transaction lifecycles\n  - Get single card transaction lifecycle\n  webhook_events:\n  - issuing.transaction.succeeded\n  - issuing.transaction.failed\n- scope: issuing.merchant_brand:read\n  group: Cards\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get single Merchant Brand by id\n  - Get all Merchant Brands matching query\n- scope: financial_report:read\n  group: Finance\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get list of financial reports\n  - Get financial report by ID\n  - Get contents of a financial report\n- scope: financial_report:write\n  group: Finance\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Get list of financial reports\n  - Create a financial\
  \ report\n  - Get financial report by ID\n  - Get contents of a financial report\n- scope: financial_transaction:read\n  group: Finance\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get list of financial transactions\n  - Get a financial transaction by ID\n- scope: payment_link:read\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a PaymentLink\n  - Get list of PaymentLinks\n- scope: payment_link:write\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Retrieve a PaymentLink\n  - Get list of PaymentLinks\n  - Create a PaymentLink\n  - Update a PaymentLink\n  - Send a PaymentLink\n  - Activate a PaymentLink\n  - Deactivate a PaymentLink\n- scope: payment_acceptance:read\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get list of PaymentIntents\n  - Retrieve a PaymentIntent\n  - Retrieve\
  \ list of PaymentAttempts\n  - Retrieve a PaymentAttempt by ID\n  - Get list of settlements\n  - Get a settlement by ID\n  - Get a settlement report by ID\n  - Get list of Refunds\n  - Retrieve a Refund\n  - Get available bank names\n  - Get available payment method types\n  - Get list of PaymentConsents\n  - Retrieve a PaymentConsent\n  - Get list of PaymentMethods\n  - Retrieve a PaymentMethod\n  - Get list of Customers\n  - Retrieve a Customer\n  - Generate a client secret for a Customer\n  - Get list of PaymentLinks\n  - Retrieve a PaymentLink\n  - Get convertible shopper currencies\n  - Get Apple Pay Domains\n  - Retrieve a Conversion Quote\n  - Retrieve BIN Info\n  webhook_events:\n  - payment_intent.created\n  - payment_intent.cancelled\n  - payment_intent.pending\n  - payment_intent.succeeded\n  - payment_intent.requires_payment_method\n  - payment_intent.requires_customer_action\n  - payment_intent.requires_capture\n  - payment_intent.payment_failed\n  - payment_attempt.received\n\
  \  - payment_attempt.risk_declined\n  - payment_attempt.pending_authorization\n  - payment_attempt.authorized\n  - payment_attempt.authorization_failed\n  - payment_attempt.capture_requested\n  - payment_attempt.capture_failed\n  - payment_attempt.authentication_redirected\n  - payment_attempt.authentication_failed\n  - payment_attempt.failed_to_process\n  - payment_attempt.cancelled\n  - payment_attempt.expired\n  - payment_attempt.settled\n  - payment_attempt.paid\n  - payment_method.created\n  - payment_method.updated\n  - payment_method.attached\n  - payment_method.detached\n  - payment_method.disabled\n  - customer.created\n  - customer.updated\n  - refund.received\n  - refund.accepted\n  - refund.settled\n  - refund.failed\n  - payment_consent.created\n  - payment_consent.updated\n  - payment_consent.pending\n  - payment_consent.verified\n  - payment_consent.disabled\n- scope: payment_acceptance:write\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n\
  \  operations:\n  - Create a PaymentIntent\n  - Cancel a PaymentIntent\n  - Capture a PaymentIntent\n  - Confirm a PaymentIntent\n  - Continue to confirm a PaymentIntent\n  - Create a Refund\n  - Add PaymentMethod to Customer\n  - Remove PaymentMethod from Customer\n  - Update a Customer\n  - Create a Customer\n  - Disable a PaymentConsent\n  - Update a PaymentConsent\n  - Verify a PaymentConsent\n  - Create a PaymentConsent\n  - Continue to verify a PaymentConsent\n  - Update a PaymentIntent\n  - Increment Authorization for a PaymentIntent\n  - Create a PaymentLink\n  - Update a PaymentLink\n  - Send a PaymentLink\n  - Activate a PaymentLink\n  - Deactivate a PaymentLink\n  - Create a Conversion Quote\n  - Add Apple Pay Domains\n  - Remove Apple Pay Domains\n  webhook_events:\n  - payment_intent.created\n  - payment_intent.cancelled\n  - payment_intent.pending\n  - payment_intent.succeeded\n  - payment_intent.requires_payment_method\n  - payment_intent.requires_customer_action\n  - payment_intent.requires_capture\n\
  \  - payment_intent.payment_failed\n  - payment_attempt.received\n  - payment_attempt.risk_declined\n  - payment_attempt.pending_authorization\n  - payment_attempt.authorized\n  - payment_attempt.authorization_failed\n  - payment_attempt.capture_requested\n  - payment_attempt.capture_failed\n  - payment_attempt.authentication_redirected\n  - payment_attempt.authentication_failed\n  - payment_attempt.failed_to_process\n  - payment_attempt.cancelled\n  - payment_attempt.expired\n  - payment_attempt.settled\n  - payment_attempt.paid\n  - payment_method.created\n  - payment_method.updated\n  - payment_method.attached\n  - payment_method.detached\n  - payment_method.disabled\n  - customer.created\n  - customer.updated\n  - refund.received\n  - refund.accepted\n  - refund.settled\n  - refund.failed\n  - payment_consent.created\n  - payment_consent.updated\n  - payment_consent.pending\n  - payment_consent.verified\n  - payment_consent.disabled\n- scope: payment_dispute:read\n  group: Payments\n\
  \  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a PaymentDispute\n  - Get list of PaymentDisputes\n  - Get list of Related Payment Intents\n  webhook_events:\n  - payment_dispute.requires_response\n  - payment_dispute.expired\n  - payment_dispute.accepted\n  - payment_dispute.challenged\n  - payment_dispute.reversed\n  - payment_dispute.pending_decision\n  - payment_dispute.pending_closure\n  - payment_dispute.won\n  - payment_dispute.lost\n- scope: payment_dispute:write\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Accept a PaymentDispute\n  - Challenge a PaymentDispute\n  - Retrieve a PaymentDispute\n  - Get list of PaymentDisputes\n  - Get list of Related Payment Intents\n  webhook_events:\n  - payment_dispute.requires_response\n  - payment_dispute.expired\n  - payment_dispute.accepted\n  - payment_dispute.challenged\n  - payment_dispute.reversed\n  - payment_dispute.pending_decision\n\
  \  - payment_dispute.pending_closure\n  - payment_dispute.won\n  - payment_dispute.lost\n- scope: pos_terminal:read\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a Terminal\n  - Get list of Terminals\n- scope: pos_terminal:write\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a Terminal\n  - Activate a Terminal\n  - Deactivate a Terminal\n  - Terminate a Terminal\n  - Update a Terminal\n  - Reset a Terminal password\n  - Process a PaymentIntent in a Terminal\n- scope: funds_split:write\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create a FundsSplitReversal\n  - Create a FundsSplit\n  - Release a FundsSplit\n- scope: funds_split:read\n  group: Payments\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a FundsSplitReversal\n  - Get list of FundsSplitReversals\n  -\
  \ Retrieve a FundsSplit\n  - Get list of FundsSplits\n  webhook_events:\n  - funds_split.created\n  - funds_split.failed\n  - funds_split.released\n  - funds_split.settled\n- scope: beneficiary:read\n  group: Payouts\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get list of beneficiaries\n  - Get a beneficiary by ID\n- scope: beneficiary:write\n  group: Payouts\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Get list of beneficiaries\n  - Get a beneficiary by ID\n  - Create a new beneficiary\n  - Delete existing beneficiary\n  - Update existing beneficiary\n  - Validate beneficiary\n  - Get the API schema\n  - Get the form schema\n  - Get supported financial institutions\n- scope: transfer:read\n  group: Payouts\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get list of transfers\n  - Get transfer by ID\n  - Supported currencies\n  - Retrieve a current rate\n  - Get list of wallet\
  \ transfers\n  - Get a wallet transfer with transfer ID\n  - List all batch transfers\n  - Retrieve a batch transfer\n  - List all items within a batch\n  webhook_events:\n  - payout.transfer.in_approval\n  - payout.transfer.approval_rejected\n  - payout.transfer.approval_blocked\n  - payout.transfer.approval_recalled\n  - payout.transfer.scheduled\n  - payout.transfer.overdue\n  - payout.transfer.processing\n  - payout.transfer.sent\n  - payout.transfer.paid\n  - payout.transfer.failed\n  - payout.transfer.cancellation_requested\n  - payout.transfer.cancelled\n  - payout.transfer.funding.requires_funding_confirmation\n  - payout.transfer.funding.scheduled\n  - payout.transfer.funding.processing\n  - payout.transfer.funding.funded\n  - payout.transfer.funding.reversed\n  - payout.transfer.funding.failed\n  - wallet_transfer.created\n  - wallet_transfer.processing\n  - wallet_transfer.sent\n  - wallet_transfer.settled\n  - wallet_transfer.failed\n  - batch_transfers.drafting\n  - batch_transfers.in_approval\n\
  \  - batch_transfers.approval_rejected\n  - batch_transfers.approval_blocked\n  - batch_transfers.approval_recalled\n  - batch_transfers.scheduled\n  - batch_transfers.funding.requires_funding_confirmation\n  - batch_transfers.funding.scheduled\n  - batch_transfers.funding.processing\n  - batch_transfers.funding.funded\n  - batch_transfers.funding.reversed\n  - batch_transfers.funding.failed\n  - batch_transfers.overdue\n  - batch_transfers.booking\n  - batch_transfers.partially_booked\n  - batch_transfers.booked\n  - batch_transfers.failed\n  - batch_transfers.cancellation_requested\n  - batch_transfers.cancelled\n- scope: transfer:write\n  group: Payouts\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Get list of transfers\n  - Get transfer by ID\n  - Cancel a transfer\n  - Confirm funding for a transfer\n  - Create a new transfer\n  - Validate transfer\n  - Supported currencies\n  - Retrieve a current rate\n  - Get list of wallet transfers\n  - Get\
  \ a wallet transfer with transfer ID\n  - Create a new wallet transfer\n  - List all batch transfers\n  - Retrieve a batch transfer\n  - List all items within a batch\n  - Create a batch transfer\n  - Add items to a batch\n  - Delete a batch transfer\n  - Delete items within a batch\n  - Quote a batch transfer\n  - Submit a batch transfer\n  webhook_events:\n  - payout.transfer.in_approval\n  - payout.transfer.approval_rejected\n  - payout.transfer.approval_blocked\n  - payout.transfer.approval_recalled\n  - payout.transfer.scheduled\n  - payout.transfer.overdue\n  - payout.transfer.processing\n  - payout.transfer.sent\n  - payout.transfer.paid\n  - payout.transfer.failed\n  - payout.transfer.cancellation_requested\n  - payout.transfer.cancelled\n  - payout.transfer.funding.requires_funding_confirmation\n  - payout.transfer.funding.scheduled\n  - payout.transfer.funding.processing\n  - payout.transfer.funding.funded\n  - payout.transfer.funding.reversed\n  - payout.transfer.funding.failed\n\
  \  - wallet_transfer.created\n  - wallet_transfer.processing\n  - wallet_transfer.sent\n  - wallet_transfer.settled\n  - wallet_transfer.failed\n  - batch_transfers.drafting\n  - batch_transfers.in_approval\n  - batch_transfers.approval_rejected\n  - batch_transfers.approval_blocked\n  - batch_transfers.approval_recalled\n  - batch_transfers.scheduled\n  - batch_transfers.funding.requires_funding_confirmation\n  - batch_transfers.funding.scheduled\n  - batch_transfers.funding.processing\n  - batch_transfers.funding.funded\n  - batch_transfers.funding.reversed\n  - batch_transfers.funding.failed\n  - batch_transfers.overdue\n  - batch_transfers.booking\n  - batch_transfers.partially_booked\n  - batch_transfers.booked\n  - batch_transfers.failed\n  - batch_transfers.cancellation_requested\n  - batch_transfers.cancelled\n- scope: risk.rfi:read\n  group: Risk\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - List all RFIs\n  - Retrieve an RFI\n  webhook_events:\n\
  \  - rfi.action_required\n  - rfi.answered\n  - rfi.closed\n- scope: risk.rfi:write\n  group: Risk\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - List all RFIs\n  - Retrieve an RFI\n  - Respond to an RFI\n  webhook_events:\n  - rfi.action_required\n  - rfi.answered\n  - rfi.closed\n- scope: simulation:write\n  group: Simulations\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Accounts\n  - Billing\n  - Deposits\n  - Issuing\n  - Linked Accounts\n  - Payment Acceptance\n  - Request for Information (RFI)\n  - Transfers\n- scope: spend.bill:read\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - List bills\n  - Get bill\n  webhook_events:\n  - spend.bill.awaiting_approval\n  - spend.bill.updated\n  - spend.bill.awaiting_payment\n  - spend.bill.payment_in_progress\n  - spend.bill.paid\n  - spend.bill.rejected\n  - spend.bill.scheduled\n  - spend.bill.deleted\n- scope: spend.bill:write\n\
  \  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create bill\n  - Update bill sync status\n  - Mark bill as paid\n- scope: spend.expense:read\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - List expenses\n  - Get expense\n  - List reimbursement reports\n  - Get reimbursement report\n  - List reimbursements\n  - Get reimbursement\n  - Get reimbursement report transfer\n  webhook_events:\n  - spend.expense.draft\n  - spend.expense.awaiting_approval\n  - spend.expense.updated\n  - spend.expense.rejected\n  - spend.expense.approved\n  - spend.expense.archived\n  - spend.expense.deleted\n  - spend.reimbursement_report.draft\n  - spend.reimbursement_report.awaiting_approval\n  - spend.reimbursement_report.awaiting_payment\n  - spend.reimbursement_report.rejected\n  - spend.reimbursement_report.payment_in_progress\n  - spend.reimbursement_report.paid\n  - spend.reimbursement_report.mark_as_paid\n\
  \  - spend.reimbursement_report.deleted\n  - spend.reimbursement_report.updated\n- scope: spend.expense:write\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Update expense sync status\n  - Update reimbursement report transfer sync status\n  - Update reimbursement report sync status\n  - Mark reimbursement report as paid\n- scope: spend.purchase_order:read\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - List purchase orders\n  - Get purchase order\n- scope: spend.purchase_order:write\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Create purchase order\n  - Update purchase order sync status\n- scope: spend.vendor:read\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - List vendors\n  - Get vendor\n- scope: spend.vendor:write\n  group: Spend\n  scheme: Airwallex Partner Connections OAuth\n\
  \  access: write\n  operations:\n  - Create vendor\n  - Update vendor sync status\n- scope: reference.order_item:read\n  group: Supporting Services\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get expiring transfer or deposit limit\n  - Get transfer or deposit limit\n- scope: reference.order_item:write\n  group: Supporting Services\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Increase transfer or deposit limit\n- scope: commerce_store:read\n  group: Supporting Services\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Get a list of e-commerce stores\n  - Get an e-commerce store by id\n- scope: file:upload\n  group: Supporting Services\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n  operations:\n  - Upload a file\n- scope: fx.conversion:read\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: read\n  operations:\n  - Retrieve a\
  \ conversion\n  - List all conversions\n  - Retrieve an amendment\n  - List all amendments\n  - Retrieve a quote\n  - Retrieve a current rate\n  webhook_events:\n  - conversion.scheduled\n  - conversion.overdue\n  - conversion.settled\n  - conversion.cancelled\n- scope: fx.conversion:write\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: write\n  operations:\n  - Retrieve a conversion\n  - List all conversions\n  - Create a conversion\n  - Create an amendment quote\n  - Create an amendment\n  - Retrieve an amendment\n  - List all amendments\n  - Retrieve a quote\n  - Create a quote\n  - Retrieve a current rate\n  webhook_events:\n  - conversion.scheduled\n  - conversion.overdue\n  - conversion.settled\n  - conversion.cancelled\n- scope: Product\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Accounts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope:\
  \ Business Accounts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Business Accounts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Business Accounts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Cards\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope:\
  \ Finance\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n\
  \  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payments\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payouts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payouts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payouts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Payouts\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Simulations\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Supporting Services\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Supporting Services\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope:\
  \ Supporting Services\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Supporting Services\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Transactional FX\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: Transactional FX\n  group: Transactional FX\n  scheme: Airwallex Partner Connections OAuth\n  access: other\n- scope: r:awx_action:balances_view\n  scheme: Airwallex AgentOS MCP (production)\n  access: read\n  method: probed\n- scope: r:awx_action:contact_management_view\n  scheme: Airwallex AgentOS MCP (production)\n  access: read\n  method: probed\n- scope: r:awx_action:conversions_view\n  scheme: Airwallex AgentOS MCP (production)\n  access: \n\n# --- truncated at 32 KB (41 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/scopes/airwallex-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/scopes/airwallex-scopes.yml
summary_line: 180 scopes
tags:
- Cross-Border Payments
- Fintech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
token_urls: []
---
