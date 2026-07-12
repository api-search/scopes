---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bank Of America Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bank of America publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bank of America API on a user''s behalf.


  Tokens are issued from https://api.bankofamerica.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bank of America
provider_slug: bank-of-america
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.bankofamerica.com/oauth/token
  name: OAuth2
  source: openapi/bank-of-america-cashpro-api-openapi.yml
scope_count: 4
scope_names:
- accounts:read
- payments:write
- statements:read
- transactions:read
scopes:
- description: Read account information and balances
  flows:
  - clientCredentials
  scope: accounts:read
- description: Initiate and manage payments
  flows:
  - clientCredentials
  scope: payments:write
- description: Access account statements
  flows:
  - clientCredentials
  scope: statements:read
- description: Read transaction history
  flows:
  - clientCredentials
  scope: transactions:read
slug: bank-of-america-scopes
source_filename: bank-of-america-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bank-of-america-cashpro-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/bank-of-america-cashpro-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.bankofamerica.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account information and balances\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bank-of-america-cashpro-api-openapi.yml\n- scope: payments:write\n  description: Initiate and manage payments\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bank-of-america-cashpro-api-openapi.yml\n- scope: statements:read\n  description: Access account statements\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bank-of-america-cashpro-api-openapi.yml\n- scope: transactions:read\n  description: Read transaction history\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bank-of-america-cashpro-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/scopes/bank-of-america-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
- Fortune 100
token_urls:
- https://api.bankofamerica.com/oauth/token
---
