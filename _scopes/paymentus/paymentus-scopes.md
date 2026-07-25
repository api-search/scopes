---
authorization_urls: []
description: ''
docs: https://developer.paymentus.io/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Paymentus Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Paymentus publishes 16 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Paymentus API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paymentus
provider_slug: paymentus
schemes:
- name: BearerAuth
  source: packages/paymentus-packages.yml
  type: jwt-scopes
scope_count: 16
scope_names:
- xotp
- xotp:profile
- xotp:profile:read
- xotp:profile:create
- xotp:profile:update
- xotp:profile:delete
- xotp:listProfiles
- xotp:payment
- xotp:payment:history
- xotp:payment:void
- xotp:autopay
- xotp:autopay:delete
- xotp:account
- xotp:accounts
- xotp:listAccounts
- paybotus
scopes:
- description: Basic XOTP functionality (base payment surface).
  flows: []
  scope: xotp
- description: Profile (wallet/payment-method token) management.
  flows: []
  scope: xotp:profile
- description: Read profile data.
  flows: []
  scope: xotp:profile:read
- description: Create profiles.
  flows: []
  scope: xotp:profile:create
- description: Update profiles.
  flows: []
  scope: xotp:profile:update
- description: Delete profiles.
  flows: []
  scope: xotp:profile:delete
- description: List profiles.
  flows: []
  scope: xotp:listProfiles
- description: Payment processing (Sale / make payment).
  flows: []
  scope: xotp:payment
- description: Read payment history.
  flows: []
  scope: xotp:payment:history
- description: Void or cancel payments.
  flows: []
  scope: xotp:payment:void
- description: AutoPay enrollment and management.
  flows: []
  scope: xotp:autopay
- description: Delete AutoPay settings.
  flows: []
  scope: xotp:autopay:delete
- description: Link an account to a user.
  flows: []
  scope: xotp:account
- description: Account management.
  flows: []
  scope: xotp:accounts
- description: List accounts.
  flows: []
  scope: xotp:listAccounts
- description: Paybotus functionality.
  flows: []
  scope: paybotus
slug: paymentus-scopes
source_filename: paymentus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: https://www.npmjs.com/package/@paymentus/auth\ndocs: https://developer.paymentus.io/\nmodel: >-\n  Granular OAuth-style scopes declared at JWT issuance via the Auth API. A client\n  requests scopes directly or supplies a Paymentus \"pixel\" that expands to a\n  required scope set (see pixels[] below).\nschemes:\n  - name: BearerAuth\n    type: jwt-scopes\n    source: packages/paymentus-packages.yml\nscopes:\n  - scope: xotp\n    description: Basic XOTP functionality (base payment surface).\n  - scope: \"xotp:profile\"\n    description: Profile (wallet/payment-method token) management.\n  - scope: \"xotp:profile:read\"\n    description: Read profile data.\n  - scope: \"xotp:profile:create\"\n    description: Create profiles.\n  - scope: \"xotp:profile:update\"\n    description: Update profiles.\n  - scope: \"xotp:profile:delete\"\n    description: Delete profiles.\n  - scope: \"xotp:listProfiles\"\n    description: List profiles.\n\
  \  - scope: \"xotp:payment\"\n    description: Payment processing (Sale / make payment).\n  - scope: \"xotp:payment:history\"\n    description: Read payment history.\n  - scope: \"xotp:payment:void\"\n    description: Void or cancel payments.\n  - scope: \"xotp:autopay\"\n    description: AutoPay enrollment and management.\n  - scope: \"xotp:autopay:delete\"\n    description: Delete AutoPay settings.\n  - scope: \"xotp:account\"\n    description: Link an account to a user.\n  - scope: \"xotp:accounts\"\n    description: Account management.\n  - scope: \"xotp:listAccounts\"\n    description: List accounts.\n  - scope: paybotus\n    description: Paybotus functionality.\npixels:\n  - name: tokenization-pixel\n    scopes: [\"xotp:profile\"]\n    required_claims: []\n  - name: list-wallets-pixel\n    scopes: [\"xotp:profile\", \"xotp:listProfiles\", \"xotp:profile:delete\"]\n    required_claims: [userLogin]\n  - name: user-checkout-pixel\n    scopes: [\"xotp:profile\", \"xotp:payment\", \"\
  xotp:listProfiles\", \"xotp:listAccounts\", \"xotp:profile:delete\"]\n    optional_scopes: [\"xotp:autopay\", \"xotp:account\"]\n    required_claims: [userLogin, paymentsData]\n  - name: guest-checkout-pixel\n    scopes: [\"xotp:payment\", \"xotp:listAccounts\", \"xotp:profile\"]\n    required_claims: [paymentsData]\n    note: Automatically sets pmToken ['anonymousPMOnly'] in the JWT.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paymentus/refs/heads/main/scopes/paymentus-scopes.yml
summary_line: 16 scopes
tags:
- Payments
- United States
- Bill Payment
- Electronic Bill Presentment
- Payment Processing
- Payment Gateway
- Disbursements
- ACH
- Real-Time Payments
- Tokenization
token_urls: []
---
