---
api_specs:
- filename: paxos-v2-openapi-original.json
  format: json
  label: Paxos API v2
  slug: paxos-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/openapi/paxos-v2-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.paxos.com/api-reference/introduction
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Paxos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paxos publishes 66 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paxos API on a user''s behalf.


  Tokens are issued from https://oauth.paxos.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paxos
provider_slug: paxos
schemes:
- description: 'Paxos APIs use [OAuth 2](https://tools.ietf.org/html/rfc6749) with the [client credentials](https://tools.ietf.org/html/rfc6749#section-4.4) grant flow.


    **Token URLs:**

    - Production: https://oauth.paxos.com/oauth2/token

    - Sandbox: https://oauth.sandbox.paxos.com/oauth2/token


    Learn more in the [API credentials guide →](https://docs.paxos.com/developer/credentials)'
  flows:
  - flow: clientCredentials
    tokenUrl: https://oauth.paxos.com/oauth2/token
  name: OAuth2
  source: openapi/paxos-v2-openapi-original.json
scope_count: 66
scope_names:
- address_ownership:read_verification
- address_ownership:write_verification
- api_creds:delete_credentials
- api_creds:read_credentials
- conversion:read_conversion_stablecoin
- conversion:write_conversion_stablecoin
- events:read_event
- exchange:historical_prices
- exchange:read_issuer_quote_execution
- exchange:read_order
- exchange:read_quote
- exchange:read_quote_execution
- exchange:write_issuer_quote
- exchange:write_issuer_quote_execution
- exchange:write_order
- exchange:write_quote_execution
- fee:write_crypto_withdrawal_fee
- funding:read_bank_balance
- funding:read_profile
- funding:write_profile
- identity:read_account
- identity:read_identity
- identity:read_identity_control
- identity:write_account
- identity:write_identity
- identity:write_identity_control
- orchestration:read_orchestration
- orchestration:read_orchestration_rule
- orchestration:write_orchestration
- orchestration:write_orchestration_rule
- rewards:create_payout_groups
- rewards:delete_payout_groups
- rewards:read_claims
- rewards:read_claims_schedule
- rewards:read_monitoring_address
- rewards:read_payout_groups
- rewards:read_rewards_details
- rewards:read_statements
- rewards:update_payout_groups
- rewards:write_claims_schedule
- rewards:write_monitoring_address
- rewards:write_payout_groups
- settlement:read_transaction
- settlement:write_transaction
- statements:read_payment
- statements:read_statement
- tax:read_tax_form
- tax:read_tax_lot
- tax:write_tax_lot
- transfer:read_crypto_destination_address
- transfer:read_deposit_address
- transfer:read_fiat_account
- transfer:read_fiat_deposit_instructions
- transfer:read_transfer
- transfer:read_transfer_limit
- transfer:reject_crypto_deposit
- transfer:update_crypto_deposit
- transfer:write_crypto_destination_address
- transfer:write_crypto_withdrawal
- transfer:write_deposit_address
- transfer:write_fiat_account
- transfer:write_fiat_deposit_instructions
- transfer:write_fiat_withdrawal
- transfer:write_internal_transfer
- transfer:write_paxos_transfer
- transfer:write_sandbox_fiat_deposit
scopes:
- description: ''
  flows: []
  scope: address_ownership:read_verification
- description: ''
  flows: []
  scope: address_ownership:write_verification
- description: ''
  flows: []
  scope: api_creds:delete_credentials
- description: ''
  flows: []
  scope: api_creds:read_credentials
- description: Retrieve stablecoin conversion details
  flows:
  - clientCredentials
  scope: conversion:read_conversion_stablecoin
- description: Create or cancel a stablecoin conversion
  flows:
  - clientCredentials
  scope: conversion:write_conversion_stablecoin
- description: Retrieve events
  flows:
  - clientCredentials
  scope: events:read_event
- description: Retrieve marketnaverage prices at a certain time increment
  flows:
  - clientCredentials
  scope: exchange:historical_prices
- description: ''
  flows: []
  scope: exchange:read_issuer_quote_execution
- description: Retrieve order or order execution details
  flows:
  - clientCredentials
  scope: exchange:read_order
- description: Retrieve quote details for buying or selling an asset
  flows:
  - clientCredentials
  scope: exchange:read_quote
- description: Retrieve quote execution details
  flows:
  - clientCredentials
  scope: exchange:read_quote_execution
- description: ''
  flows: []
  scope: exchange:write_issuer_quote
- description: ''
  flows: []
  scope: exchange:write_issuer_quote_execution
- description: Create or cancel an order for buying or selling an asset
  flows:
  - clientCredentials
  scope: exchange:write_order
- description: Create a quote execution for buying or selling an asset
  flows:
  - clientCredentials
  scope: exchange:write_quote_execution
- description: Create a guaranteed fee for crypto withdrawal
  flows:
  - clientCredentials
  scope: fee:write_crypto_withdrawal_fee
- description: Retrieve Paxos dedicated bank account balance
  flows:
  - clientCredentials
  scope: funding:read_bank_balance
- description: Retrieve Profile details and deposit funds in Sandbox
  flows:
  - clientCredentials
  scope: funding:read_profile
- description: Create a Profile
  flows:
  - clientCredentials
  scope: funding:write_profile
- description: Retrieve Account details
  flows:
  - clientCredentials
  scope: identity:read_account
- description: Retrieve Identity details or documents
  flows:
  - clientCredentials
  scope: identity:read_identity
- description: ''
  flows: []
  scope: identity:read_identity_control
- description: Create or update Account and Account Members
  flows:
  - clientCredentials
  scope: identity:write_account
- description: Create or update Identity details and set Sandbox Identify Status
  flows:
  - clientCredentials
  scope: identity:write_identity
- description: ''
  flows: []
  scope: identity:write_identity_control
- description: ''
  flows: []
  scope: orchestration:read_orchestration
- description: ''
  flows: []
  scope: orchestration:read_orchestration_rule
- description: ''
  flows: []
  scope: orchestration:write_orchestration
- description: ''
  flows: []
  scope: orchestration:write_orchestration_rule
- description: ''
  flows: []
  scope: rewards:create_payout_groups
- description: ''
  flows: []
  scope: rewards:delete_payout_groups
- description: ''
  flows: []
  scope: rewards:read_claims
- description: ''
  flows: []
  scope: rewards:read_claims_schedule
- description: ''
  flows: []
  scope: rewards:read_monitoring_address
- description: ''
  flows: []
  scope: rewards:read_payout_groups
- description: ''
  flows: []
  scope: rewards:read_rewards_details
- description: ''
  flows: []
  scope: rewards:read_statements
- description: ''
  flows: []
  scope: rewards:update_payout_groups
- description: ''
  flows: []
  scope: rewards:write_claims_schedule
- description: ''
  flows: []
  scope: rewards:write_monitoring_address
- description: ''
  flows: []
  scope: rewards:write_payout_groups
- description: Retrieve settlement transaction details
  flows:
  - clientCredentials
  scope: settlement:read_transaction
- description: Create, affirm or cancel a settlement transaction
  flows:
  - clientCredentials
  scope: settlement:write_transaction
- description: ''
  flows: []
  scope: statements:read_payment
- description: ''
  flows: []
  scope: statements:read_statement
- description: Retrieve tax details
  flows:
  - clientCredentials
  scope: tax:read_tax_form
- description: Retrieve tax lot details
  flows:
  - clientCredentials
  scope: tax:read_tax_lot
- description: Update the given tax-lot ID
  flows:
  - clientCredentials
  scope: tax:write_tax_lot
- description: ''
  flows: []
  scope: transfer:read_crypto_destination_address
- description: Retrieve deposit address details
  flows:
  - clientCredentials
  scope: transfer:read_deposit_address
- description: Retrieve Fiat Account details
  flows:
  - clientCredentials
  scope: transfer:read_fiat_account
- description: Retrieve fiat deposit instruction details
  flows:
  - clientCredentials
  scope: transfer:read_fiat_deposit_instructions
- description: Retrieve transfer details
  flows:
  - clientCredentials
  scope: transfer:read_transfer
- description: Retrieve limits for the given transaction type
  flows:
  - clientCredentials
  scope: transfer:read_transfer_limit
- description: Reject a crypto deposit (travel rule)
  flows:
  - clientCredentials
  scope: transfer:reject_crypto_deposit
- description: Provide required travel-rule details
  flows:
  - clientCredentials
  scope: transfer:update_crypto_deposit
- description: ''
  flows: []
  scope: transfer:write_crypto_destination_address
- description: Withdraw asset to a specified destination address
  flows:
  - clientCredentials
  scope: transfer:write_crypto_withdrawal
- description: Create an deposit address on a blockchain network
  flows:
  - clientCredentials
  scope: transfer:write_deposit_address
- description: Create, update or delete a Fiat Account
  flows:
  - clientCredentials
  scope: transfer:write_fiat_account
- description: Create, update or delete fiat deposit instructions
  flows:
  - clientCredentials
  scope: transfer:write_fiat_deposit_instructions
- description: Withdraw fiat to the given destination
  flows:
  - clientCredentials
  scope: transfer:write_fiat_withdrawal
- description: Transfer assets between two Profiles
  flows:
  - clientCredentials
  scope: transfer:write_internal_transfer
- description: ''
  flows: []
  scope: transfer:write_paxos_transfer
- description: Initiate a test fiat deposit in the Sandbox environment
  flows:
  - clientCredentials
  scope: transfer:write_sandbox_fiat_deposit
slug: paxos-scopes
source_filename: paxos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/paxos-v2-openapi-original.json\ndocs: https://docs.paxos.com/api-reference/introduction\nauthorization_endpoint: https://oauth.paxos.com/oauth2/auth\ntoken_endpoint: https://oauth.paxos.com/oauth2/token\nschemes:\n- name: OAuth2\n  source: openapi/paxos-v2-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.paxos.com/oauth2/token\n  description: |-\n    Paxos APIs use [OAuth 2](https://tools.ietf.org/html/rfc6749) with the [client credentials](https://tools.ietf.org/html/rfc6749#section-4.4) grant flow.\n\n    **Token URLs:**\n    - Production: https://oauth.paxos.com/oauth2/token\n    - Sandbox: https://oauth.sandbox.paxos.com/oauth2/token\n\n    Learn more in the [API credentials guide →](https://docs.paxos.com/developer/credentials)\nscopes:\n- scope: address_ownership:read_verification\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: address_ownership:write_verification\n\
  \  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: api_creds:delete_credentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: api_creds:read_credentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: conversion:read_conversion_stablecoin\n  description: Retrieve stablecoin conversion details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: conversion:write_conversion_stablecoin\n  description: Create or cancel a stablecoin conversion\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: events:read_event\n  description: Retrieve events\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:historical_prices\n  description: Retrieve marketnaverage prices at a certain time increment\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:read_issuer_quote_execution\n\
  \  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:read_order\n  description: Retrieve order or order execution details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:read_quote\n  description: Retrieve quote details for buying or selling an asset\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:read_quote_execution\n  description: Retrieve quote execution details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:write_issuer_quote\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:write_issuer_quote_execution\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: exchange:write_order\n  description: Create or cancel an order for buying or selling an asset\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope:\
  \ exchange:write_quote_execution\n  description: Create a quote execution for buying or selling an asset\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: fee:write_crypto_withdrawal_fee\n  description: Create a guaranteed fee for crypto withdrawal\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: funding:read_bank_balance\n  description: Retrieve Paxos dedicated bank account balance\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: funding:read_profile\n  description: Retrieve Profile details and deposit funds in Sandbox\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: funding:write_profile\n  description: Create a Profile\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:read_account\n  description: Retrieve Account details\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:read_identity\n  description: Retrieve Identity details or documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:read_identity_control\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:write_account\n  description: Create or update Account and Account Members\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:write_identity\n  description: Create or update Identity details and set Sandbox Identify Status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: identity:write_identity_control\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: orchestration:read_orchestration\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: orchestration:read_orchestration_rule\n  sources:\n\
  \  - openapi/paxos-v2-openapi-original.json\n- scope: orchestration:write_orchestration\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: orchestration:write_orchestration_rule\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:create_payout_groups\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:delete_payout_groups\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_claims\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_claims_schedule\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_monitoring_address\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_payout_groups\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_rewards_details\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:read_statements\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope:\
  \ rewards:update_payout_groups\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:write_claims_schedule\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:write_monitoring_address\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: rewards:write_payout_groups\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: settlement:read_transaction\n  description: Retrieve settlement transaction details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: settlement:write_transaction\n  description: Create, affirm or cancel a settlement transaction\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: statements:read_payment\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: statements:read_statement\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: tax:read_tax_form\n  description: Retrieve tax details\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: tax:read_tax_lot\n  description: Retrieve tax lot details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: tax:write_tax_lot\n  description: Update the given tax-lot ID\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_crypto_destination_address\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_deposit_address\n  description: Retrieve deposit address details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_fiat_account\n  description: Retrieve Fiat Account details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_fiat_deposit_instructions\n  description: Retrieve fiat deposit instruction details\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_transfer\n  description: Retrieve transfer details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:read_transfer_limit\n  description: Retrieve limits for the given transaction type\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:reject_crypto_deposit\n  description: Reject a crypto deposit (travel rule)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:update_crypto_deposit\n  description: Provide required travel-rule details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_crypto_destination_address\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_crypto_withdrawal\n  description: Withdraw asset to a specified destination address\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_deposit_address\n  description: Create an deposit address on a blockchain network\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_fiat_account\n  description: Create, update or delete a Fiat Account\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_fiat_deposit_instructions\n  description: Create, update or delete fiat deposit instructions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_fiat_withdrawal\n  description: Withdraw fiat to the given destination\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_internal_transfer\n  description: Transfer assets between two Profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n\
  - scope: transfer:write_paxos_transfer\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n- scope: transfer:write_sandbox_fiat_deposit\n  description: Initiate a test fiat deposit in the Sandbox environment\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/paxos-v2-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/scopes/paxos-scopes.yml
summary_line: 66 scopes · clientCredentials
tags:
- Company
- Stablecoins
- Cryptocurrency
- Payments
- Crypto Brokerage
- Trading
- Custody
- Blockchain
- Financial Services
- Digital Assets
token_urls:
- https://oauth.paxos.com/oauth2/token
---
