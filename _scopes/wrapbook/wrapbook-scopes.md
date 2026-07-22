---
authorization_urls:
- https://app.wrapbook.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Wrapbook Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wrapbook publishes 21 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wrapbook API on a user''s behalf.


  Tokens are issued from https://app.wrapbook.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wrapbook
provider_slug: wrapbook
schemes:
- flows:
  - authorizationUrl: https://app.wrapbook.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://app.wrapbook.com/oauth/register
    revocationUrl: https://app.wrapbook.com/oauth/revoke
    tokenUrl: https://app.wrapbook.com/oauth/token
  name: OAuth2
  source: well-known/wrapbook-oauth-authorization-server.json
scope_count: 21
scope_names:
- accounting_ap_invoices:read
- accounting_bank_accounts:read
- accounting_bank_reconciliation:read
- accounting_chart_of_accounts:read
- accounting_chart_reference_mapping:read
- accounting_currencies:read
- accounting_distribution_changes:read
- accounting_electronic_signatures:read
- accounting_journal_entries:read
- accounting_payroll_transactions:read
- accounting_period_management:read
- accounting_reports:read
- accounting_tag_management:read
- accounting_vendor_payments:read
- accounting_vendors:read
- budget_cost_tracking:read
- budget_production_accounting:read
- payroll_invoices:read
- payroll_reports:read
- purchase_orders:read
- core:read
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: accounting_ap_invoices:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_bank_accounts:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_bank_reconciliation:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_chart_of_accounts:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_chart_reference_mapping:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_currencies:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_distribution_changes:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_electronic_signatures:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_journal_entries:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_payroll_transactions:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_period_management:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_reports:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_tag_management:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_vendor_payments:read
- description: ''
  flows:
  - authorizationCode
  scope: accounting_vendors:read
- description: ''
  flows:
  - authorizationCode
  scope: budget_cost_tracking:read
- description: ''
  flows:
  - authorizationCode
  scope: budget_production_accounting:read
- description: ''
  flows:
  - authorizationCode
  scope: payroll_invoices:read
- description: ''
  flows:
  - authorizationCode
  scope: payroll_reports:read
- description: ''
  flows:
  - authorizationCode
  scope: purchase_orders:read
- description: ''
  flows:
  - authorizationCode
  scope: core:read
slug: wrapbook-scopes
source_filename: wrapbook-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://app.wrapbook.com/.well-known/oauth-authorization-server\nnotes: >-\n  Wrapbook publishes no public API reference, but its production app exposes RFC 8414\n  OAuth 2.0 authorization-server metadata declaring 21 read-only scopes covering the\n  accounting, payroll, budgeting, and purchase-order surface the platform shares with\n  its accounting integrations (Sage Intacct, QuickBooks Online, Oracle NetSuite,\n  Acumatica). Scope descriptions below are inferred only from the scope identifiers\n  themselves; Wrapbook publishes no scope reference page.\nschemes:\n- name: OAuth2\n  source: well-known/wrapbook-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.wrapbook.com/oauth/authorize\n    tokenUrl: https://app.wrapbook.com/oauth/token\n    revocationUrl: https://app.wrapbook.com/oauth/revoke\n    registrationUrl: https://app.wrapbook.com/oauth/register\n    pkce: [S256]\n\
  scopes:\n- scope: accounting_ap_invoices:read\n  flows: [authorizationCode]\n- scope: accounting_bank_accounts:read\n  flows: [authorizationCode]\n- scope: accounting_bank_reconciliation:read\n  flows: [authorizationCode]\n- scope: accounting_chart_of_accounts:read\n  flows: [authorizationCode]\n- scope: accounting_chart_reference_mapping:read\n  flows: [authorizationCode]\n- scope: accounting_currencies:read\n  flows: [authorizationCode]\n- scope: accounting_distribution_changes:read\n  flows: [authorizationCode]\n- scope: accounting_electronic_signatures:read\n  flows: [authorizationCode]\n- scope: accounting_journal_entries:read\n  flows: [authorizationCode]\n- scope: accounting_payroll_transactions:read\n  flows: [authorizationCode]\n- scope: accounting_period_management:read\n  flows: [authorizationCode]\n- scope: accounting_reports:read\n  flows: [authorizationCode]\n- scope: accounting_tag_management:read\n  flows: [authorizationCode]\n- scope: accounting_vendor_payments:read\n\
  \  flows: [authorizationCode]\n- scope: accounting_vendors:read\n  flows: [authorizationCode]\n- scope: budget_cost_tracking:read\n  flows: [authorizationCode]\n- scope: budget_production_accounting:read\n  flows: [authorizationCode]\n- scope: payroll_invoices:read\n  flows: [authorizationCode]\n- scope: payroll_reports:read\n  flows: [authorizationCode]\n- scope: purchase_orders:read\n  flows: [authorizationCode]\n- scope: core:read\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wrapbook/refs/heads/main/scopes/wrapbook-scopes.yml
summary_line: 21 scopes · authorizationCode
tags:
- Company
- Entertainment
- Payroll
- Production Accounting
- Accounts Payable
- Film
- Television
- Fintech
token_urls:
- https://app.wrapbook.com/oauth/token
---
