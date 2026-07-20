---
api_specs:
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Contacts API
  slug: bexio-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Sales Order Management API
  slug: bexio-sales-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Accounting API
  slug: bexio-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Items API
  slug: bexio-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Projects & Time Tracking API
  slug: bexio-projects-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Files API
  slug: bexio-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Purchase API
  slug: bexio-purchase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Payroll API
  slug: bexio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
- filename: bexio-openapi.yml
  format: yaml
  label: bexio Banking API
  slug: bexio-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/openapi/bexio-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.bexio.com/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Bexio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'bexio publishes 71 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the bexio API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: bexio
provider_slug: bexio
schemes:
- authorizationUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/auth
  flow: authorizationCode
  issuer: https://auth.bexio.com/realms/bexio
  name: oauth2_authorization_code
  source: https://auth.bexio.com/realms/bexio/.well-known/openid-configuration
  tokenUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/token
  type: oauth2
scope_count: 71
scope_names:
- openid
- profile
- email
- offline_access
- company_profile
- additional_company
- company_memberships_show
- contact_show
- contact_edit
- note_show
- note_edit
- lead_show
- lead_edit
- kb_offer_show
- kb_offer_edit
- kb_order_show
- kb_order_edit
- kb_invoice_show
- kb_invoice_edit
- kb_delivery_show
- kb_delivery_edit
- kb_credit_voucher_show
- kb_credit_voucher_edit
- kb_bill_show
- kb_bill_edit
- kb_expense_show
- kb_expense_edit
- kb_article_order_show
- kb_article_order_edit
- article_show
- article_edit
- stock_edit
- accounting
- accounting_settings_show
- accounting_settings_edit
- transaction_show
- transaction_edit
- subledger_show
- subledger_edit
- finance_reports
- project_show
- project_edit
- task_show
- task_edit
- monitoring_show
- monitoring_edit
- payroll_employee_show
- payroll_employee_edit
- payroll_absence_show
- payroll_absence_edit
- payroll_paystub_show
- payroll_time_account_show
- payroll_time_account_edit
- payroll_statistic_show
- bank_account_show
- bank_account_edit
- bank_payment_show
- bank_payment_edit
- bill_banking_payment_edit
- file
- archive_show
- archive_edit
- archive_settings_show
- archive_settings_edit
- connected_clients_show
- connected_clients_edit
- pat_show
- pat_edit
- roles
- chat_edit
- subscription_and_permissions
scopes:
- description: OIDC authentication (subject identifier).
  flows: []
  scope: openid
- description: OIDC standard profile claims.
  flows: []
  scope: profile
- description: OIDC email claim.
  flows: []
  scope: email
- description: Issue refresh tokens for long-lived server-to-server access.
  flows: []
  scope: offline_access
- description: Read the company profile.
  flows: []
  scope: company_profile
- description: Access additional companies on the account.
  flows: []
  scope: additional_company
- description: Read company memberships.
  flows: []
  scope: company_memberships_show
- description: Read contacts
  flows: []
  scope: contact_show
- description: Create and modify contacts.
  flows: []
  scope: contact_edit
- description: Read notes.
  flows: []
  scope: note_show
- description: Create and modify notes.
  flows: []
  scope: note_edit
- description: Read leads.
  flows: []
  scope: lead_show
- description: Create and modify leads.
  flows: []
  scope: lead_edit
- description: Read quotes/offers (Offerte).
  flows: []
  scope: kb_offer_show
- description: Create and modify quotes/offers.
  flows: []
  scope: kb_offer_edit
- description: Read orders (Auftrag).
  flows: []
  scope: kb_order_show
- description: Create and modify orders.
  flows: []
  scope: kb_order_edit
- description: Read invoices (Rechnung).
  flows: []
  scope: kb_invoice_show
- description: Create and modify invoices
  flows: []
  scope: kb_invoice_edit
- description: Read delivery notes (Lieferschein).
  flows: []
  scope: kb_delivery_show
- description: Create and modify delivery notes.
  flows: []
  scope: kb_delivery_edit
- description: Read credit notes (Gutschrift).
  flows: []
  scope: kb_credit_voucher_show
- description: Create and modify credit notes.
  flows: []
  scope: kb_credit_voucher_edit
- description: Read supplier bills (Lieferantenrechnungen).
  flows: []
  scope: kb_bill_show
- description: Create and modify supplier bills.
  flows: []
  scope: kb_bill_edit
- description: Read expenses (Spesen).
  flows: []
  scope: kb_expense_show
- description: Create and modify expenses.
  flows: []
  scope: kb_expense_edit
- description: Read article/order line items.
  flows: []
  scope: kb_article_order_show
