---
api_specs:
- filename: ramp-accounts-api-openapi.yml
  format: yaml
  label: Ramp Accounts API
  slug: ramp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-accounts-api-openapi.yml
- filename: ramp-audit-logs-api-openapi.yml
  format: yaml
  label: Ramp Audit Logs API
  slug: ramp-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-audit-logs-api-openapi.yml
- filename: ramp-bills-api-openapi.yml
  format: yaml
  label: Ramp Bills API
  slug: ramp-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-bills-api-openapi.yml
- filename: ramp-cards-api-openapi.yml
  format: yaml
  label: Ramp Cards API
  slug: ramp-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-cards-api-openapi.yml
- filename: ramp-departments-api-openapi.yml
  format: yaml
  label: Ramp Departments API
  slug: ramp-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-departments-api-openapi.yml
- filename: ramp-locations-api-openapi.yml
  format: yaml
  label: Ramp Locations API
  slug: ramp-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-locations-api-openapi.yml
- filename: ramp-reimbursements-api-openapi.yml
  format: yaml
  label: Ramp Reimbursements API
  slug: ramp-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-reimbursements-api-openapi.yml
- filename: ramp-statements-api-openapi.yml
  format: yaml
  label: Ramp Statements API
  slug: ramp-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-statements-api-openapi.yml
- filename: ramp-transactions-api-openapi.yml
  format: yaml
  label: Ramp Transactions API
  slug: ramp-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-transactions-api-openapi.yml
- filename: ramp-users-api-openapi.yml
  format: yaml
  label: Ramp Users API
  slug: ramp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-users-api-openapi.yml
- filename: ramp-vendors-api-openapi.yml
  format: yaml
  label: Ramp Vendors API
  slug: ramp-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-vendors-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Ramp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ramp publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ramp API on a user''s behalf.


  Tokens are issued from https://api.ramp.com/developer/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ramp
provider_slug: ramp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.ramp.com/developer/v1/token
  name: OAuth2
  source: openapi/ramp-developer-api-openapi.yml
scope_count: 12
scope_names:
- accounting:read
- accounting:write
- applications:read
- audit:read
- bills:read
- cards:read
- departments:read
- locations:read
- reimbursements:read
- statements:read
- transactions:read
- users:read
scopes:
- description: Read accounting resources
  flows:
  - clientCredentials
  scope: accounting:read
- description: Write accounting resources
  flows:
  - clientCredentials
  scope: accounting:write
- description: Read applications
  flows:
  - clientCredentials
  scope: applications:read
- description: Read audit logs
  flows:
  - clientCredentials
  scope: audit:read
- description: Read bills
  flows:
  - clientCredentials
  scope: bills:read
- description: Read cards
  flows:
  - clientCredentials
  scope: cards:read
- description: Read departments
  flows:
  - clientCredentials
  scope: departments:read
- description: Read locations
  flows:
  - clientCredentials
  scope: locations:read
- description: Read reimbursements
  flows:
  - clientCredentials
  scope: reimbursements:read
- description: Read statements
  flows:
  - clientCredentials
  scope: statements:read
- description: Read transactions
  flows:
  - clientCredentials
  scope: transactions:read
- description: Read users
  flows:
  - clientCredentials
  scope: users:read
slug: ramp-scopes
source_filename: ramp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ramp-developer-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/ramp-developer-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ramp.com/developer/v1/token\nscopes:\n- scope: accounting:read\n  description: Read accounting resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: accounting:write\n  description: Write accounting resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: applications:read\n  description: Read applications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: audit:read\n  description: Read audit logs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: bills:read\n  description: Read bills\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n\
  - scope: cards:read\n  description: Read cards\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: departments:read\n  description: Read departments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: locations:read\n  description: Read locations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: reimbursements:read\n  description: Read reimbursements\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: statements:read\n  description: Read statements\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: transactions:read\n  description: Read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n- scope: users:read\n  description: Read users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/ramp-developer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/scopes/ramp-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursement
token_urls:
- https://api.ramp.com/developer/v1/token
---
