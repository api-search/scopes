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
- filename: moodys-healthcheck-api-openapi.yml
  format: yaml
  label: Moody's Health Check API
  slug: moodys-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-healthcheck-api-openapi.yml
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
- filename: moodys-filetypes-api-openapi.yml
  format: yaml
  label: Moody's File Types API
  slug: moodys-filetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/openapi/moodys-filetypes-api-openapi.yml
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
authorization_urls: []
description: ''
docs: https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Moodys Scopes
name_suffix: OAuth Scopes
note: Moody's APIs do not use OAuth scopes — the Data Buffet API user guide (https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md) documents an OAuth2 client_credentials flow with access/encryption keys and no scope parameter, and permissions across Moody's products are tied to account entitlements and roles rather than scopes.
overview: 'Moody''s uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.economy.com/data/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moody's
provider_slug: moodys
schemes:
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-data-buffet-api-openapi.yml
- description: OAuth2 Client Credentials (Scenario Studio API) — empty scopes map.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token
  name: oauth2
  source: openapi/moodys-scenario-studio-api-swagger.json
- description: OAuth2 Client Credentials (AutoCycle API) — empty scopes map.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-autocycle-api-swagger.json
- description: OAuth2 Client Credentials (Muni Loss Forecast API) — empty scopes map.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/muni/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-municipal-api-swagger.json
scope_count: 0
scope_names: []
scopes: []
slug: moodys-scopes
source_filename: moodys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moodys-data-buffet-api-openapi.yml\ndocs: https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md\nnote: Moody's APIs do not use OAuth scopes — the Data Buffet API user guide (https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md)\n  documents an OAuth2 client_credentials flow with access/encryption keys and no scope\n  parameter, and permissions across Moody's products are tied to account entitlements\n  and roles rather than scopes.\nschemes:\n- name: oauth2\n  source: openapi/moodys-data-buffet-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\n- name: oauth2\n  source: openapi/moodys-scenario-studio-api-swagger.json\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/scenario-studio/v2/oauth2/token\n  description: OAuth2 Client Credentials (Scenario Studio API) — empty scopes map.\n- name: oauth2\n  source: openapi/moodys-autocycle-api-swagger.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/autocycle/v1/oauth2/token\n  description: OAuth2 Client Credentials (AutoCycle API) — empty scopes map.\n- name: oauth2\n  source: openapi/moodys-municipal-api-swagger.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/muni/v1/oauth2/token\n  description: OAuth2 Client Credentials (Muni Loss Forecast API) — empty scopes map.\nscopes: []\n"
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
- Risk
- Screening
token_urls:
- https://api.economy.com/data/v1/oauth2/token
- https://api.economy.com/scenario-studio/v2/oauth2/token
- https://api.economy.com/autocycle/v1/oauth2/token
- https://api.economy.com/muni/v1/oauth2/token
---
