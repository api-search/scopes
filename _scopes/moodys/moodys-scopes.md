---
api_specs:
- filename: moodys-series-api-openapi.yml
  format: yaml
  label: Moody's Data Buffet API
  slug: data-buffet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-series-api-openapi.yml
- filename: moodys-audit-api-openapi.yml
  format: yaml
  label: Moody's Audit API
  slug: moodys-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-audit-api-openapi.yml
- filename: moodys-dataseries-api-openapi.yml
  format: yaml
  label: Moody's Data Series API
  slug: moodys-dataseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-dataseries-api-openapi.yml
- filename: moodys-forecast-api-openapi.yml
  format: yaml
  label: Moody's Forecast API
  slug: moodys-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-forecast-api-openapi.yml
- filename: moodys-interpolation-api-openapi.yml
  format: yaml
  label: Moody's Interpolation API
  slug: moodys-interpolation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-interpolation-api-openapi.yml
- filename: moodys-order-api-openapi.yml
  format: yaml
  label: Moody's Order API
  slug: moodys-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-order-api-openapi.yml
- filename: moodys-project-api-openapi.yml
  format: yaml
  label: Moody's Project API
  slug: moodys-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-project-api-openapi.yml
- filename: moodys-scenario-api-openapi.yml
  format: yaml
  label: Moody's Scenario API
  slug: moodys-scenario-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-scenario-api-openapi.yml
- filename: moodys-seriessearch-api-openapi.yml
  format: yaml
  label: Moody's Series Search API
  slug: moodys-seriessearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-seriessearch-api-openapi.yml
- filename: moodys-universe-api-openapi.yml
  format: yaml
  label: Moody's Universe API
  slug: moodys-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-universe-api-openapi.yml
- filename: moodys-vin-api-openapi.yml
  format: yaml
  label: Moody's Vin API
  slug: moodys-vin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-vin-api-openapi.yml
- filename: moodys-frequency-api-openapi.yml
  format: yaml
  label: Moody's Frequency API
  slug: moodys-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-frequency-api-openapi.yml
- filename: moodys-multiseries-api-openapi.yml
  format: yaml
  label: Moody's Multi Series API
  slug: moodys-multiseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-multiseries-api-openapi.yml
- filename: moodys-vintage-api-openapi.yml
  format: yaml
  label: Moody's Vintage API
  slug: moodys-vintage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-vintage-api-openapi.yml
- filename: moodys-file-types-api-openapi.yml
  format: yaml
  label: Moody's File Types API
  slug: moodys-file-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-file-types-api-openapi.yml
- filename: moodys-health-check-api-openapi.yml
  format: yaml
  label: Moody's Health Check API
  slug: moodys-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-health-check-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Moodys Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Moody''s uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.economy.com/scenario-studio/v2/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moody's
provider_slug: moodys
schemes:
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-audit-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-baskets-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-dataseries-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-file-types-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-forecast-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-frequency-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-health-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-health-check-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-interpolation-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-multiseries-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-order-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-orders-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-project-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-reference-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-scenario-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-search-api-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-series-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-seriessearch-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-universe-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-vin-api-openapi.yml
- description: OAuth2 Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-vintage-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: moodys-scopes
source_filename: moodys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/moodys-audit-api-openapi.yml, openapi/moodys-baskets-api-openapi.yml, openapi/moodys-dataseries-api-openapi.yml,\n  openapi/moodys-file-types-api-openapi.yml, openapi/moodys-forecast-api-openapi.yml, openapi/moodys-frequency-api-openapi.yml,\n  openapi/moodys-health-api-openapi.yml, openapi/moodys-health-check-api-openapi.yml, openapi/moodys-interpolation-api-openapi.yml,\n  openapi/moodys-multiseries-api-openapi.yml, openapi/moodys-order-api-openapi.yml, openapi/moodys-orders-api-openapi.yml,\n  openapi/moodys-project-api-openapi.yml, openapi/moodys-reference-api-openapi.yml, openapi/moodys-scenario-api-openapi.yml,\n  openapi/moodys-search-api-openapi.yml, openapi/moodys-series-api-openapi.yml, openapi/moodys-seriessearch-api-openapi.yml,\n  openapi/moodys-universe-api-openapi.yml, openapi/moodys-vin-api-openapi.yml, openapi/moodys-vintage-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/moodys-audit-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-baskets-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-dataseries-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-file-types-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-forecast-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-frequency-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-health-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-health-check-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-interpolation-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n\
  \  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-multiseries-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-order-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-project-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n\
  - name: oauth2\n  source: openapi/moodys-reference-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-scenario-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-search-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-series-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n\
  \  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-seriessearch-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-universe-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-vin-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token\n  description: OAuth2 Client Credentials\n- name: oauth2\n  source: openapi/moodys-vintage-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 Client\
  \ Credentials\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/scopes/moodys-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk Management
- Screening
token_bound: false
token_urls:
- https://api.economy.com/scenario-studio/v2/oauth2/token
- https://api.economy.com/data/v1/oauth2/token
- https://api.economy.com/autocycle/v1/oauth2/token
---
