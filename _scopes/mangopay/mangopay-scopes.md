---
authorization_urls: []
description: ''
docs: https://docs.mangopay.com/api-reference/overview/api-keys/scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Mangopay Scopes
name_suffix: OAuth Scopes
note: Mangopay uses OAuth 2.0 client_credentials, but access is governed by permission scopes assigned to the API key (not requested in the token call); each scope grants READ (GET) and/or WRITE (POST/PUT) access to a fixed group of endpoints (https://docs.mangopay.com/api-reference/overview/api-keys).
overview: 'Mangopay publishes 20 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mangopay API on a user''s behalf.


  Tokens are issued from https://api.mangopay.com/v2.01/{clientId}/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mangopay
provider_slug: mangopay
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.mangopay.com/v2.01/{clientId}/oauth/token
  name: OAuth2
  source: openapi/openapi.json
scope_count: 20
scope_names:
- Bankaccounts
- Client.Details
- Client.Developers
- Client.PayIns
- Client.Reports
- Client.Wallets
- Conversions
- Disputes.General
- Disputes.Settlement
- Payins
- Payouts
- Refunds.General
- Refunds.Payins
- Refunds.Payouts
- Refunds.Repudiations
- Refunds.Transfers
- Transfers
- Users.Details
- Users.Verification
- Wallet.Details
scopes:
- description: Manage recipients and bank accounts (IBAN, US, CA, GB, OTHER) — validate and create recipients and bank accounts, deactivate them, view payout methods and recipient schemas, and list transactions for a bank account.
  flows: []
  scope: Bankaccounts
- description: Update client information and upload the client logo; view client details.
  flows: []
  scope: Client.Details
- description: Manage webhooks (create and update hooks) and view hooks, events, and API responses for monitoring.
  flows: []
  scope: Client.Developers
- description: Create a bank wire pay-in to the repudiation wallet (write only; no read endpoints).
  flows: []
  scope: Client.PayIns
- description: Create transactions and wallets reports; view and list reports.
  flows: []
  scope: Client.Reports
- description: View and list client wallets (including by funds type) and list transactions for a client wallet (read only; no write endpoints).
  flows: []
  scope: Client.Wallets
- description: Create quotes and quoted or instant currency conversions between user or client wallets; view indicative conversion rates, quotes, and conversions.
  flows: []
  scope: Conversions
- description: Manage the dispute lifecycle — submit, update, and close disputes, create and submit dispute documents and pages; view and list disputes, dispute documents, repudiations, and dispute transactions.
  flows: []
  scope: Disputes.General
- description: Create and view settlement transfers related to disputes.
  flows: []
  scope: Disputes.Settlement
- description: Create and manage pay-ins across all payment methods — card registrations, tokenization, and validations, direct/web card pay-ins, recurring pay-ins, preauthorizations, deposit preauthorizations, bank wires, banking aliases, mandates, direct debits, and local/alternative methods (Apple Pay, Google Pay, PayPal, Klarna, iDEAL, Bancontact, Bizum, BLIK, Giropay, etc.).
  flows: []
  scope: Payins
- description: Create payouts and check instant payout eligibility; view payouts.
  flows: []
  scope: Payouts
- description: View refund details.
  flows: []
  scope: Refunds.General
- description: Create and list refunds for pay-in transactions.
  flows: []
  scope: Refunds.Payins
- description: List refunds for payout transactions.
  flows: []
  scope: Refunds.Payouts
- description: List refunds associated with repudiations (disputes).
  flows: []
  scope: Refunds.Repudiations
- description: Create and list refunds for transfer operations.
  flows: []
  scope: Refunds.Transfers
- description: Create transfers between wallets and view transfer details.
  flows: []
  scope: Transfers
- description: Create, update, and categorize natural and legal users; view and list users and their details.
  flows: []
  scope: Users.Details
- description: Conduct identity verification — KYC documents and pages, UBO declarations, and related verification endpoints.
  flows: []
  scope: Users.Verification
- description: Create and update user wallets; view and list wallets and list transactions for a wallet and a user.
  flows: []
  scope: Wallet.Details
slug: mangopay-scopes
source_filename: mangopay-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/openapi.json\ndocs: https://docs.mangopay.com/api-reference/overview/api-keys/scopes\nnote: Mangopay uses OAuth 2.0 client_credentials, but access is governed by permission\n  scopes assigned to the API key (not requested in the token call); each scope grants\n  READ (GET) and/or WRITE (POST/PUT) access to a fixed group of endpoints\n  (https://docs.mangopay.com/api-reference/overview/api-keys).\nschemes:\n- name: OAuth2\n  source: openapi/openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mangopay.com/v2.01/{clientId}/oauth/token\nscopes:\n- scope: Bankaccounts\n  description: Manage recipients and bank accounts (IBAN, US, CA, GB, OTHER) — validate\n    and create recipients and bank accounts, deactivate them, view payout methods\n    and recipient schemas, and list transactions for a bank account.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope:\
  \ Client.Details\n  description: Update client information and upload the client logo; view client\n    details.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Client.Developers\n  description: Manage webhooks (create and update hooks) and view hooks, events,\n    and API responses for monitoring.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Client.PayIns\n  description: Create a bank wire pay-in to the repudiation wallet (write only; no\n    read endpoints).\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Client.Reports\n  description: Create transactions and wallets reports; view and list reports.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Client.Wallets\n  description: View and list client wallets (including by funds type) and list transactions\n    for a client wallet (read only; no write endpoints).\n\
  \  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Conversions\n  description: Create quotes and quoted or instant currency conversions between user\n    or client wallets; view indicative conversion rates, quotes, and conversions.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Disputes.General\n  description: Manage the dispute lifecycle — submit, update, and close disputes,\n    create and submit dispute documents and pages; view and list disputes, dispute\n    documents, repudiations, and dispute transactions.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Disputes.Settlement\n  description: Create and view settlement transfers related to disputes.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Payins\n  description: Create and manage pay-ins across all payment methods — card registrations,\n    tokenization,\
  \ and validations, direct/web card pay-ins, recurring pay-ins, preauthorizations,\n    deposit preauthorizations, bank wires, banking aliases, mandates, direct debits,\n    and local/alternative methods (Apple Pay, Google Pay, PayPal, Klarna, iDEAL,\n    Bancontact, Bizum, BLIK, Giropay, etc.).\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Payouts\n  description: Create payouts and check instant payout eligibility; view payouts.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Refunds.General\n  description: View refund details.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Refunds.Payins\n  description: Create and list refunds for pay-in transactions.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Refunds.Payouts\n  description: List refunds for payout transactions.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n\
  - scope: Refunds.Repudiations\n  description: List refunds associated with repudiations (disputes).\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Refunds.Transfers\n  description: Create and list refunds for transfer operations.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Transfers\n  description: Create transfers between wallets and view transfer details.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Users.Details\n  description: Create, update, and categorize natural and legal users; view and list\n    users and their details.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n- scope: Users.Verification\n  description: Conduct identity verification — KYC documents and pages, UBO declarations,\n    and related verification endpoints.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n\
  - scope: Wallet.Details\n  description: Create and update user wallets; view and list wallets and list transactions\n    for a wallet and a user.\n  sources:\n  - https://docs.mangopay.com/api-reference/overview/api-keys/scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangopay/refs/heads/main/scopes/mangopay-scopes.yml
summary_line: 20 scopes · clientCredentials
tags:
- Payments
- Marketplace Payments
- Digital Wallets
- KYC
- KYB
- Fund Transfers
- Currency Conversion
- Payment Cards
- Fintech
- European
token_urls:
- https://api.mangopay.com/v2.01/{clientId}/oauth/token
---
