---
api_specs:
- filename: openapi-specifications
  format: yaml
  label: QuickBooks Online Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://developer.intuit.com/app/developer/qbo/docs/develop/explore-the-quickbooks-online-api/openapi-specifications
authorization_urls:
- https://appcenter.intuit.com/connect/oauth2
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Quickbooks Online Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'QuickBooks Online publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the QuickBooks Online API on a user''s behalf.


  Tokens are issued from https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: QuickBooks Online
provider_slug: quickbooks-online
schemes:
- description: Intuit OAuth 2.0
  flows:
  - authorizationUrl: https://appcenter.intuit.com/connect/oauth2
    flow: authorizationCode
    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
  name: OAuth2
  source: openapi/quickbooks-online-openapi.yml
scope_count: 5
scope_names:
- com.intuit.quickbooks.accounting
- com.intuit.quickbooks.payment
- email
- openid
- profile
scopes:
- description: Accounting scope
  flows:
  - authorizationCode
  scope: com.intuit.quickbooks.accounting
- description: Payments scope
  flows:
  - authorizationCode
  scope: com.intuit.quickbooks.payment
- description: User email
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: User profile
  flows:
  - authorizationCode
  scope: profile
slug: quickbooks-online-scopes
source_filename: quickbooks-online-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/quickbooks-online-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/quickbooks-online-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://appcenter.intuit.com/connect/oauth2\n    tokenUrl: https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer\n  description: Intuit OAuth 2.0\nscopes:\n- scope: com.intuit.quickbooks.accounting\n  description: Accounting scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n- scope: com.intuit.quickbooks.payment\n  description: Payments scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n- scope: email\n  description: User email\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n- scope: profile\n\
  \  description: User profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/quickbooks-online-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quickbooks-online/refs/heads/main/scopes/quickbooks-online-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Accounting
- Bookkeeping
- Invoicing
- Small Business
- Finance
- Payments
- Payroll
token_urls:
- https://oauth.platform.intuit.com/oauth2/v1/tokens/bearer
---