- description: Create and modify article/order line items.
  flows: []
  scope: kb_article_order_edit
- description: Read items/products (Artikel).
  flows: []
  scope: article_show
- description: Create and modify items/products.
  flows: []
  scope: article_edit
- description: Modify stock levels.
  flows: []
  scope: stock_edit
- description: Chart of accounts
  flows: []
  scope: accounting
- description: Read accounting settings.
  flows: []
  scope: accounting_settings_show
- description: Modify accounting settings.
  flows: []
  scope: accounting_settings_edit
- description: Read accounting transactions.
  flows: []
  scope: transaction_show
- description: Create and modify accounting transactions.
  flows: []
  scope: transaction_edit
- description: Read subledger data.
  flows: []
  scope: subledger_show
- description: Modify subledger data.
  flows: []
  scope: subledger_edit
- description: Access finance reports.
  flows: []
  scope: finance_reports
- description: Read projects.
  flows: []
  scope: project_show
- description: Create and modify projects.
  flows: []
  scope: project_edit
- description: Read tasks.
  flows: []
  scope: task_show
- description: Create and modify tasks.
  flows: []
  scope: task_edit
- description: Read time-tracking / monitoring data.
  flows: []
  scope: monitoring_show
- description: Create and modify time-tracking entries.
  flows: []
  scope: monitoring_edit
- description: Read payroll employees.
  flows: []
  scope: payroll_employee_show
- description: Create and modify payroll employees.
  flows: []
  scope: payroll_employee_edit
- description: Read payroll absences.
  flows: []
  scope: payroll_absence_show
- description: Create and modify payroll absences.
  flows: []
  scope: payroll_absence_edit
- description: Read paystubs.
  flows: []
  scope: payroll_paystub_show
- description: Read payroll time accounts.
  flows: []
  scope: payroll_time_account_show
- description: Modify payroll time accounts.
  flows: []
  scope: payroll_time_account_edit
- description: Read payroll statistics.
  flows: []
  scope: payroll_statistic_show
- description: Read bank accounts.
  flows: []
  scope: bank_account_show
- description: Create and modify bank accounts.
  flows: []
  scope: bank_account_edit
- description: Read bank payments.
  flows: []
  scope: bank_payment_show
- description: Create and modify bank payments.
  flows: []
  scope: bank_payment_edit
- description: Create bill banking payments (pay supplier bills).
  flows: []
  scope: bill_banking_payment_edit
- description: Upload
  flows: []
  scope: file
- description: Read archived documents.
  flows: []
  scope: archive_show
- description: Modify archived documents.
  flows: []
  scope: archive_edit
- description: Read archive settings.
  flows: []
  scope: archive_settings_show
- description: Modify archive settings.
  flows: []
  scope: archive_settings_edit
- description: Read connected clients (accountant sharing).
  flows: []
  scope: connected_clients_show
- description: Modify connected clients.
  flows: []
  scope: connected_clients_edit
- description: Read Personal Access Tokens.
  flows: []
  scope: pat_show
- description: Create and modify Personal Access Tokens.
  flows: []
  scope: pat_edit
- description: Access role assignments.
  flows: []
  scope: roles
- description: Modify chat.
  flows: []
  scope: chat_edit
- description: Read subscription and permission settings.
  flows: []
  scope: subscription_and_permissions
