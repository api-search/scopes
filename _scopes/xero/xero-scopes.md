---
api_specs:
- filename: xero-accounting-api-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-api-openapi.yml
- filename: xero-asset-api-openapi.yml
  format: yaml
  label: Xero Asset API
  slug: xero-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-asset-api-openapi.yml
- filename: xero-files-api-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-api-openapi.yml
- filename: xero-finance-api-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-api-openapi.yml
- filename: xero-identity-api-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-api-openapi.yml
- filename: xero-payrollau-api-openapi.yml
  format: yaml
  label: Xero PayrollAu API
  slug: xero-payrollau-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollau-api-openapi.yml
- filename: xero-payrollnz-api-openapi.yml
  format: yaml
  label: Xero PayrollNz API
  slug: xero-payrollnz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrollnz-api-openapi.yml
- filename: xero-payrolluk-api-openapi.yml
  format: yaml
  label: Xero PayrollUk API
  slug: xero-payrolluk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payrolluk-api-openapi.yml
- filename: xero-project-api-openapi.yml
  format: yaml
  label: Xero Project API
  slug: xero-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-project-api-openapi.yml
- filename: xero-accountdata-api-openapi.yml
  format: yaml
  label: Xero Account Data API
  slug: xero-accountdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accountdata-api-openapi.yml
- filename: xero-feedconnections-api-openapi.yml
  format: yaml
  label: Xero Feed Connections API
  slug: xero-feedconnections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-feedconnections-api-openapi.yml
- filename: xero-app-store-api-openapi.yml
  format: yaml
  label: Xero App Store API
  slug: xero-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-app-store-api-openapi.yml
- filename: xero-bank-feeds-api-openapi.yml
  format: yaml
  label: Xero Bank Feeds API
  slug: xero-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bank-feeds-api-openapi.yml
authorization_urls:
- https://login.xero.com/identity/connect/authorize
description: ''
docs: https://developer.xero.com/documentation/guides/oauth2/scopes/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Xero Scopes
name_suffix: OAuth Scopes
note: Broad scopes (accounting.transactions[.read], accounting.reports.read) are deprecated in favour of granular scopes; "Broad scopes will remain available until September 2027." Docs scopes merged with the spec-derived baseline.
overview: 'Xero publishes 68 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xero API on a user''s behalf.


  Tokens are issued from https://identity.xero.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xero
provider_slug: xero
schemes:
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-account-data-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-accounting-api-openapi.yml
- description: For more information
  flows:
  - flow: clientCredentials
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-app-store-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-asset-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-bank-feeds-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-bank-feeds-v2-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-files-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-finance-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-identity-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payrollau-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payrollau-v2-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payrollnz-api-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payrolluk-api-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-project-api-openapi.yml
scope_count: 68
scope_names:
- accountdata.balances.read
- accountdata.movements.read
- accountdata.transactions.read
- accounting.attachments
- accounting.attachments.read
- accounting.budgets.read
- accounting.contacts
- accounting.contacts.read
- accounting.journals.read
- accounting.reports.read
- accounting.reports.tenninetynine.read
- accounting.settings
- accounting.settings.read
- accounting.transactions
- accounting.transactions.read
- assets
- assets.read
- bankfeeds
- bankfeedsv2
- email
- files
- files.read
- finance.bankstatementsplus.read
- finance.cashvalidation.read
- finance.statements.read
- marketplace.billing
- openid
- paymentservices
- payroll.employees
- payroll.employees.read
- payroll.payruns
- payroll.payruns.read
- payroll.payslip
- payroll.payslip.read
- payroll.settings
- payroll.settings.read
- payroll.timesheets
- payroll.timesheets.read
- profile
- projects
- projects.read
- accounting.invoices
- accounting.invoices.read
- accounting.payments
- accounting.payments.read
- accounting.banktransactions
- accounting.banktransactions.read
- accounting.manualjournals
- accounting.manualjournals.read
- accounting.reports.aged.read
- accounting.reports.balancesheet.read
- accounting.reports.banksummary.read
- accounting.reports.budgetsummary.read
- accounting.reports.executivesummary.read
- accounting.reports.profitandloss.read
- accounting.reports.trialbalance.read
- accounting.reports.taxreports.read
- practicemanager.job
- practicemanager.job.read
- practicemanager.client
- practicemanager.client.read
- practicemanager.staff
- practicemanager.staff.read
- practicemanager.time
- practicemanager.time.read
- einvoicing
- app.connections
- offline_access
scopes:
- description: Read general ledger account balances
  flows:
  - authorizationCode
  scope: accountdata.balances.read
