---
api_specs:
- filename: citizens-bank-accounts-api-openapi.yml
  format: yaml
  label: Citizens Bank Accounts API
  slug: accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/openapi/citizens-bank-accounts-api-openapi.yml
- filename: citizens-bank-atm-locator-api-openapi.yml
  format: yaml
  label: Citizens Bank ATM Locator API
  slug: atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/openapi/citizens-bank-atm-locator-api-openapi.yml
authorization_urls:
- https://api.citizensbank.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Citizens Financial Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Citizens Financial publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Citizens Financial API on a user''s behalf.


  Tokens are issued from https://api.citizensbank.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Citizens Financial
provider_slug: citizens-financial
schemes:
- flows:
  - authorizationUrl: https://api.citizensbank.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.citizensbank.com/oauth/token
  name: oauth2
  source: openapi/citizens-bank-accounts-api-openapi.yml
scope_count: 2
scope_names:
- accounts:read
- transactions:read
scopes:
- description: Read account information
  flows:
  - authorizationCode
  scope: accounts:read
- description: Read transaction history
  flows:
  - authorizationCode
  scope: transactions:read
slug: citizens-financial-scopes
source_filename: citizens-financial-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/citizens-bank-accounts-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/citizens-bank-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.citizensbank.com/oauth/authorize\n    tokenUrl: https://api.citizensbank.com/oauth/token\nscopes:\n- scope: accounts:read\n  description: Read account information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/citizens-bank-accounts-api-openapi.yml\n- scope: transactions:read\n  description: Read transaction history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/citizens-bank-accounts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial/refs/heads/main/scopes/citizens-financial-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Accounts
- ATMs
- Banking
- Open Banking
- Payments
- Point of Sale
- Transactions
token_urls:
- https://api.citizensbank.com/oauth/token
---
