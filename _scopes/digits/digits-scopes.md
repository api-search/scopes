---
api_specs:
- filename: digits-openapi-original.json
  format: json
  label: Digits Connect API
  slug: digits-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/openapi/digits-openapi-original.json
authorization_urls:
- https://connect.digits.com/v1/oauth/authorize
description: ''
docs: https://developer.digits.com/docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Digits Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Digits publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Digits API on a user''s behalf.


  Tokens are issued from https://connect.digits.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Digits
provider_slug: digits
schemes:
- flows:
  - authorizationUrl: https://connect.digits.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://connect.digits.com/v1/oauth/token
  name: OAuth2
scope_count: 6
scope_names:
- source:sync
- ledger:read
- documents:write
- organization:sync
- user:sync
- bills:manage
scopes:
- description: Create and update source data — sync sources, transactions, parties, departments, locations, projects, and products into a dedicated source.
  flows: []
  scope: source:sync
- description: Read the merged ledger — parties, categories/chart of accounts, transactions, summaries, and financial statements.
  flows: []
  scope: ledger:read
- description: Write documents (e.g. attach source documents / financial reports).
  flows: []
  scope: documents:write
- description: Manage organization-level resources — employees, entities, clients, and client entities.
  flows: []
  scope: organization:sync
- description: Sync user records associated with the connected account.
  flows: []
  scope: user:sync
- description: Manage the bill workflow — submit, approve, pay, reject, void, and update payment status on bills.
  flows: []
  scope: bills:manage
slug: digits-scopes
source_filename: digits-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.digits.com/docs/authentication\ndocs: https://developer.digits.com/docs/authentication\nschemes:\n- name: OAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.digits.com/v1/oauth/authorize\n    tokenUrl: https://connect.digits.com/v1/oauth/token\nscopes:\n- scope: source:sync\n  description: Create and update source data — sync sources, transactions, parties, departments, locations, projects, and products into a dedicated source.\n- scope: ledger:read\n  description: Read the merged ledger — parties, categories/chart of accounts, transactions, summaries, and financial statements.\n- scope: documents:write\n  description: Write documents (e.g. attach source documents / financial reports).\n- scope: organization:sync\n  description: Manage organization-level resources — employees, entities, clients, and client entities.\n- scope: user:sync\n  description: Sync user records associated\
  \ with the connected account.\n- scope: bills:manage\n  description: Manage the bill workflow — submit, approve, pay, reject, void, and update payment status on bills.\nnotes: >-\n  Scopes are requested as a space-separated `scope` query parameter on the authorization request\n  (e.g. \"source:sync ledger:read documents:write\"). Scope names were observed in the Digits Connect\n  API reference (per-operation \"Requires scope:\" notes) and the authentication guide.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits/refs/heads/main/scopes/digits-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Accounting
- Bookkeeping
- Financial Reporting
- General Ledger
- AI
- Fintech
- Accountants
- Bill Pay
- Invoicing
token_urls:
- https://connect.digits.com/v1/oauth/token
---
