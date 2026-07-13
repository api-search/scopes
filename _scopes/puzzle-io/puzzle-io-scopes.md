---
api_specs:
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Companies API
  slug: puzzle-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Transactions API
  slug: puzzle-io-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Ledger Accounts API
  slug: puzzle-io-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Journal Entries API
  slug: puzzle-io-journal-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Financial Reports API
  slug: puzzle-io-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Metrics API
  slug: puzzle-io-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Categories API
  slug: puzzle-io-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
- filename: puzzle-io-openapi.yml
  format: yaml
  label: Puzzle Integrations API
  slug: puzzle-io-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/openapi/puzzle-io-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Puzzle Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Puzzle publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Puzzle API on a user''s behalf.


  Tokens are issued from https://puzzle-api.readme.io/reference.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Puzzle
provider_slug: puzzle-io
schemes:
- description: OAuth 2.0 with scoped access (for example read:company, read:transactions, read:report). Partner credentials are issued after the Puzzle partner technical review.
  flows:
  - flow: clientCredentials
    tokenUrl: https://puzzle-api.readme.io/reference
  name: oauth2
  source: openapi/puzzle-io-openapi.yml
scope_count: 4
scope_names:
- read:accounts
- read:company
- read:report
- read:transactions
scopes:
- description: Read ledger accounts
  flows:
  - clientCredentials
  scope: read:accounts
- description: Read company data
  flows:
  - clientCredentials
  scope: read:company
- description: Read financial statements
  flows:
  - clientCredentials
  scope: read:report
- description: Read transactions
  flows:
  - clientCredentials
  scope: read:transactions
slug: puzzle-io-scopes
source_filename: puzzle-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/puzzle-io-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/puzzle-io-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://puzzle-api.readme.io/reference\n  description: OAuth 2.0 with scoped access (for example read:company, read:transactions, read:report).\n    Partner credentials are issued after the Puzzle partner technical review.\nscopes:\n- scope: read:accounts\n  description: Read ledger accounts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/puzzle-io-openapi.yml\n- scope: read:company\n  description: Read company data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/puzzle-io-openapi.yml\n- scope: read:report\n  description: Read financial statements\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/puzzle-io-openapi.yml\n- scope: read:transactions\n  description: Read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/puzzle-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puzzle-io/refs/heads/main/scopes/puzzle-io-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Accounting
- Fintech
- General Ledger
- Financial Reporting
- Bookkeeping
- Startups
- Embedded Accounting
- Metrics
token_urls:
- https://puzzle-api.readme.io/reference
---
