---
api_specs:
- filename: leanlaw-client-api-openapi.yml
  format: yaml
  label: LeanLaw Client API
  slug: leanlaw-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-client-api-openapi.yml
- filename: leanlaw-codes-api-openapi.yml
  format: yaml
  label: LeanLaw Codes API
  slug: leanlaw-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-codes-api-openapi.yml
- filename: leanlaw-customfield-api-openapi.yml
  format: yaml
  label: LeanLaw Custom Field API
  slug: leanlaw-customfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-customfield-api-openapi.yml
- filename: leanlaw-expense-api-openapi.yml
  format: yaml
  label: LeanLaw Expense API
  slug: leanlaw-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-expense-api-openapi.yml
- filename: leanlaw-fixedfee-api-openapi.yml
  format: yaml
  label: LeanLaw Fixed Fee API
  slug: leanlaw-fixedfee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-fixedfee-api-openapi.yml
- filename: leanlaw-invoice-api-openapi.yml
  format: yaml
  label: LeanLaw Invoice API
  slug: leanlaw-invoice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-invoice-api-openapi.yml
- filename: leanlaw-matter-api-openapi.yml
  format: yaml
  label: LeanLaw Matter API
  slug: leanlaw-matter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-matter-api-openapi.yml
- filename: leanlaw-practicearea-api-openapi.yml
  format: yaml
  label: LeanLaw Practice Area API
  slug: leanlaw-practicearea-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-practicearea-api-openapi.yml
- filename: leanlaw-timeentry-api-openapi.yml
  format: yaml
  label: LeanLaw Time Entry API
  slug: leanlaw-timeentry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-timeentry-api-openapi.yml
- filename: leanlaw-user-api-openapi.yml
  format: yaml
  label: LeanLaw User API
  slug: leanlaw-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/openapi/leanlaw-user-api-openapi.yml
authorization_urls: []
description: ''
docs: https://platform.leanlaw.io/agents
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Leanlaw Scopes
name_suffix: OAuth Scopes
note: Derived from the LIVE OAuth metadata, not from the OpenAPI. The published OpenAPI declares only a `BearerAuth` (http/bearer) scheme with no oauth2 flows, so derive-oauth-scopes.py found zero scopes in the spec; the real scope surface is published in the authorization-server and protected-resource discovery documents. This is a genuine gap between LeanLaw's contract and its deployed auth.
overview: 'LeanLaw uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LeanLaw
provider_slug: leanlaw
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: leanlaw-scopes
source_filename: leanlaw-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://api.leanlaw.io/.well-known/oauth-protected-resource\ndocs: https://platform.leanlaw.io/agents\nnote: >-\n  Derived from the LIVE OAuth metadata, not from the OpenAPI. The published OpenAPI declares only a\n  `BearerAuth` (http/bearer) scheme with no oauth2 flows, so derive-oauth-scopes.py found zero scopes\n  in the spec; the real scope surface is published in the authorization-server and protected-resource\n  discovery documents. This is a genuine gap between LeanLaw's contract and its deployed auth.\nauthorization_server: https://auth.myleanlaw.co/\nissuer: https://auth.myleanlaw.co/\nprotected_resource: https://api.leanlaw.io/mcp\nauthorization_endpoint: https://api.myleanlaw.co/oauth/authorize\ntoken_endpoint: https://api.myleanlaw.co/oauth/token\nrevocation_endpoint: https://api.myleanlaw.co/oauth/revoke\njwks_uri: https://api.myleanlaw.co/.well-known/jwks.json\nflows:\n- authorization_code\n- refresh_token\npkce:\n\
  \  supported: true\n  code_challenge_methods: [S256, plain]\ntoken_endpoint_auth_methods:\n- none\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\nscope_count: 16\nscopes:\n- name: openid\n  description: OpenID Connect authentication; issues an ID token (RS256).\n  source: openid-configuration\n- name: offline_access\n  description: Issue a refresh token so the agent can act after the initial session expires.\n  source: both\n- name: 'read:*'\n  description: Read access to every supported resource. Wildcard grant.\n  source: both\n- name: 'write:*'\n  description: Write access to every supported resource. Wildcard grant.\n  source: both\n- name: 'read:clients'\n  description: Read law-firm clients, including contact details when requested via select=contact.\n  source: both\n- name: 'write:clients'\n  description: Create, update and delete clients.\n  source: both\n- name: 'read:matters'\n  description: Read matters, their responsible/originator users, practice area and\
  \ LEDES configuration.\n  source: both\n- name: 'write:matters'\n  description: Create, update and delete matters. Creating a matter can also create the matching\n    QuickBooks Online customer/sub-customer for firms on the QBO integration.\n  source: both\n- name: 'read:time-entries'\n  description: Read billable time entries.\n  source: both\n- name: 'write:time-entries'\n  description: Create, update and delete time entries.\n  source: both\n- name: 'read:expenses'\n  description: Read matter expenses.\n  source: both\n- name: 'write:expenses'\n  description: Create, update and delete expenses.\n  source: both\n- name: 'read:fixed-fees'\n  description: Read fixed-fee (flat-fee) billable items.\n  source: both\n- name: 'write:fixed-fees'\n  description: Create, update and delete fixed fees.\n  source: both\n- name: 'read:invoices'\n  description: Read invoices. There is no write scope for invoices — the invoice surface is read-only.\n  source: both\n- name: 'read:balances'\n  description:\
  \ Read client account balances.\n  source: both\n- name: 'read:codes'\n  description: Read LEDES activity, task and expense code sets.\n  source: both\nobservations:\n- No write scope exists for invoices, balances or codes — those surfaces are read-only by design and\n  the scope list reflects it.\n- Trust accounts and settlements are explicitly excluded from the agent surface per\n  https://platform.leanlaw.io/agents, and no scope is published for them.\n- The `read:*` / `write:*` wildcards let a client request blanket access; a least-privilege\n  integration should request the specific resource scopes instead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leanlaw/refs/heads/main/scopes/leanlaw-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Legal
- Legal Billing
- Law Firms
- Time Tracking
- Billing
- Invoicing
- Accounting
- Trust Accounting
- Practice Management
- QuickBooks
- Payments
- LegalTech
- SaaS
token_urls: []
---
