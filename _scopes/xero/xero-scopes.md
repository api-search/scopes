---
api_specs:
- filename: xero-accounting-openapi.yml
  format: yaml
  label: Xero Accounting API
  slug: xero-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-accounting-openapi.yml
- filename: xero-assets-openapi.yml
  format: yaml
  label: Xero Assets API
  slug: xero-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-assets-openapi.yml
- filename: xero-bankfeeds-openapi.yml
  format: yaml
  label: Xero Bank Feeds API
  slug: xero-bank-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-bankfeeds-openapi.yml
- filename: xero-finance-openapi.yml
  format: yaml
  label: Xero Finance API
  slug: xero-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-finance-openapi.yml
- filename: xero-identity-openapi.yml
  format: yaml
  label: Xero Identity API
  slug: xero-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-identity-openapi.yml
- filename: xero-payroll-au-openapi.yml
  format: yaml
  label: Xero Payroll Australia API
  slug: xero-payroll-australia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-au-openapi.yml
- filename: xero-payroll-nz-openapi.yml
  format: yaml
  label: Xero Payroll New Zealand API
  slug: xero-payroll-new-zealand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-nz-openapi.yml
- filename: xero-payroll-uk-openapi.yml
  format: yaml
  label: Xero Payroll United Kingdom API
  slug: xero-payroll-united-kingdom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-payroll-uk-openapi.yml
- filename: xero-projects-openapi.yml
  format: yaml
  label: Xero Projects API
  slug: xero-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-projects-openapi.yml
- filename: xero-files-openapi.yml
  format: yaml
  label: Xero Files API
  slug: xero-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/openapi/xero-files-openapi.yml
authorization_urls:
- https://login.xero.com/identity/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Xero Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xero publishes 36 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xero API on a user''s behalf.


  Tokens are issued from https://identity.xero.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xero
provider_slug: xero
schemes:
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-accounting-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-assets-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-bankfeeds-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-files-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-finance-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-identity-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payroll-au-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payroll-nz-openapi.yml
- description: For more information visit https://developer.xero.com/documentation/oauth2/overview
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-payroll-uk-openapi.yml
- description: For more information
  flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-projects-openapi.yml
scope_count: 36
scope_names:
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
- email
- files
- files.read
- finance.bankstatementsplus.read
- finance.cashvalidation.read
- finance.statements.read
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
scopes:
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
slug: xero-scopes
source_filename: xero-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xero-accounting-openapi.yml, openapi/xero-assets-openapi.yml, openapi/xero-bankfeeds-openapi.yml,\n  openapi/xero-files-openapi.yml, openapi/xero-finance-openapi.yml, openapi/xero-identity-openapi.yml,\n  openapi/xero-payroll-au-openapi.yml, openapi/xero-payroll-nz-openapi.yml, openapi/xero-payroll-uk-openapi.yml,\n  openapi/xero-projects-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/xero-accounting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-assets-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-bankfeeds-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-files-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-finance-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\n- name: OAuth2\n  source: openapi/xero-identity-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n\
  \  description: For more information\n- name: OAuth2\n  source: openapi/xero-payroll-au-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-payroll-nz-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n- name: OAuth2\n  source: openapi/xero-payroll-uk-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information visit https://developer.xero.com/documentation/oauth2/overview\n\
  - name: OAuth2\n  source: openapi/xero-projects-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\n  description: For more information\nscopes:\n- scope: accounting.attachments\n  description: Grant read-write access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.attachments.read\n  description: Grant read-only access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.budgets.read\n  description: Grant read-only access to read budgets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.contacts\n  description: Grant read-write access to contacts and contact groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.contacts.read\n\
  \  description: Grant read-only access to contacts and contact groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.journals.read\n  description: Grant read-only access to journals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.reports.read\n  description: Grant read-only access to accounting reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.reports.tenninetynine.read\n  description: Grant read-only access to 1099 reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.settings\n  description: Grant read-write access to organisation and account settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.settings.read\n  description: Grant read-only access to organisation and account settings\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.transactions\n  description: Grant read-write access to bank transactions, credit notes, invoices, repeating\n    invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.transactions.read\n  description: Grant read-only access to invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: assets\n  description: Grant read-write access to fixed assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-assets-openapi.yml\n- scope: assets.read\n  description: Grant read-only access to fixed assets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-assets-openapi.yml\n- scope: bankfeeds\n  description: Grant read-write access to bankfeeds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-bankfeeds-openapi.yml\n- scope: email\n  description: Grant\
  \ read-only access to your email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n  - openapi/xero-assets-openapi.yml\n  - openapi/xero-bankfeeds-openapi.yml\n  - openapi/xero-files-openapi.yml\n  - openapi/xero-finance-openapi.yml\n  - openapi/xero-identity-openapi.yml\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-projects-openapi.yml\n- scope: files\n  description: Grant read-write access to files and folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-files-openapi.yml\n- scope: files.read\n  description: Grant read-only access to files and folders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-files-openapi.yml\n- scope: finance.bankstatementsplus.read\n  description: Grant read-only access to bank statements accounting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-openapi.yml\n- scope: finance.cashvalidation.read\n  description: Grant read-only access to bank statement\
  \ and reconcilation data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-openapi.yml\n- scope: finance.statements.read\n  description: Grant read-only access to finacial statements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-finance-openapi.yml\n- scope: openid\n  description: Grant read-only access to your open id\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n  - openapi/xero-assets-openapi.yml\n  - openapi/xero-bankfeeds-openapi.yml\n  - openapi/xero-files-openapi.yml\n  - openapi/xero-finance-openapi.yml\n  - openapi/xero-identity-openapi.yml\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-projects-openapi.yml\n- scope: paymentservices\n  description: Grant read-write access to payment services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: payroll.employees\n  description: Grant read-write access to payroll employees\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.employees.read\n  description: Grant read-only access to payroll employees\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.payruns\n  description: Grant read-write access to payroll payruns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.payruns.read\n  description: Grant read-only access to payroll payruns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.payslip\n  description: Grant read-write access to payroll payslips\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.payslip.read\n  description: Grant read-only access to payroll payslips\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.settings\n  description: Grant read-write access to payroll settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.settings.read\n  description: Grant read-only access to payroll settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.timesheets\n  description: Grant read-write access to\
  \ payroll timesheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: payroll.timesheets.read\n  description: Grant read-only access to payroll timesheets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-payroll-nz-openapi.yml\n  - openapi/xero-payroll-uk-openapi.yml\n- scope: profile\n  description: your profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n  - openapi/xero-assets-openapi.yml\n  - openapi/xero-bankfeeds-openapi.yml\n  - openapi/xero-files-openapi.yml\n  - openapi/xero-finance-openapi.yml\n  - openapi/xero-identity-openapi.yml\n  - openapi/xero-payroll-au-openapi.yml\n  - openapi/xero-projects-openapi.yml\n- scope: projects\n  description: Grant read-write access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-projects-openapi.yml\n\
  - scope: projects.read\n  description: Grant read-only access to projects\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-projects-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero/refs/heads/main/scopes/xero-scopes.yml
summary_line: 36 scopes · authorizationCode
tags:
- Accounting
- Bank Feeds
- Finance
- Financial Services
- Invoicing
- Payroll
- Small Business
token_urls:
- https://identity.xero.com/connect/token
---