- description: Read general ledger account movements
  flows:
  - authorizationCode
  scope: accountdata.movements.read
- description: Read general ledger account transactions
  flows:
  - authorizationCode
  scope: accountdata.transactions.read
- description: Grant read-write access to attachments
  flows:
  - authorizationCode
  scope: accounting.attachments
- description: Grant read-only access to attachments
  flows:
  - authorizationCode
  scope: accounting.attachments.read
- description: Grant read-only access to read budgets
  flows:
  - authorizationCode
  scope: accounting.budgets.read
- description: Grant read-write access to contacts and contact groups
  flows:
  - authorizationCode
  scope: accounting.contacts
- description: Grant read-only access to contacts and contact groups
  flows:
  - authorizationCode
  scope: accounting.contacts.read
- description: Grant read-only access to journals
  flows:
  - authorizationCode
  scope: accounting.journals.read
- description: Grant read-only access to accounting reports
  flows:
  - authorizationCode
  scope: accounting.reports.read
- description: Grant read-only access to 1099 reports
  flows:
  - authorizationCode
  scope: accounting.reports.tenninetynine.read
- description: Grant read-write access to organisation and account settings
  flows:
  - authorizationCode
  scope: accounting.settings
- description: Grant read-only access to organisation and account settings
  flows:
  - authorizationCode
  scope: accounting.settings.read
- description: Grant read-write access to bank transactions, credit notes, invoices, repeating invoices
  flows:
  - authorizationCode
  scope: accounting.transactions
- description: Grant read-only access to invoices
  flows:
  - authorizationCode
  scope: accounting.transactions.read
- description: Grant read-write access to fixed assets
  flows:
  - authorizationCode
  scope: assets
- description: Grant read-only access to fixed assets
  flows:
  - authorizationCode
  scope: assets.read
- description: Grant read-write access to bankfeeds
  flows:
  - authorizationCode
  scope: bankfeeds
- description: Grant read-write access to Bank Feeds Feed Connections 2.0
  flows:
  - authorizationCode
  scope: bankfeedsv2
- description: Grant read-only access to your email
  flows:
  - authorizationCode
  scope: email
- description: Grant read-write access to files and folders
  flows:
  - authorizationCode
  scope: files
- description: Grant read-only access to files and folders
  flows:
  - authorizationCode
  scope: files.read
- description: Grant read-only access to bank statements accounting data
  flows:
  - authorizationCode
  scope: finance.bankstatementsplus.read
- description: Grant read-only access to bank statement and reconcilation data
  flows:
  - authorizationCode
  scope: finance.cashvalidation.read
- description: Grant read-only access to finacial statements
  flows:
  - authorizationCode
  scope: finance.statements.read
- description: Grant read-only access to fixed assets
  flows:
  - clientCredentials
  scope: marketplace.billing
- description: Grant read-only access to your open id
  flows:
  - authorizationCode
  scope: openid
- description: Grant read-write access to payment services
  flows:
  - authorizationCode
  scope: paymentservices
- description: Grant read-write access to payroll employees
  flows:
  - authorizationCode
  scope: payroll.employees
- description: Grant read-only access to payroll employees
  flows:
  - authorizationCode
  scope: payroll.employees.read
- description: Grant read-write access to payroll payruns
  flows:
  - authorizationCode
  scope: payroll.payruns
- description: Grant read-only access to payroll payruns
  flows:
  - authorizationCode
  scope: payroll.payruns.read
