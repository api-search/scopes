---
api_specs:
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-webhooks-asyncapi.yml
  format: yaml
  label: Braintree Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/asyncapi/braintree-webhooks-asyncapi.yml
- filename: braintree-payments-openapi.yml
  format: yaml
  label: Braintree Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-payments-openapi.yml
- filename: braintree-subscriptions-openapi.yml
  format: yaml
  label: Braintree Subscriptions API
  slug: subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/openapi/braintree-subscriptions-openapi.yml
authorization_urls: []
description: Braintree's OAuth 2.0 scopes. The core gateway authenticates with HTTP Basic API keys, so the OpenAPI securitySchemes declare no oauth2 flows and the derive pass finds none. OAuth is used by platforms/partners to connect separate Braintree accounts — on its own or with the Grant API and Shared Vault. The connect URL is generated server-side via the SDK (gateway.oauth.connectUrl), and the access token is exchanged from the returned authorization code; scopes are requested as a comma-delimited string (e.g. grant_payment_method,shared_vault_transactions).
docs: https://developer.paypal.com/braintree/docs/guides/extend/oauth/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Braintree Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'braintree publishes 40 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the braintree API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: braintree
provider_slug: braintree
schemes:
- connect_url_note: Generated server-side via gateway.oauth.connectUrl(redirectUri, scope, state).
  docs: https://developer.paypal.com/braintree/docs/guides/extend/oauth/reference
  grant_types:
  - authorization_code
  - refresh_token
  name: Braintree OAuth
  notes: Scopes are requested as a comma-delimited string on the connect URL. Coarse connect-flow scopes (below) plus a fine-grained per-resource permission model are both documented.
  token_note: Access token created from the authorization code via the server SDK (createTokenFromCode).
  type: oauth2
scope_count: 40
scope_names:
- shared_vault_transactions
- grant_payment_method
- read_facilitated_transactions
- view_facilitated_transaction_metrics
- transaction:sale
- transaction:refund
- transaction:void
- transaction:find
- transaction:search
- transaction:clone
- transaction:manage_escrow
- transaction:manage_settlement
- customer:create
- customer:update
- customer:delete
- customer:find
- customer:search
- payment_method:create
- payment_method:update
- payment_method:delete
- payment_method:find
- subscription:create
- subscription:update
- subscription:cancel
- subscription:find
- subscription:search
- address:create
- address:update
- address:delete
- address:find
- dispute:find
- dispute:search
- dispute:accept
- dispute:finalize
- dispute:add_evidence
- dispute:remove_evidence
- client_token:generate
- credit_card_verification:search
- credit_card:expiring_between
- apple_pay:manage_web_domains
scopes:
- description: Create transactions for a connected merchant using payment methods stored in the platform's own Shared Vault.
  flows: []
  scope: shared_vault_transactions
- description: Grant a customer's vaulted payment method from one account to another via the Grant API.
  flows: []
  scope: grant_payment_method
- description: Read transactions facilitated on behalf of connected merchants.
  flows: []
  scope: read_facilitated_transactions
- description: View aggregated metrics for facilitated transactions.
  flows: []
  scope: view_facilitated_transaction_metrics
- description: Create sale transactions.
  flows: []
  scope: transaction:sale
- description: Refund transactions.
  flows: []
  scope: transaction:refund
- description: Void transactions.
  flows: []
  scope: transaction:void
- description: Retrieve a transaction.
  flows: []
  scope: transaction:find
- description: Search transactions.
  flows: []
  scope: transaction:search
- description: Clone a transaction.
  flows: []
  scope: transaction:clone
- description: Manage escrow (hold/release) on marketplace transactions.
  flows: []
  scope: transaction:manage_escrow
- description: Manage settlement of transactions.
  flows: []
  scope: transaction:manage_settlement
- description: Create customers.
  flows: []
  scope: customer:create
- description: Update customers.
  flows: []
  scope: customer:update
- description: Delete customers.
  flows: []
  scope: customer:delete
- description: Retrieve a customer.
  flows: []
  scope: customer:find
