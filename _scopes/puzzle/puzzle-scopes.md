---
api_specs:
- filename: puzzle-openapi-original.json
  format: json
  label: Puzzle Accounting API
  slug: puzzle-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/openapi/puzzle-openapi-original.json
authorization_urls: []
description: ''
docs: https://puzzle-api.readme.io/docs/scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Puzzle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Puzzle publishes 21 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Puzzle API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Puzzle
provider_slug: puzzle
schemes:
- authorizationUrl: https://api.puzzle.io/oauth/authorize
  flow: authorizationCode
  name: OAuth2
  pkce: true
  tokenUrl: https://api.puzzle.io/oauth/token
scope_count: 21
scope_names:
- read:company
- write:company
- write:account
- write:transaction
- write:account_balance
- write:benefit
- write:department
- write:location
- write:worker
- write:payroll
- write:journal
- write:bill
- write:customer
- write:integration_connection
- write:invoice
- write:product
- write:request
- write:task
- write:vendor
- write:classification
- offline_access
scopes:
- description: Grants read-only access to company data.
  flows: []
  scope: read:company
- description: Allows creating or updating company info.
  flows: []
  scope: write:company
- description: Allows creating financial accounts.
  flows: []
  scope: write:account
- description: Allows creating transactions.
  flows: []
  scope: write:transaction
- description: Allows creating financial account balances.
  flows: []
  scope: write:account_balance
- description: Allows creating company benefit policies.
  flows: []
  scope: write:benefit
- description: Allows creating departments.
  flows: []
  scope: write:department
- description: Allows creating office locations.
  flows: []
  scope: write:location
- description: Allows creating employees and contractors.
  flows: []
  scope: write:worker
- description: Allows creating payrolls.
  flows: []
  scope: write:payroll
- description: Allows creating and updating journal entries.
  flows: []
  scope: write:journal
- description: Allows creating bills.
  flows: []
  scope: write:bill
- description: Allows creating customers.
  flows: []
  scope: write:customer
- description: Allows creating integration connections.
  flows: []
  scope: write:integration_connection
- description: Allows creating invoices.
  flows: []
  scope: write:invoice
- description: Allows creating products.
  flows: []
  scope: write:product
- description: Allows creating requests.
  flows: []
  scope: write:request
- description: Allows creating tasks.
  flows: []
  scope: write:task
- description: Allows creating vendors.
  flows: []
  scope: write:vendor
- description: Allows creating classifications.
  flows: []
  scope: write:classification
- description: Allows obtaining a refresh token for long-lived access.
  flows: []
  scope: offline_access
slug: puzzle-scopes
source_filename: puzzle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://puzzle-api.readme.io/docs/scopes\ndocs: https://puzzle-api.readme.io/docs/scopes\nschemes:\n- name: OAuth2\n  flow: authorizationCode\n  pkce: true\n  authorizationUrl: https://api.puzzle.io/oauth/authorize\n  tokenUrl: https://api.puzzle.io/oauth/token\ndefault_scopes: [offline_access, read:company]\nnotes: >-\n  Scopes are requested at /oauth/authorize. If no scopes are provided, the read-only\n  scopes (offline_access, read:company) are used by default. Scopes are documented in\n  the developer docs; the OpenAPI document itself does not declare oauth2 securitySchemes,\n  so these were captured from the scopes reference page.\nscopes:\n- {scope: 'read:company', description: Grants read-only access to company data.}\n- {scope: 'write:company', description: Allows creating or updating company info.}\n- {scope: 'write:account', description: Allows creating financial accounts.}\n- {scope: 'write:transaction', description:\
  \ Allows creating transactions.}\n- {scope: 'write:account_balance', description: Allows creating financial account balances.}\n- {scope: 'write:benefit', description: Allows creating company benefit policies.}\n- {scope: 'write:department', description: Allows creating departments.}\n- {scope: 'write:location', description: Allows creating office locations.}\n- {scope: 'write:worker', description: Allows creating employees and contractors.}\n- {scope: 'write:payroll', description: Allows creating payrolls.}\n- {scope: 'write:journal', description: Allows creating and updating journal entries.}\n- {scope: 'write:bill', description: Allows creating bills.}\n- {scope: 'write:customer', description: Allows creating customers.}\n- {scope: 'write:integration_connection', description: Allows creating integration connections.}\n- {scope: 'write:invoice', description: Allows creating invoices.}\n- {scope: 'write:product', description: Allows creating products.}\n- {scope: 'write:request', description:\
  \ Allows creating requests.}\n- {scope: 'write:task', description: Allows creating tasks.}\n- {scope: 'write:vendor', description: Allows creating vendors.}\n- {scope: 'write:classification', description: Allows creating classifications.}\n- {scope: 'offline_access', description: Allows obtaining a refresh token for long-lived access.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle/refs/heads/main/scopes/puzzle-scopes.yml
summary_line: 21 scopes
tags:
- Company
- Accounting
- Financial
- Bookkeeping
- Fintech
- General Ledger
- Payroll
- Agent-Native
- MCP
token_urls: []
---