- description: Grant read-write access to payroll payslips
  flows:
  - authorizationCode
  scope: payroll.payslip
- description: Grant read-only access to payroll payslips
  flows:
  - authorizationCode
  scope: payroll.payslip.read
- description: Grant read-write access to payroll settings
  flows:
  - authorizationCode
  scope: payroll.settings
- description: Grant read-only access to payroll settings
  flows:
  - authorizationCode
  scope: payroll.settings.read
- description: Grant read-write access to payroll timesheets
  flows:
  - authorizationCode
  scope: payroll.timesheets
- description: Grant read-only access to payroll timesheets
  flows:
  - authorizationCode
  scope: payroll.timesheets.read
- description: your profile information
  flows:
  - authorizationCode
  scope: profile
- description: Grant read-write access to projects
  flows:
  - authorizationCode
  scope: projects
- description: Grant read-only access to projects
  flows:
  - authorizationCode
  scope: projects.read
- description: ''
  flows: []
  scope: accounting.invoices
- description: ''
  flows: []
  scope: accounting.invoices.read
- description: ''
  flows: []
  scope: accounting.payments
- description: ''
  flows: []
  scope: accounting.payments.read
- description: ''
  flows: []
  scope: accounting.banktransactions
- description: ''
  flows: []
  scope: accounting.banktransactions.read
- description: ''
  flows: []
  scope: accounting.manualjournals
- description: ''
  flows: []
  scope: accounting.manualjournals.read
- description: ''
  flows: []
  scope: accounting.reports.aged.read
- description: ''
  flows: []
  scope: accounting.reports.balancesheet.read
- description: ''
  flows: []
  scope: accounting.reports.banksummary.read
- description: ''
  flows: []
  scope: accounting.reports.budgetsummary.read
- description: ''
  flows: []
  scope: accounting.reports.executivesummary.read
- description: ''
  flows: []
  scope: accounting.reports.profitandloss.read
- description: ''
  flows: []
  scope: accounting.reports.trialbalance.read
- description: ''
  flows: []
  scope: accounting.reports.taxreports.read
- description: ''
  flows: []
  scope: practicemanager.job
- description: ''
  flows: []
  scope: practicemanager.job.read
- description: ''
  flows: []
  scope: practicemanager.client
- description: ''
  flows: []
  scope: practicemanager.client.read
- description: ''
  flows: []
  scope: practicemanager.staff
- description: ''
  flows: []
  scope: practicemanager.staff.read
- description: ''
  flows: []
  scope: practicemanager.time
- description: ''
  flows: []
  scope: practicemanager.time.read
- description: ''
  flows: []
  scope: einvoicing
- description: ''
  flows: []
  scope: app.connections
- description: ''
  flows: []
  scope: offline_access
