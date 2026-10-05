---
authorization_urls: []
description: ''
docs: https://developers.addepar.com/docs/oauth
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Addepar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Addepar publishes 22 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Addepar API on a user''s behalf.


  Tokens are issued from https://api.addepar.com/public/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Addepar
provider_slug: addepar
schemes: []
scope_count: 22
scope_names:
- PROFILE
- PORTFOLIO
- TRANSACTIONS
- TRANSACTIONS_WRITE
- FILES
- FILES_WRITE
- GROUPS
- GROUPS_WRITE
- ENTITIES
- ENTITIES_WRITE
- POSITIONS
- POSITIONS_WRITE
- USERS
- USERS_WRITE
- TEAMS
- TEAMS_WRITE
- AUDIT_TRAIL
- REPORTS_WRITE
- BENCHMARKS_READ
- BENCHMARKS_WRITE
- BILLING_READ
- BILLING_WRITE
scopes:
- description: Access to the authorizing user's basic profile information.
  flows: []
  scope: PROFILE
- description: Read access to portfolio views, queries, and snapshots.
  flows: []
  scope: PORTFOLIO
- description: Read access to transactions.
  flows: []
  scope: TRANSACTIONS
- description: Create/update/delete transactions.
  flows: []
  scope: TRANSACTIONS_WRITE
- description: Read access to files.
  flows: []
  scope: FILES
- description: Upload and manage files.
  flows: []
  scope: FILES_WRITE
- description: Read access to groups.
  flows: []
  scope: GROUPS
- description: Create/update/delete groups.
  flows: []
  scope: GROUPS_WRITE
- description: Read access to entities (ownership graph).
  flows: []
  scope: ENTITIES
- description: Create/update/delete entities.
  flows: []
  scope: ENTITIES_WRITE
- description: Read access to positions.
  flows: []
  scope: POSITIONS
- description: Create/update/delete positions.
  flows: []
  scope: POSITIONS_WRITE
- description: Read access to users.
  flows: []
  scope: USERS
- description: Create/update/delete users.
  flows: []
  scope: USERS_WRITE
- description: Read access to teams.
  flows: []
  scope: TEAMS
- description: Create/update/delete teams.
  flows: []
  scope: TEAMS_WRITE
- description: Read access to the audit trail.
  flows: []
  scope: AUDIT_TRAIL
- description: Generate reports.
  flows: []
  scope: REPORTS_WRITE
- description: Read access to benchmarks.
  flows: []
  scope: BENCHMARKS_READ
- description: Create/update/delete benchmarks.
  flows: []
  scope: BENCHMARKS_WRITE
- description: Read access to billing (fees, fee schedules, billable portfolios).
  flows: []
  scope: BILLING_READ
- description: Manage billing configuration.
  flows: []
  scope: BILLING_WRITE
slug: addepar-scopes
source_filename: addepar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developers.addepar.com/docs/oauth\naid: addepar\nname: Addepar OAuth 2.0 Scopes\ndocs: https://developers.addepar.com/docs/oauth\nflow: authorizationCode\ntoken_url: https://api.addepar.com/public/oauth2/token\nsummary: >-\n  Granular OAuth 2.0 scopes granted per integration by Addepar. Read scopes and\n  paired *_WRITE scopes gate access to the corresponding resource domains.\nscopes:\n- name: PROFILE\n  description: Access to the authorizing user's basic profile information.\n- name: PORTFOLIO\n  description: Read access to portfolio views, queries, and snapshots.\n- name: TRANSACTIONS\n  description: Read access to transactions.\n- name: TRANSACTIONS_WRITE\n  description: Create/update/delete transactions.\n- name: FILES\n  description: Read access to files.\n- name: FILES_WRITE\n  description: Upload and manage files.\n- name: GROUPS\n  description: Read access to groups.\n- name: GROUPS_WRITE\n  description: Create/update/delete\
  \ groups.\n- name: ENTITIES\n  description: Read access to entities (ownership graph).\n- name: ENTITIES_WRITE\n  description: Create/update/delete entities.\n- name: POSITIONS\n  description: Read access to positions.\n- name: POSITIONS_WRITE\n  description: Create/update/delete positions.\n- name: USERS\n  description: Read access to users.\n- name: USERS_WRITE\n  description: Create/update/delete users.\n- name: TEAMS\n  description: Read access to teams.\n- name: TEAMS_WRITE\n  description: Create/update/delete teams.\n- name: AUDIT_TRAIL\n  description: Read access to the audit trail.\n- name: REPORTS_WRITE\n  description: Generate reports.\n- name: BENCHMARKS_READ\n  description: Read access to benchmarks.\n- name: BENCHMARKS_WRITE\n  description: Create/update/delete benchmarks.\n- name: BILLING_READ\n  description: Read access to billing (fees, fee schedules, billable portfolios).\n- name: BILLING_WRITE\n  description: Manage billing configuration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addepar/refs/heads/main/scopes/addepar-scopes.yml
summary_line: 22 scopes · authorizationCode
tags:
- Company
- Fintech
- Wealth Management
- Portfolio Management
- Investment Management
- Financial Data
- JSON:API
- REST
token_bound: false
token_urls:
- https://api.addepar.com/public/oauth2/token
---
