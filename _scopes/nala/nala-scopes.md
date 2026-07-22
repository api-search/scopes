---
api_specs:
- filename: nala-rafiki-openapi.yml
  format: yaml
  label: Rafiki API
  slug: rafiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/openapi/nala-rafiki-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.rafiki.com/reference/authentication#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nala Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NALA publishes 9 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the NALA API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NALA
provider_slug: nala
schemes: []
scope_count: 9
scope_names:
- bank:read
- lookup:read
- payment-account:read
- payment-account:write
- payout:read
- payout:write
- wallet:read
- statement:read
- statement:write
scopes:
- description: List banks (financial institutions that own payment accounts).
  flows: []
  scope: bank:read
- description: Look up metadata for a mobile money or bank account before payout.
  flows: []
  scope: lookup:read
- description: List payment accounts (recipients).
  flows: []
  scope: payment-account:read
- description: Create (or get-or-create) payment accounts. Also required to create payouts.
  flows: []
  scope: payment-account:write
- description: Read/list historical payouts and poll payout state.
  flows: []
  scope: payout:read
- description: Create payouts (send money). Requires payment-account:write as well.
  flows: []
  scope: payout:write
- description: List wallets and their currency balances.
  flows: []
  scope: wallet:read
- description: Read wallet statements and list statement lines.
  flows: []
  scope: statement:read
- description: Create (generate) wallet statements.
  flows: []
  scope: statement:write
slug: nala-scopes
source_filename: nala-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.rafiki.com/reference/authentication.md\ndocs: https://docs.rafiki.com/reference/authentication#scopes\napi: Rafiki API\nmodel: >-\n  Rafiki scopes are per-API-key permissions selected in the web portal at key\n  creation time (not OAuth2 flow scopes). Each endpoint documents the scope(s)\n  required to call it. Grant only the minimum scopes a key needs.\nscopes:\n  - scope: bank:read\n    description: List banks (financial institutions that own payment accounts).\n    operations: [List banks]\n  - scope: lookup:read\n    description: Look up metadata for a mobile money or bank account before payout.\n    operations: [Get lookups]\n  - scope: payment-account:read\n    description: List payment accounts (recipients).\n    operations: [List payment accounts]\n  - scope: payment-account:write\n    description: Create (or get-or-create) payment accounts. Also required to create payouts.\n    operations: [Create payment\
  \ accounts, Create payout]\n  - scope: payout:read\n    description: Read/list historical payouts and poll payout state.\n    operations: [Get payout, List payouts]\n  - scope: payout:write\n    description: Create payouts (send money). Requires payment-account:write as well.\n    operations: [Create payout]\n  - scope: wallet:read\n    description: List wallets and their currency balances.\n    operations: [List wallets]\n  - scope: statement:read\n    description: Read wallet statements and list statement lines.\n    operations: [Get statement, List statement lines]\n  - scope: statement:write\n    description: Create (generate) wallet statements.\n    operations: [Create statement]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nala/refs/heads/main/scopes/nala-scopes.yml
summary_line: 9 scopes
tags:
- Company
- Fintech
- Payments
- Remittances
- Money Transfer
- Payouts
- Cross-Border Payments
- Mobile Money
- Stablecoins
- Africa
token_urls: []
---
