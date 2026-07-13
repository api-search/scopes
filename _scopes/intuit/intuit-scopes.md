---
api_specs:
- filename: quickbooks-accounting.yml
  format: yaml
  label: QuickBooks Online Accounting API
  slug: quickbooks-accounting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/openapi/quickbooks-accounting.yml
authorization_urls:
- https://appcenter.intuit.com/connect/oauth2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Intuit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Intuit publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Intuit API on a user''s behalf.


  Tokens are issued from https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Intuit
provider_slug: intuit
schemes:
- description: Intuit uses OAuth 2.0 for authorization. Apps must be registered on the Intuit Developer portal to obtain client credentials. Access tokens have a 60-minute lifetime and can be refreshed using refresh tokens (100-day lifetime).
  flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: oauth2
  source: openapi/quickbooks-accounting.yml
scope_count: 1
scope_names:
- com.intuit.quickbooks.accounting
scopes:
- description: Access to QuickBooks Online Accounting API
  flows:
  - authorizationCode
  scope: com.intuit.quickbooks.accounting
slug: intuit-scopes
source_filename: intuit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quickbooks-accounting.yml\nschemes:\n- name: oauth2\n  source: openapi/quickbooks-accounting.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n  description: Intuit uses OAuth 2.0 for authorization. Apps must be registered on the Intuit\n    Developer portal to obtain client credentials. Access tokens have a 60-minute lifetime and\n    can be refreshed using refresh tokens (100-day lifetime).\nscopes:\n- scope: com.intuit.quickbooks.accounting\n  description: Access to QuickBooks Online Accounting API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-accounting.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intuit/refs/heads/main/scopes/intuit-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Accounting
- Custom Fields
- Financial
- Financial Services
- Invoicing
- Payments
- Payroll
- Project Management
- Sales Tax
- Small Business
- Tax
- Tax Preparation
- Taxes
- Time Tracking
- Fortune 1000
token_urls:
- https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
---
