---
api_specs:
- filename: charles-schwab-trader-api-openapi.yml
  format: yaml
  label: Charles Schwab Trader API
  slug: trader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-trader-api-openapi.yml
- filename: charles-schwab-market-data-api-openapi.yml
  format: yaml
  label: Charles Schwab Market Data API
  slug: market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/openapi/charles-schwab-market-data-api-openapi.yml
authorization_urls:
- https://api.schwabapi.com/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Charles Schwab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Charles Schwab publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Charles Schwab API on a user''s behalf.


  Tokens are issued from https://api.schwabapi.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Charles Schwab
provider_slug: charles-schwab
schemes:
- flows:
  - authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schwabapi.com/v1/oauth/token
  name: oauth2
  source: openapi/charles-schwab-market-data-api-openapi.yml
- flows:
  - authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.schwabapi.com/v1/oauth/token
  name: oauth2
  source: openapi/charles-schwab-trader-api-openapi.yml
scope_count: 1
scope_names:
- api
scopes:
- description: Access Schwab Trader and Market Data APIs
  flows:
  - authorizationCode
  scope: api
slug: charles-schwab-scopes
source_filename: charles-schwab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charles-schwab-market-data-api-openapi.yml, openapi/charles-schwab-trader-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/charles-schwab-market-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize\n    tokenUrl: https://api.schwabapi.com/v1/oauth/token\n- name: oauth2\n  source: openapi/charles-schwab-trader-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.schwabapi.com/v1/oauth/authorize\n    tokenUrl: https://api.schwabapi.com/v1/oauth/token\nscopes:\n- scope: api\n  description: Access Schwab Trader and Market Data APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charles-schwab-market-data-api-openapi.yml\n  - openapi/charles-schwab-trader-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charles-schwab/refs/heads/main/scopes/charles-schwab-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Accounts
- Banking
- Brokerage
- Financial Services
- Investing
- Market Data
- OAuth 2.0
- Orders
- Trading
- Fortune 500
token_urls:
- https://api.schwabapi.com/v1/oauth/token
---
