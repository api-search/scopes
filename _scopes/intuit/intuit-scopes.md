---
api_specs:
- filename: intuit-customers-api-openapi.yml
  format: yaml
  label: Intuit Customers API
  slug: intuit-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-customers-api-openapi.yml
- filename: intuit-invoices-api-openapi.yml
  format: yaml
  label: Intuit Invoices API
  slug: intuit-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-invoices-api-openapi.yml
- filename: intuit-items-api-openapi.yml
  format: yaml
  label: Intuit Items API
  slug: intuit-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-items-api-openapi.yml
- filename: intuit-payments-api-openapi.yml
  format: yaml
  label: Intuit Payments API
  slug: intuit-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intuit/openapi/intuit-payments-api-openapi.yml
authorization_urls:
- https://appcenter.intuit.com/connect/oauth2
description: ''
docs: https://developer.intuit.com/quickbooks-online/docs/learn/scopes
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Intuit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Intuit publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Intuit API on a user''s behalf.


  Tokens are issued from https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Intuit
provider_slug: intuit
schemes:
- flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: oauth2
  source: openapi/_original/quickbooks-accounting.yml
scope_count: 12
scope_names:
- com.intuit.quickbooks.accounting
- com.intuit.quickbooks.payment
- openid
- profile
- email
- phone
- address
- app-foundations.custom-field-definitions.read
- app-foundations.custom-field-definitions
- project-management.project
- indirect-tax.tax-calculation.quickbooks
- payroll.compensation.read
scopes:
- description: Grants access to the QuickBooks Online Accounting API, which focuses on accounting data.
  flows: []
  scope: com.intuit.quickbooks.accounting
- description: Grants access to the QuickBooks Payments API, which focuses on payments processing.
  flows: []
  scope: com.intuit.quickbooks.payment
- description: Grants access to OpenID Connect features, with one or more of profile, email, phone, address.
  flows: []
  scope: openid
- description: User's given and family names info
  flows: []
  scope: profile
- description: User's email address info
  flows: []
  scope: email
- description: User's phone number info
  flows: []
  scope: phone
- description: User's physical address info
  flows: []
  scope: address
- description: Grants access to read Custom Fields definition data.
  flows: []
  scope: app-foundations.custom-field-definitions.read
- description: Grants access to read and write Custom Fields definitions data.
  flows: []
  scope: app-foundations.custom-field-definitions
- description: Grants access to read and write Project data.
  flows: []
  scope: project-management.project
- description: Grants access to the Sales Tax API.
  flows: []
  scope: indirect-tax.tax-calculation.quickbooks
- description: Grants read access to pay types (i.e., compensation) using the Time API. Compensation data can only be queried for customers using QuickBooks Payroll.
  flows: []
  scope: payroll.compensation.read
slug: intuit-scopes
source_filename: intuit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: searched\nsource: https://developer.intuit.com/quickbooks-online/docs/learn/scopes\ndocs: https://developer.intuit.com/quickbooks-online/docs/learn/scopes\nschemes:\n- name: oauth2\n  source: openapi/_original/quickbooks-accounting.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\nguidance: Instead of requesting access to all scopes upfront, we recommend requesting them incrementally based on your app's current data requirements.\nscopes:\n- scope: com.intuit.quickbooks.accounting\n  api: QuickBooks Online Accounting API\n  description: Grants access to the QuickBooks Online Accounting API, which focuses on accounting data.\n  sources: [openapi/_original/quickbooks-accounting.yml, https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n- scope: com.intuit.quickbooks.payment\n  api: QuickBooks Payments\
  \ API\n  description: Grants access to the QuickBooks Payments API, which focuses on payments processing.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n- scope: openid\n  api: OpenID Connect\n  description: Grants access to OpenID Connect features, with one or more of profile, email, phone, address.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes, https://developer.api.intuit.com/.well-known/openid_configuration]\n- {scope: profile, api: OpenID Connect, description: User's given and family names info, sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]}\n- {scope: email, api: OpenID Connect, description: User's email address info, sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]}\n- {scope: phone, api: OpenID Connect, description: User's phone number info, sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]}\n- {scope: address, api: OpenID Connect,\
  \ description: User's physical address info, sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]}\n- scope: app-foundations.custom-field-definitions.read\n  api: QuickBooks Online GraphQL API\n  description: Grants access to read Custom Fields definition data.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n- scope: app-foundations.custom-field-definitions\n  api: QuickBooks Online GraphQL API\n  description: Grants access to read and write Custom Fields definitions data.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n- scope: project-management.project\n  api: QuickBooks Online GraphQL API\n  description: Grants access to read and write Project data.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n- scope: indirect-tax.tax-calculation.quickbooks\n  api: QuickBooks Online GraphQL API\n  description: Grants access to the Sales Tax API.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n\
  - scope: payroll.compensation.read\n  api: QuickBooks Online GraphQL API\n  description: Grants read access to pay types (i.e., compensation) using the Time API. Compensation data can only be queried for customers using QuickBooks Payroll.\n  sources: [https://developer.intuit.com/quickbooks-online/docs/learn/scopes]\n"
source_yaml_url: https://artifacts.apis.io/intuit/scopes/intuit-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Accounting
- Custom Fields
- Finance
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Time Tracking
- Fortune 1000
token_bound: false
token_urls:
- https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
---