slug: xero-scopes
source_filename: xero-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: openapi/xero-account-data-api-openapi.yml, openapi/xero-accounting-api-openapi.yml, openapi/xero-app-store-api-openapi.yml, openapi/xero-asset-api-openapi.yml, openapi/xero-bank-feeds-api-openapi.yml,\n  openapi/xero-bank-feeds-v2-api-openapi.yml, openapi/xero-files-api-openapi.yml, openapi/xero-finance-api-openapi.yml, openapi/xero-identity-api-openapi.yml, openapi/xero-payrollau-api-openapi.yml, openapi/xero-payrollau-v2-api-openapi.yml,\n  openapi/xero-payrollnz-api-openapi.yml, openapi/xero-payrolluk-api-openapi.yml, openapi/xero-project-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/xero-account-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source:\
  \ openapi/xero-accounting-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-app-store-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-asset-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-bank-feeds-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n\
  - name: OAuth2\n  source: openapi/xero-bank-feeds-v2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-files-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-finance-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-identity-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n\
  \    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-payrollau-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-payrollau-v2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-payrollnz-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description:\
  \ For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-payrolluk-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-project-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\nscopes:\n- scope: accountdata.balances.read\n  description: Read general ledger account balances\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-account-data-api-openapi.yml\n- scope: accountdata.movements.read\n  description: Read general ledger account movements\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-account-data-api-openapi.yml\n- scope: accountdata.transactions.read\n  description: Read general ledger account transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-account-data-api-openapi.yml\n- scope: accounting.attachments\n  description: Grant read-write access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View and manage your attachments Accounts, BankTransactions, BankTransfers, Contacts, CreditNotes, Invoices, LinkedTransactions, ManualJournals, PurchaseOrders, Receipts, RepeatingInvoices\n- scope: accounting.attachments.read\n  description: Grant read-only access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your attachments As above but GET only\n- scope: accounting.budgets.read\n  description: Grant read-only access to read budgets\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your budgets Budgets\n- scope: accounting.contacts\n  description: Grant read-write access to contacts and contact groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View and manage your contacts Contacts, ContactGroups\n- scope: accounting.contacts.read\n  description: Grant read-only access to contacts and contact groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your contacts As above but GET only\n- scope: accounting.journals.read\n  description: Grant read-only access to journals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your general ledger Journals\n- scope: accounting.reports.read\n  description: Grant read-only access to accounting reports\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your reports AgedPayablesByContact, AgedReceivablesByContact, BalanceSheet, BankSummary, BASReport, BudgetSummary, ExecutiveSummary, GSTReport, ProfitAndLoss, TrialBalance\n  status: deprecated\n- scope: accounting.reports.tenninetynine.read\n  description: Grant read-only access to 1099 reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your 1099 reports 1099Report\n- scope: accounting.settings\n  description: Grant read-write access to organisation and account settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View and manage your organisation settings Accounts, BrandingThemes, Currencies, Items, InvoiceReminders, Organisation, TaxRates, TrackingCategories, Users\n- scope: accounting.settings.read\n  description: Grant read-only access to organisation and account settings\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your organisation settings As above but GET only\n- scope: accounting.transactions\n  description: Grant read-write access to bank transactions, credit notes, invoices, repeating invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View and manage your business transactions BankTransactions, BankTransfers, BatchPayments, CreditNotes, ExpenseClaims, Invoices, LinkedTransactions, ManualJournals, Overpayments, Quotes\n  status: deprecated\n- scope: accounting.transactions.read\n  description: Grant read-only access to invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View your business transactions As above but GET only\n  status: deprecated\n- scope: assets\n  description: Grant read-write access to fixed assets\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-asset-api-openapi.yml\n  docs_description: View and manage your fixed assets Assets, Asset Types, Settings\n- scope: assets.read\n  description: Grant read-only access to fixed assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-asset-api-openapi.yml\n  docs_description: View your fixed assets As above but GET only\n- scope: bankfeeds\n  description: Grant read-write access to bankfeeds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-bank-feeds-api-openapi.yml\n  docs_description: Legacy scope for existing 1.0 integrations. Feed Connections 1.0, Statements API\n- scope: bankfeedsv2\n  description: Grant read-write access to Bank Feeds Feed Connections 2.0\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-bank-feeds-v2-api-openapi.yml\n  docs_description: View and manage Feed Connections 2.0 and Statements 1.0. Use this scope for new integrations. Feed Connections 2.0, Statements API\n- scope: email\n  description:\
  \ Grant read-only access to your email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  - openapi/xero-asset-api-openapi.yml\n  - openapi/xero-bank-feeds-api-openapi.yml\n  - openapi/xero-bank-feeds-v2-api-openapi.yml\n  - openapi/xero-files-api-openapi.yml\n  - openapi/xero-finance-api-openapi.yml\n  - openapi/xero-identity-api-openapi.yml\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-project-api-openapi.yml\n  docs_description: email address\n- scope: files\n  description: Grant read-write access to files and folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-files-api-openapi.yml\n  docs_description: View and manage your file library Files, Folders, Associations\n- scope: files.read\n  description: Grant read-only access to files and folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-files-api-openapi.yml\n  docs_description: View your file library As above but GET only\n- scope: finance.bankstatementsplus.read\n\
  \  description: Grant read-only access to bank statements accounting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-api-openapi.yml\n  docs_description: View your Bank statement and reconciled transactions Bank Statements Plus\n- scope: finance.cashvalidation.read\n  description: Grant read-only access to bank statement and reconcilation data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-api-openapi.yml\n  docs_description: View your Bank statement and reconciliation data Cash Validation\n- scope: finance.statements.read\n  description: Grant read-only access to finacial statements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-api-openapi.yml\n  docs_description: View your financial statements Financial Statements\n- scope: marketplace.billing\n  description: Grant read-only access to fixed assets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/xero-app-store-api-openapi.yml\n  docs_description: View\
  \ and manage Xero App Store data Access to Xero App Store endpoints\n- scope: openid\n  description: Grant read-only access to your open id\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  - openapi/xero-asset-api-openapi.yml\n  - openapi/xero-bank-feeds-api-openapi.yml\n  - openapi/xero-bank-feeds-v2-api-openapi.yml\n  - openapi/xero-files-api-openapi.yml\n  - openapi/xero-finance-api-openapi.yml\n  - openapi/xero-identity-api-openapi.yml\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-project-api-openapi.yml\n  docs_description: your application intends to use the user’s identity\n- scope: paymentservices\n  description: Grant read-write access to payment services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  docs_description: View and manage your payment services PaymentServices\n- scope: payroll.employees\n  description: Grant read-write access to payroll employees\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View and manage your employees Employees, LeaveApplications\n- scope: payroll.employees.read\n  description: Grant read-only access to payroll employees\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View your employees As above but GET only\n- scope: payroll.payruns\n  description: Grant read-write access to payroll payruns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View and manage your pay runs Payruns\n- scope: payroll.payruns.read\n  description: Grant read-only access to payroll payruns\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View your pay runs As above but GET only\n- scope: payroll.payslip\n  description: Grant read-write access to payroll payslips\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View and manage your payslips Payslips\n- scope: payroll.payslip.read\n  description: Grant read-only access to payroll payslips\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View your payslips As above but GET only\n- scope: payroll.settings\n  description: Grant read-write access to payroll settings\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View and manage your payroll settings Settings, PayrollCalendars, PayItems, SuperFunds, SuperFundProducts\n- scope: payroll.settings.read\n  description: Grant read-only access to payroll settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View your payroll settings As above but GET only\n- scope: payroll.timesheets\n  description: Grant read-write access to payroll timesheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollau-v2-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View and manage your timesheets Timesheets\n- scope: payroll.timesheets.read\n\
  \  description: Grant read-only access to payroll timesheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-payrollau-v2-api-openapi.yml\n  - openapi/xero-payrollnz-api-openapi.yml\n  - openapi/xero-payrolluk-api-openapi.yml\n  docs_description: View your timesheets As above but GET only\n- scope: profile\n  description: your profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-api-openapi.yml\n  - openapi/xero-asset-api-openapi.yml\n  - openapi/xero-bank-feeds-api-openapi.yml\n  - openapi/xero-bank-feeds-v2-api-openapi.yml\n  - openapi/xero-files-api-openapi.yml\n  - openapi/xero-finance-api-openapi.yml\n  - openapi/xero-identity-api-openapi.yml\n  - openapi/xero-payrollau-api-openapi.yml\n  - openapi/xero-project-api-openapi.yml\n  docs_description: first name, last name, full name and xero user id\n- scope: projects\n  description: Grant read-write access to projects\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-project-api-openapi.yml\n  docs_description: View and manage your projects Projects, Tasks, Time\n- scope: projects.read\n  description: Grant read-only access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-project-api-openapi.yml\n  docs_description: View your projects As above but GET only\n- scope: accounting.invoices\n  sources:\n  - docs\n  docs_description: View and manage invoices CreditNotes, Invoices, LinkedTransactions, Quotes, PurchaseOrders, RepeatingInvoices, Items\n  status: new\n- scope: accounting.invoices.read\n  sources:\n  - docs\n  docs_description: View invoices As above but GET only\n  status: new\n- scope: accounting.payments\n  sources:\n  - docs\n  docs_description: View and manage payments BatchPayments, Overpayments, Payments, Prepayments\n  status: new\n- scope: accounting.payments.read\n  sources:\n  - docs\n  docs_description: View payments As above but GET only\n  status: new\n- scope: accounting.banktransactions\n\
  \  sources:\n  - docs\n  docs_description: View and manage bank transactions BankTransactions, BankTransfers\n  status: new\n- scope: accounting.banktransactions.read\n  sources:\n  - docs\n  docs_description: View bank transactions As above but GET only\n  status: new\n- scope: accounting.manualjournals\n  sources:\n  - docs\n  docs_description: View and manage manual journals ManualJournals\n  status: new\n- scope: accounting.manualjournals.read\n  sources:\n  - docs\n  docs_description: View manual journals As above but GET only\n  status: new\n- scope: accounting.reports.aged.read\n  sources:\n  - docs\n  docs_description: View aged reports AgedPayablesByContact, AgedReceivablesByContact\n  status: new\n- scope: accounting.reports.balancesheet.read\n  sources:\n  - docs\n  docs_description: View balance sheets BalanceSheet\n  status: new\n- scope: accounting.reports.banksummary.read\n  sources:\n  - docs\n  docs_description: View bank summary BankSummary\n  status: new\n- scope: accounting.reports.budgetsummary.read\n\
  \  sources:\n  - docs\n  docs_description: View budget summary BudgetSummary\n  status: new\n- scope: accounting.reports.executivesummary.read\n  sources:\n  - docs\n  docs_description: View executive summary ExecutiveSummary\n  status: new\n- scope: accounting.reports.profitandloss.read\n  sources:\n  - docs\n  docs_description: View profit and loss ProfitAndLoss\n  status: new\n- scope: accounting.reports.trialbalance.read\n  sources:\n  - docs\n  docs_description: View trial balance TrialBalance\n  status: new\n- scope: accounting.reports.taxreports.read\n  sources:\n  - docs\n  docs_description: View GST or BAS reports GSTReport, BASReport\n  status: new\n- scope: practicemanager.job\n  sources:\n  - docs\n  docs_description: View and manage your Practice Manager job data Access to job endpoints\n- scope: practicemanager.job.read\n  sources:\n  - docs\n  docs_description: View your Practice Manager job data As above but GET only\n- scope: practicemanager.client\n  sources:\n  - docs\n\
  \  docs_description: View and manage your Practice Manager client data Access to client endpoints and client group endpoints\n- scope: practicemanager.client.read\n  sources:\n  - docs\n  docs_description: View your Practice Manager client data As above but GET only\n- scope: practicemanager.staff\n  sources:\n  - docs\n  docs_description: View and manage your Practice Manager staff data Access to staff endpoints\n- scope: practicemanager.staff.read\n  sources:\n  - docs\n  docs_description: View your Practice Manager staff data As above but GET only\n- scope: practicemanager.time\n  sources:\n  - docs\n  docs_description: View and manage your Practice Manager time data Access to time endpoints\n- scope: practicemanager.time.read\n  sources:\n  - docs\n  docs_description: View your Practice Manager time data As above but GET only\n- scope: einvoicing\n  sources:\n  - docs\n  docs_description: View and manage registration information eInvoicing\n- scope: app.connections\n  sources:\n  -\
  \ docs\n  docs_description: View your connection data Access to Connections endpoint\n- scope: offline_access\n  sources:\n  - docs\n  docs_description: To get a refresh token, you must request the offline_access scope.\ndocs: https://developer.xero.com/documentation/guides/oauth2/scopes/\nnote: Broad scopes (accounting.transactions[.read], accounting.reports.read) are deprecated in favour of granular scopes; \"Broad scopes will remain available until September 2027.\" Docs scopes merged with\n  the spec-derived baseline.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/scopes/xero-scopes.yml
summary_line: 68 scopes · authorizationCode/clientCredentials
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
token_bound: false
token_urls:
- https://identity.xero.com/connect/token
---