- description: Search customers.
  flows: []
  scope: customer:search
- description: Vault a payment method.
  flows: []
  scope: payment_method:create
- description: Update a vaulted payment method.
  flows: []
  scope: payment_method:update
- description: Delete a vaulted payment method.
  flows: []
  scope: payment_method:delete
- description: Retrieve a vaulted payment method.
  flows: []
  scope: payment_method:find
- description: Create subscriptions.
  flows: []
  scope: subscription:create
- description: Update subscriptions.
  flows: []
  scope: subscription:update
- description: Cancel subscriptions.
  flows: []
  scope: subscription:cancel
- description: Retrieve a subscription.
  flows: []
  scope: subscription:find
- description: Search subscriptions.
  flows: []
  scope: subscription:search
- description: Create customer addresses.
  flows: []
  scope: address:create
- description: Update customer addresses.
  flows: []
  scope: address:update
- description: Delete customer addresses.
  flows: []
  scope: address:delete
- description: Retrieve a customer address.
  flows: []
  scope: address:find
- description: Retrieve a dispute.
  flows: []
  scope: dispute:find
- description: Search disputes.
  flows: []
  scope: dispute:search
- description: Accept a dispute.
  flows: []
  scope: dispute:accept
- description: Finalize a dispute.
  flows: []
  scope: dispute:finalize
- description: Add evidence to a dispute.
  flows: []
  scope: dispute:add_evidence
- description: Remove evidence from a dispute.
  flows: []
  scope: dispute:remove_evidence
- description: Generate client tokens for client SDK initialization.
  flows: []
  scope: client_token:generate
- description: Search credit card verifications.
  flows: []
  scope: credit_card_verification:search
- description: Find credit cards expiring within a date range.
  flows: []
  scope: credit_card:expiring_between
- description: Manage registered Apple Pay web domains.
  flows: []
  scope: apple_pay:manage_web_domains
