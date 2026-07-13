---
api_specs:
- filename: Xero-OpenAPI
  format: yaml
  label: Xero Accounting API
  slug: api
  spec_type: OpenAPI
  url: https://github.com/XeroAPI/Xero-OpenAPI
authorization_urls:
- https://login.xero.com/identity/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Xero Accounting Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xero Accounting publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xero Accounting API on a user''s behalf.


  Tokens are issued from https://identity.xero.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xero Accounting
provider_slug: xero-accounting
schemes:
- flows:
  - authorizationUrl: https://login.xero.com/identity/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.xero.com/connect/token
  name: OAuth2
  source: openapi/xero-accounting-openapi.yml
scope_count: 6
scope_names:
- accounting.attachments
- accounting.contacts
- accounting.journals.read
- accounting.reports.read
- accounting.settings
- accounting.transactions
scopes:
- description: Grant read/write access to attachments
  flows:
  - authorizationCode
  scope: accounting.attachments
- description: Grant read/write access to contacts and contact groups
  flows:
  - authorizationCode
  scope: accounting.contacts
- description: Grant read-only access to journals
  flows:
  - authorizationCode
  scope: accounting.journals.read
- description: Grant read-only access to accounting reports
  flows:
  - authorizationCode
  scope: accounting.reports.read
- description: Grant read/write access to organisation and account settings
  flows:
  - authorizationCode
  scope: accounting.settings
- description: Grant read/write access to bank transactions, credit notes, invoices, repeating invoices
  flows:
  - authorizationCode
  scope: accounting.transactions
slug: xero-accounting-scopes
source_filename: xero-accounting-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xero-accounting-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/xero-accounting-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.xero.com/identity/connect/authorize\n    tokenUrl: https://identity.xero.com/connect/token\nscopes:\n- scope: accounting.attachments\n  description: Grant read/write access to attachments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.contacts\n  description: Grant read/write access to contacts and contact groups\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.journals.read\n  description: Grant read-only access to journals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.reports.read\n  description: Grant read-only access to accounting reports\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.settings\n  description: Grant read/write access to organisation and account settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n- scope: accounting.transactions\n  description: Grant read/write access to bank transactions, credit notes, invoices, repeating\n    invoices\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xero-accounting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xero-accounting/refs/heads/main/scopes/xero-accounting-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Financial Reporting
- SaaS
token_urls:
- https://identity.xero.com/connect/token
---
