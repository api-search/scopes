---
api_specs:
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Transactions API
  slug: digits-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Source Sync API
  slug: digits-com-source-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Parties API
  slug: digits-com-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Chart of Accounts API
  slug: digits-com-chart-of-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Financial Statements API
  slug: digits-com-financial-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Connections API
  slug: digits-com-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
- filename: digits-com-openapi.yml
  format: yaml
  label: Digits Organizations API
  slug: digits-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/openapi/digits-com-openapi.yml
authorization_urls:
- https://connect.digits.com/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Digits Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Digits publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Digits API on a user''s behalf.


  Tokens are issued from https://connect.digits.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Digits
provider_slug: digits-com
schemes:
- description: OAuth 2.0 authorization code grant.
  flows:
  - authorizationUrl: https://connect.digits.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://connect.digits.com/v1/oauth/token
  name: OAuth2
  source: openapi/digits-com-openapi.yml
scope_count: 2
scope_names:
- ledger.read
- ledger.write
scopes:
- description: Read ledger data and statements
  flows:
  - authorizationCode
  scope: ledger.read
- description: Sync source data into the ledger
  flows:
  - authorizationCode
  scope: ledger.write
slug: digits-com-scopes
source_filename: digits-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/digits-com-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/digits-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://connect.digits.com/v1/oauth/authorize\n    tokenUrl: https://connect.digits.com/v1/oauth/token\n  description: OAuth 2.0 authorization code grant.\nscopes:\n- scope: ledger.read\n  description: Read ledger data and statements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/digits-com-openapi.yml\n- scope: ledger.write\n  description: Sync source data into the ledger\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/digits-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digits-com/refs/heads/main/scopes/digits-com-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Accounting
- Bookkeeping
- Finance
- General Ledger
- AI
- FinTech
token_urls:
- https://connect.digits.com/v1/oauth/token
---
