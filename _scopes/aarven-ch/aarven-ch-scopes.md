---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Aarven Ch Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aarven publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aarven API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aarven
provider_slug: aarven-ch
schemes: []
scope_count: 4
scope_names:
- BookingsWrite
- BookingsRead
- AccountsRead
- CompanyRead
scopes:
- description: Required for POST /bookings
  flows: []
  scope: BookingsWrite
- description: Required for GET /bookings and GET /bookings/{id}
  flows: []
  scope: BookingsRead
- description: Required for GET /accounts and GET /tax-codes
  flows: []
  scope: AccountsRead
- description: Required for GET /company
  flows: []
  scope: CompanyRead
slug: aarven-ch-scopes
source_filename: aarven-ch-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://aarven.ch/Api\nscopes:\n  - name: BookingsWrite\n    description: Required for POST /bookings\n  - name: BookingsRead\n    description: Required for GET /bookings and GET /bookings/{id}\n  - name: AccountsRead\n    description: Required for GET /accounts and GET /tax-codes\n  - name: CompanyRead\n    description: Required for GET /company\n"
source_yaml_url: https://artifacts.apis.io/aarven-ch/scopes/aarven-ch-scopes.yml
summary_line: 4 scopes
tags:
- Accounting
- Artificial Intelligence
- Bookkeeping
- Swiss
- Finance
- Automation
token_bound: false
token_urls: []
---