slug: bexio-scopes
source_filename: bexio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://auth.bexio.com/realms/bexio/.well-known/openid-configuration (live scopes_supported, 2026-07-17)\ndocs: https://docs.bexio.com/\nnotes: >-\n  Scope list captured verbatim from the live OIDC discovery document\n  scopes_supported for the bexio Keycloak realm. bexio uses a <module>_show /\n  <module>_edit convention (show = read, edit = write). Standard OIDC scopes\n  (openid, profile, email) and offline_access (refresh tokens) are also\n  supported. Descriptions are derived from the module_action naming convention;\n  verify against the developer portal app-registration UI.\nschemes:\n- name: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://auth.bexio.com/realms/bexio\n  authorizationUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/auth\n  tokenUrl: https://auth.bexio.com/realms/bexio/protocol/openid-connect/token\n  source: https://auth.bexio.com/realms/bexio/.well-known/openid-configuration\n\
  scopes:\n- {scope: openid, description: OIDC authentication (subject identifier).}\n- {scope: profile, description: OIDC standard profile claims.}\n- {scope: email, description: OIDC email claim.}\n- {scope: offline_access, description: Issue refresh tokens for long-lived server-to-server access.}\n- {scope: company_profile, description: Read the company profile.}\n- {scope: additional_company, description: Access additional companies on the account.}\n- {scope: company_memberships_show, description: Read company memberships.}\n- {scope: contact_show, description: Read contacts, relations, groups, sectors.}\n- {scope: contact_edit, description: Create and modify contacts.}\n- {scope: note_show, description: Read notes.}\n- {scope: note_edit, description: Create and modify notes.}\n- {scope: lead_show, description: Read leads.}\n- {scope: lead_edit, description: Create and modify leads.}\n- {scope: kb_offer_show, description: Read quotes/offers (Offerte).}\n- {scope: kb_offer_edit, description:\
  \ Create and modify quotes/offers.}\n- {scope: kb_order_show, description: Read orders (Auftrag).}\n- {scope: kb_order_edit, description: Create and modify orders.}\n- {scope: kb_invoice_show, description: Read invoices (Rechnung).}\n- {scope: kb_invoice_edit, description: Create and modify invoices, generate QR-bill PDFs.}\n- {scope: kb_delivery_show, description: Read delivery notes (Lieferschein).}\n- {scope: kb_delivery_edit, description: Create and modify delivery notes.}\n- {scope: kb_credit_voucher_show, description: Read credit notes (Gutschrift).}\n- {scope: kb_credit_voucher_edit, description: Create and modify credit notes.}\n- {scope: kb_bill_show, description: Read supplier bills (Lieferantenrechnungen).}\n- {scope: kb_bill_edit, description: Create and modify supplier bills.}\n- {scope: kb_expense_show, description: Read expenses (Spesen).}\n- {scope: kb_expense_edit, description: Create and modify expenses.}\n- {scope: kb_article_order_show, description: Read article/order\
  \ line items.}\n- {scope: kb_article_order_edit, description: Create and modify article/order line items.}\n- {scope: article_show, description: Read items/products (Artikel).}\n- {scope: article_edit, description: Create and modify items/products.}\n- {scope: stock_edit, description: Modify stock levels.}\n- {scope: accounting, description: Chart of accounts, journal entries, VAT, currencies.}\n- {scope: accounting_settings_show, description: Read accounting settings.}\n- {scope: accounting_settings_edit, description: Modify accounting settings.}\n- {scope: transaction_show, description: Read accounting transactions.}\n- {scope: transaction_edit, description: Create and modify accounting transactions.}\n- {scope: subledger_show, description: Read subledger data.}\n- {scope: subledger_edit, description: Modify subledger data.}\n- {scope: finance_reports, description: Access finance reports.}\n- {scope: project_show, description: Read projects.}\n- {scope: project_edit, description: Create\
  \ and modify projects.}\n- {scope: task_show, description: Read tasks.}\n- {scope: task_edit, description: Create and modify tasks.}\n- {scope: monitoring_show, description: Read time-tracking / monitoring data.}\n- {scope: monitoring_edit, description: Create and modify time-tracking entries.}\n- {scope: payroll_employee_show, description: Read payroll employees.}\n- {scope: payroll_employee_edit, description: Create and modify payroll employees.}\n- {scope: payroll_absence_show, description: Read payroll absences.}\n- {scope: payroll_absence_edit, description: Create and modify payroll absences.}\n- {scope: payroll_paystub_show, description: Read paystubs.}\n- {scope: payroll_time_account_show, description: Read payroll time accounts.}\n- {scope: payroll_time_account_edit, description: Modify payroll time accounts.}\n- {scope: payroll_statistic_show, description: Read payroll statistics.}\n- {scope: bank_account_show, description: Read bank accounts.}\n- {scope: bank_account_edit, description:\
  \ Create and modify bank accounts.}\n- {scope: bank_payment_show, description: Read bank payments.}\n- {scope: bank_payment_edit, description: Create and modify bank payments.}\n- {scope: bill_banking_payment_edit, description: Create bill banking payments (pay supplier bills).}\n- {scope: file, description: Upload, list, and manage files and attachments.}\n- {scope: archive_show, description: Read archived documents.}\n- {scope: archive_edit, description: Modify archived documents.}\n- {scope: archive_settings_show, description: Read archive settings.}\n- {scope: archive_settings_edit, description: Modify archive settings.}\n- {scope: connected_clients_show, description: Read connected clients (accountant sharing).}\n- {scope: connected_clients_edit, description: Modify connected clients.}\n- {scope: pat_show, description: Read Personal Access Tokens.}\n- {scope: pat_edit, description: Create and modify Personal Access Tokens.}\n- {scope: roles, description: Access role assignments.}\n\
  - {scope: chat_edit, description: Modify chat.}\n- {scope: subscription_and_permissions, description: Read subscription and permission settings.}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bexio/refs/heads/main/scopes/bexio-scopes.yml
summary_line: 71 scopes
tags:
- Accounting
- ERP
- Invoicing
- SMB
- Switzerland
token_urls: []
---
