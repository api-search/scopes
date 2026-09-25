---
authorization_urls: []
description: ''
docs: https://docs.api.aspireapp.com/glossary
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Aspire Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aspire publishes 2 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aspire API on a user''s behalf.


  Tokens are issued from https://api.aspireapp.com/public/v1/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aspire
provider_slug: aspire
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.aspireapp.com/public/v1/login
  - flow: authorizationCode
    pkce: true
  name: OAuth2
  source: https://docs.api.aspireapp.com/authentication
scope_count: 2
scope_names:
- transfers
- quotes
scopes:
- description: Create and manage payout/transfer operations. Required (together with quotes) for FX transfers.
  flows: []
  scope: transfers
- description: Create foreign-exchange quotes (lock an exchange rate) prior to an FX transfer. Required together with transfers for FX transfers.
  flows: []
  scope: quotes
slug: aspire-scopes
source_filename: aspire-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.api.aspireapp.com/authentication\ndocs: https://docs.api.aspireapp.com/glossary\napi: Aspire API\nnotes: >-\n  Aspire API keys and OAuth tokens are granted scopes that limit which endpoints\n  a token may call. The docs enumerate transfers and quotes explicitly and note\n  that FX transfers require BOTH transfers and quotes. Additional product scopes\n  (cards, transactions/bank-feeds) are implied by the product surface but are\n  not exhaustively published; only documented scopes are recorded here.\nschemes:\n- name: OAuth2\n  source: https://docs.api.aspireapp.com/authentication\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.aspireapp.com/public/v1/login\n  - flow: authorizationCode\n    pkce: true\nscopes:\n- scope: transfers\n  description: >-\n    Create and manage payout/transfer operations. Required (together with\n    quotes) for FX transfers.\n  sources: [https://docs.api.aspireapp.com/authentication]\n\
  - scope: quotes\n  description: >-\n    Create foreign-exchange quotes (lock an exchange rate) prior to an FX\n    transfer. Required together with transfers for FX transfers.\n  sources: [https://docs.api.aspireapp.com/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspire/refs/heads/main/scopes/aspire-scopes.yml
summary_line: 2 scopes · clientCredentials/authorizationCode
tags:
- Company
- Fintech
- Business Banking
- Payments
- Payouts
- Card Issuance
- Foreign Exchange
- Expense Management
- Financial Services
- Singapore
token_urls:
- https://api.aspireapp.com/public/v1/login
---
