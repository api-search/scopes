---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Alliance Data Systems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Alliance Data Systems (Bread Financial Holdings) publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Alliance Data Systems (Bread Financial Holdings) API on a user''s behalf.


  Tokens are issued from https://auth.platform.breadpayments.com/auth/sso/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Alliance Data Systems (Bread Financial Holdings)
provider_slug: alliance-data-systems
schemes:
- description: OAuth 2.0 Client Credentials flow using API + Secret keys issued from the Bread Merchant Portal.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.platform.breadpayments.com/auth/sso/token
  name: oauth2ClientCredentials
  source: openapi/bread-pay-platform-openapi.yml
scope_count: 3
scope_names:
- buyers:read
- transactions:read
- transactions:write
scopes:
- description: Read buyer records
  flows:
  - clientCredentials
  scope: buyers:read
- description: Read transactions
  flows:
  - clientCredentials
  scope: transactions:read
- description: Create, authorize, settle, refund transactions
  flows:
  - clientCredentials
  scope: transactions:write
slug: alliance-data-systems-scopes
source_filename: alliance-data-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bread-pay-platform-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/bread-pay-platform-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.platform.breadpayments.com/auth/sso/token\n  description: OAuth 2.0 Client Credentials flow using API + Secret keys issued from the Bread\n    Merchant Portal.\nscopes:\n- scope: buyers:read\n  description: Read buyer records\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bread-pay-platform-openapi.yml\n- scope: transactions:read\n  description: Read transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bread-pay-platform-openapi.yml\n- scope: transactions:write\n  description: Create, authorize, settle, refund transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bread-pay-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alliance-data-systems/refs/heads/main/scopes/alliance-data-systems-scopes.yml
summary_line: 3 scopes · clientCredentials
tags:
- Financial Services
- Fintech
- Buy Now Pay Later
- BNPL
- Bread Pay
- Private Label Credit
- Co Brand Credit Cards
- Loyalty Programs
- Marketing
- Data Driven Marketing
- Payments
- Lending
- Savings
- Personal Loans
- Consumer Banking
- Retail Finance
- Fortune 500
- NYSE BFH
- Comenity Bank
- Rebrand
token_urls:
- https://auth.platform.breadpayments.com/auth/sso/token
---
