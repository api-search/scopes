---
api_specs:
- filename: bolsai-admin-api-openapi.yml
  format: yaml
  label: Bolsai Admin API
  slug: bolsai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-admin-api-openapi.yml
- filename: bolsai-api-keys-api-openapi.yml
  format: yaml
  label: Bolsai API Keys API
  slug: bolsai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-api-keys-api-openapi.yml
- filename: bolsai-auth-api-openapi.yml
  format: yaml
  label: Bolsai Auth API
  slug: bolsai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-auth-api-openapi.yml
- filename: bolsai-billing-api-openapi.yml
  format: yaml
  label: Bolsai Billing API
  slug: bolsai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-billing-api-openapi.yml
- filename: bolsai-companies-api-openapi.yml
  format: yaml
  label: Bolsai Companies API
  slug: bolsai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-companies-api-openapi.yml
- filename: bolsai-dividends-api-openapi.yml
  format: yaml
  label: Bolsai Dividends API
  slug: bolsai-dividends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-dividends-api-openapi.yml
- filename: bolsai-feedback-api-openapi.yml
  format: yaml
  label: Bolsai Feedback API
  slug: bolsai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-feedback-api-openapi.yml
- filename: bolsai-fiis-api-openapi.yml
  format: yaml
  label: Bolsai Fiis API
  slug: bolsai-fiis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-fiis-api-openapi.yml
- filename: bolsai-financials-api-openapi.yml
  format: yaml
  label: Bolsai Financials API
  slug: bolsai-financials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-financials-api-openapi.yml
- filename: bolsai-fundamentals-api-openapi.yml
  format: yaml
  label: Bolsai Fundamentals API
  slug: bolsai-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-fundamentals-api-openapi.yml
- filename: bolsai-health-api-openapi.yml
  format: yaml
  label: Bolsai Health API
  slug: bolsai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-health-api-openapi.yml
- filename: bolsai-macro-api-openapi.yml
  format: yaml
  label: Bolsai Macro API
  slug: bolsai-macro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-macro-api-openapi.yml
- filename: bolsai-screener-api-openapi.yml
  format: yaml
  label: Bolsai Screener API
  slug: bolsai-screener-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-screener-api-openapi.yml
- filename: bolsai-stocks-api-openapi.yml
  format: yaml
  label: Bolsai Stocks API
  slug: bolsai-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-stocks-api-openapi.yml
- filename: bolsai-oauth-api-openapi.yml
  format: yaml
  label: Bolsai OAUTH API
  slug: bolsai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-oauth-api-openapi.yml
- filename: bolsai-tesouro-api-openapi.yml
  format: yaml
  label: Bolsai Tesouro API
  slug: bolsai-tesouro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bolsai/openapi/bolsai-tesouro-api-openapi.yml
authorization_urls:
- https://usebolsai.com/api/v1/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Bolsai Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Bolsai uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://usebolsai.com/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bolsai
provider_slug: bolsai
schemes:
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-companies-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-dividends-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-fiis-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-financials-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-fundamentals-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-macro-api-openapi.yml
- flows:
  - authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://usebolsai.com/api/v1/oauth/token
  name: oauth2
  source: openapi/bolsai-stocks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: bolsai-scopes
source_filename: bolsai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: none\nsource: openapi/bolsai-companies-api-openapi.yml, openapi/bolsai-dividends-api-openapi.yml,\n  openapi/bolsai-fiis-api-openapi.yml, openapi/bolsai-financials-api-openapi.yml, openapi/bolsai-fundamentals-api-openapi.yml,\n  openapi/bolsai-macro-api-openapi.yml, openapi/bolsai-stocks-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bolsai-companies-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-dividends-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-fiis-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl:\
  \ https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-financials-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-fundamentals-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-macro-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\n- name: oauth2\n  source: openapi/bolsai-stocks-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://usebolsai.com/api/v1/oauth/authorize\n    tokenUrl: https://usebolsai.com/api/v1/oauth/token\nscopes: []\nnote: The OAuth2 security\
  \ scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/bolsai/scopes/bolsai-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Finance
- Financial Data
- Market Data
- Stocks/equities
- Real Estate Funds
- Dividends
- Fundamentals
- Macroeconomic Data
- Brazil
- Developer Tools
- MCP
- AI Agents
token_bound: false
token_urls:
- https://usebolsai.com/api/v1/oauth/token
---