slug: braintree-scopes
source_filename: braintree-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-14'\nmethod: searched\nsource: https://developer.paypal.com/braintree/docs/guides/extend/oauth/reference\ndocs: https://developer.paypal.com/braintree/docs/guides/extend/oauth/overview\ndescription: >-\n  Braintree's OAuth 2.0 scopes. The core gateway authenticates with HTTP Basic\n  API keys, so the OpenAPI securitySchemes declare no oauth2 flows and the derive\n  pass finds none. OAuth is used by platforms/partners to connect separate\n  Braintree accounts — on its own or with the Grant API and Shared Vault. The\n  connect URL is generated server-side via the SDK (gateway.oauth.connectUrl),\n  and the access token is exchanged from the returned authorization code; scopes\n  are requested as a comma-delimited string (e.g. grant_payment_method,shared_vault_transactions).\nschemes:\n  - name: Braintree OAuth\n    type: oauth2\n    grant_types: [authorization_code, refresh_token]\n    connect_url_note: Generated server-side via gateway.oauth.connectUrl(redirectUri,\
  \ scope, state).\n    token_note: Access token created from the authorization code via the server SDK (createTokenFromCode).\n    docs: https://developer.paypal.com/braintree/docs/guides/extend/oauth/reference\n    notes: >-\n      Scopes are requested as a comma-delimited string on the connect URL.\n      Coarse connect-flow scopes (below) plus a fine-grained per-resource\n      permission model are both documented.\nscopes:\n  # Cross-account / platform scopes\n  - {scope: shared_vault_transactions, description: 'Create transactions for a connected merchant using payment methods stored in the platform''s own Shared Vault.', schemes: [Braintree OAuth]}\n  - {scope: grant_payment_method, description: 'Grant a customer''s vaulted payment method from one account to another via the Grant API.', schemes: [Braintree OAuth]}\n  - {scope: read_facilitated_transactions, description: 'Read transactions facilitated on behalf of connected merchants.', schemes: [Braintree OAuth]}\n  - {scope: view_facilitated_transaction_metrics,\
  \ description: 'View aggregated metrics for facilitated transactions.', schemes: [Braintree OAuth]}\n  # Fine-grained resource permission scopes\n  - {scope: 'transaction:sale', description: 'Create sale transactions.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:refund', description: 'Refund transactions.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:void', description: 'Void transactions.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:find', description: 'Retrieve a transaction.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:search', description: 'Search transactions.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:clone', description: 'Clone a transaction.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:manage_escrow', description: 'Manage escrow (hold/release) on marketplace transactions.', schemes: [Braintree OAuth]}\n  - {scope: 'transaction:manage_settlement', description: 'Manage settlement of transactions.', schemes: [Braintree\
  \ OAuth]}\n  - {scope: 'customer:create', description: 'Create customers.', schemes: [Braintree OAuth]}\n  - {scope: 'customer:update', description: 'Update customers.', schemes: [Braintree OAuth]}\n  - {scope: 'customer:delete', description: 'Delete customers.', schemes: [Braintree OAuth]}\n  - {scope: 'customer:find', description: 'Retrieve a customer.', schemes: [Braintree OAuth]}\n  - {scope: 'customer:search', description: 'Search customers.', schemes: [Braintree OAuth]}\n  - {scope: 'payment_method:create', description: 'Vault a payment method.', schemes: [Braintree OAuth]}\n  - {scope: 'payment_method:update', description: 'Update a vaulted payment method.', schemes: [Braintree OAuth]}\n  - {scope: 'payment_method:delete', description: 'Delete a vaulted payment method.', schemes: [Braintree OAuth]}\n  - {scope: 'payment_method:find', description: 'Retrieve a vaulted payment method.', schemes: [Braintree OAuth]}\n  - {scope: 'subscription:create', description: 'Create subscriptions.',\
  \ schemes: [Braintree OAuth]}\n  - {scope: 'subscription:update', description: 'Update subscriptions.', schemes: [Braintree OAuth]}\n  - {scope: 'subscription:cancel', description: 'Cancel subscriptions.', schemes: [Braintree OAuth]}\n  - {scope: 'subscription:find', description: 'Retrieve a subscription.', schemes: [Braintree OAuth]}\n  - {scope: 'subscription:search', description: 'Search subscriptions.', schemes: [Braintree OAuth]}\n  - {scope: 'address:create', description: 'Create customer addresses.', schemes: [Braintree OAuth]}\n  - {scope: 'address:update', description: 'Update customer addresses.', schemes: [Braintree OAuth]}\n  - {scope: 'address:delete', description: 'Delete customer addresses.', schemes: [Braintree OAuth]}\n  - {scope: 'address:find', description: 'Retrieve a customer address.', schemes: [Braintree OAuth]}\n  - {scope: 'dispute:find', description: 'Retrieve a dispute.', schemes: [Braintree OAuth]}\n  - {scope: 'dispute:search', description: 'Search disputes.',\
  \ schemes: [Braintree OAuth]}\n  - {scope: 'dispute:accept', description: 'Accept a dispute.', schemes: [Braintree OAuth]}\n  - {scope: 'dispute:finalize', description: 'Finalize a dispute.', schemes: [Braintree OAuth]}\n  - {scope: 'dispute:add_evidence', description: 'Add evidence to a dispute.', schemes: [Braintree OAuth]}\n  - {scope: 'dispute:remove_evidence', description: 'Remove evidence from a dispute.', schemes: [Braintree OAuth]}\n  - {scope: 'client_token:generate', description: 'Generate client tokens for client SDK initialization.', schemes: [Braintree OAuth]}\n  - {scope: 'credit_card_verification:search', description: 'Search credit card verifications.', schemes: [Braintree OAuth]}\n  - {scope: 'credit_card:expiring_between', description: 'Find credit cards expiring within a date range.', schemes: [Braintree OAuth]}\n  - {scope: 'apple_pay:manage_web_domains', description: 'Manage registered Apple Pay web domains.', schemes: [Braintree OAuth]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintree/refs/heads/main/scopes/braintree-scopes.yml
summary_line: 40 scopes
tags: []
token_urls: []
---
