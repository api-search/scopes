---
api_specs:
- filename: slash-openapi-original.json
  format: json
  label: Slash Public API
  slug: slash-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/openapi/slash-openapi-original.json
authorization_urls: []
description: ''
docs: https://docs.slash.com/introduction
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Slash Scopes
name_suffix: OAuth Scopes
note: 'Slash''s public API authenticates primarily with API keys (X-API-Key), so the OpenAPI declares no oauth2 securityScheme and the derive-oauth-scopes pass found no flows. Slash DOES run a third-party OAuth/OIDC surface for developer applications: an OIDC discovery document plus a fine-grained permission-key model attached to developer applications. Both are captured below.'
overview: 'Slash uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Slash
provider_slug: slash
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: slash-scopes
source_filename: slash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.slash.com/.well-known/openid-configuration\ndocs: https://docs.slash.com/introduction\nnote: >-\n  Slash's public API authenticates primarily with API keys (X-API-Key), so the\n  OpenAPI declares no oauth2 securityScheme and the derive-oauth-scopes pass\n  found no flows. Slash DOES run a third-party OAuth/OIDC surface for developer\n  applications: an OIDC discovery document plus a fine-grained permission-key\n  model attached to developer applications. Both are captured below.\noidc:\n  issuer_host: https://api.slash.com\n  authorization_endpoint: https://app.slash.com/oauth2/authorize\n  token_endpoint: https://api.joinslash.com/oauth2/token\n  userinfo_endpoint: https://api.joinslash.com/oauth2/userinfo\n  response_types_supported: [code]\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  scopes_supported:\n    - scope: openid\n      description: OpenID Connect authentication; returns the subject\
  \ identifier.\n    - scope: offline_access\n      description: Issues a refresh token for long-lived access.\n    - scope: profile\n      description: Access to the user's basic profile claims.\n    - scope: email\n      description: Access to the user's email address.\n    - scope: phone\n      description: Access to the user's phone number.\n    - scope: address\n      description: Access to the user's address.\ndeveloper_application_permissions:\n  source: openapi/slash-openapi-original.json#/components/schemas\n  description: >-\n    Fine-grained permission keys a developer application requests over a legal\n    entity and its Slash accounts. Modeled as `.view` / `.modify` /\n    `.initiate` grants (the closest thing Slash has to OAuth scopes for\n    partner/third-party apps).\n  legal_entity_scopes:\n    - legal_entity.home.view\n    - legal_entity.view\n    - legal_entity.users.view\n    - legal_entity.users.modify\n    - legal_entity.users.card_groups.view\n    - legal_entity.users.card_groups.modify\n\
  \    - legal_entity.subscriptions.view\n    - legal_entity.subscriptions.modify\n    - legal_entity.accounting.view\n    - legal_entity.accounting.modify\n    - legal_entity.contacts.view\n    - legal_entity.contacts.modify\n    - legal_entity.third_party_credentials.view\n    - legal_entity.third_party_credentials.modify\n    - legal_entity.authorized_third_parties.view\n    - legal_entity.authorized_third_parties.modify\n    - legal_entity.api_key.view\n    - legal_entity.api_key.modify\n    - legal_entity.applications.view\n    - legal_entity.applications.modify\n    - legal_entity.permission_roles.view\n    - legal_entity.automation_rules.view\n    - legal_entity.automation_rules.modify\n    - legal_entity.developer_account.view\n    - legal_entity.developer_account.modify\n    - legal_entity.cashback.view\n    - legal_entity.cashback.modify\n    - legal_entity.webhooks.view\n    - legal_entity.webhooks.modify\n    - legal_entity.ticket_reconciliation.view\n    - legal_entity.analytics.view\n\
  \    - legal_entity.transactions.crypto_deposit.accelerate\n  slash_account_scopes:\n    - slash_accounts.view\n    - slash_accounts.home.view\n    - slash_accounts.cards.physical.view\n    - slash_accounts.cards.physical.modify\n    - slash_accounts.cards.virtual.view\n    - slash_accounts.cards.virtual.modify\n    - slash_accounts.incoming_transactions.view\n    - slash_accounts.transactions.view\n    - slash_accounts.transactions.ach_pull.initiate\n    - slash_accounts.transactions.ach_push.initiate\n    - slash_accounts.transactions.wire.initiate\n    - slash_accounts.transactions.between_accounts.initiate\n    - slash_accounts.transactions.rtp.initiate\n    - slash_accounts.balance.view\n    - slash_accounts.subaccounts.view\n    - slash_accounts.subaccounts.modify\n    - slash_accounts.merchant_allowlist.view\n    - slash_accounts.merchant_allowlist.modify\n    - slash_accounts.integrations.view\n    - slash_accounts.integrations.modify\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slash/refs/heads/main/scopes/slash-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Banking
- Payments
- Financial Services
- Fintech
- Corporate Cards
- Business Banking
- Invoicing
- Expense Management
- Treasury
- FDX
token_urls: []
---
