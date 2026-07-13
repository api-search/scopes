---
api_specs:
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Report v3 API
  slug: expense-report-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Expense Entry v3 API
  slug: expense-entry-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Quick Expense v3 API
  slug: quick-expense-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
- filename: sap-concur-expense-report-openapi.yml
  format: yaml
  label: Receipt Image v3 API
  slug: receipt-image-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/openapi/sap-concur-expense-report-openapi.yml
authorization_urls:
- https://us.api.concursolutions.com/oauth2/v0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sap Concur Expense Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SAP Concur Expense publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SAP Concur Expense API on a user''s behalf.


  Tokens are issued from https://us.api.concursolutions.com/oauth2/v0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
schemes:
- flows:
  - authorizationUrl: https://us.api.concursolutions.com/oauth2/v0/authorize
    flow: authorizationCode
    tokenUrl: https://us.api.concursolutions.com/oauth2/v0/token
  name: OAuth2
  source: openapi/sap-concur-expense-report-openapi.yml
scope_count: 3
scope_names:
- expense.report.delete
- expense.report.read
- expense.report.write
scopes:
- description: Delete expense reports
  flows:
  - authorizationCode
  scope: expense.report.delete
- description: Read expense reports
  flows:
  - authorizationCode
  scope: expense.report.read
- description: Create and modify expense reports
  flows:
  - authorizationCode
  scope: expense.report.write
slug: sap-concur-expense-scopes
source_filename: sap-concur-expense-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-concur-expense-report-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sap-concur-expense-report-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.api.concursolutions.com/oauth2/v0/authorize\n    tokenUrl: https://us.api.concursolutions.com/oauth2/v0/token\nscopes:\n- scope: expense.report.delete\n  description: Delete expense reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sap-concur-expense-report-openapi.yml\n- scope: expense.report.read\n  description: Read expense reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sap-concur-expense-report-openapi.yml\n- scope: expense.report.write\n  description: Create and modify expense reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sap-concur-expense-report-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/scopes/sap-concur-expense-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
token_urls:
- https://us.api.concursolutions.com/oauth2/v0/token
---
