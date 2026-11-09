---
api_specs:
- filename: dealroom-aggregate-api-openapi.yml
  format: yaml
  label: Dealroom Aggregate API
  slug: dealroom-aggregate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-aggregate-api-openapi.yml
- filename: dealroom-companies-api-openapi.yml
  format: yaml
  label: Dealroom Companies API
  slug: dealroom-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-companies-api-openapi.yml
- filename: dealroom-discovery-api-openapi.yml
  format: yaml
  label: Dealroom Discovery API
  slug: dealroom-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-discovery-api-openapi.yml
- filename: dealroom-entities-api-openapi.yml
  format: yaml
  label: Dealroom Entities API
  slug: dealroom-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-entities-api-openapi.yml
- filename: dealroom-filters-api-openapi.yml
  format: yaml
  label: Dealroom Filters API
  slug: dealroom-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-filters-api-openapi.yml
- filename: dealroom-founders-api-openapi.yml
  format: yaml
  label: Dealroom Founders API
  slug: dealroom-founders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-founders-api-openapi.yml
- filename: dealroom-funds-api-openapi.yml
  format: yaml
  label: Dealroom Funds API
  slug: dealroom-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-funds-api-openapi.yml
- filename: dealroom-government-ngo-api-openapi.yml
  format: yaml
  label: Dealroom Government & NGO API
  slug: dealroom-government-ngo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-government-ngo-api-openapi.yml
- filename: dealroom-health-api-openapi.yml
  format: yaml
  label: Dealroom Health API
  slug: dealroom-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-health-api-openapi.yml
- filename: dealroom-investors-api-openapi.yml
  format: yaml
  label: Dealroom Investors API
  slug: dealroom-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-investors-api-openapi.yml
- filename: dealroom-jobs-api-openapi.yml
  format: yaml
  label: Dealroom Jobs API
  slug: dealroom-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-jobs-api-openapi.yml
- filename: dealroom-news-api-openapi.yml
  format: yaml
  label: Dealroom News API
  slug: dealroom-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-news-api-openapi.yml
- filename: dealroom-notes-api-openapi.yml
  format: yaml
  label: Dealroom Notes API
  slug: dealroom-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-notes-api-openapi.yml
- filename: dealroom-people-api-openapi.yml
  format: yaml
  label: Dealroom People API
  slug: dealroom-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-people-api-openapi.yml
- filename: dealroom-search-api-openapi.yml
  format: yaml
  label: Dealroom Search API
  slug: dealroom-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-search-api-openapi.yml
- filename: dealroom-transactions-api-openapi.yml
  format: yaml
  label: Dealroom Transactions API
  slug: dealroom-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-transactions-api-openapi.yml
- filename: dealroom-universities-api-openapi.yml
  format: yaml
  label: Dealroom Universities API
  slug: dealroom-universities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-universities-api-openapi.yml
- filename: dealroom-valuations-api-openapi.yml
  format: yaml
  label: Dealroom Valuations API
  slug: dealroom-valuations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-valuations-api-openapi.yml
- filename: dealroom-time-series-api-openapi.yml
  format: yaml
  label: Dealroom Time Series API
  slug: dealroom-time-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealroom/openapi/dealroom-time-series-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Dealroom Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dealroom publishes 12 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dealroom API on a user''s behalf.


  Tokens are issued from https://accounts.dealroom.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dealroom
provider_slug: dealroom
schemes:
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-aggregate-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-companies-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-discovery-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-entities-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-filters-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-founders-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-funds-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-government-ngo-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-health-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-investors-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-jobs-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-news-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-notes-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-people-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-search-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-time-series-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-transactions-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-universities-api-openapi.yml
- description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id` / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will reuse the same token across operations. Revoking or deactivating a key rejects it on the next request (within a ≤5-minute server-side cache window), not at token expiry.
  flows:
  - flow: clientCredentials
    tokenUrl: https://accounts.dealroom.co/oauth/token
  name: oauth2
  source: openapi/dealroom-valuations-api-openapi.yml
scope_count: 12
scope_names:
- read:aggregate
- read:dimensions
- read:entities
- read:founders
- read:investors
- read:jobs
- read:news
- read:people
- read:search
- read:timeseries
- read:transactions
- read:valuations
scopes:
- description: Grant the read:aggregate permission
  flows:
  - clientCredentials
  scope: read:aggregate
- description: Grant the read:dimensions permission
  flows:
  - clientCredentials
  scope: read:dimensions
- description: Grant the read:entities permission
  flows:
  - clientCredentials
  scope: read:entities
- description: Grant the read:founders permission
  flows:
  - clientCredentials
  scope: read:founders
- description: Grant the read:investors permission
  flows:
  - clientCredentials
  scope: read:investors
- description: Grant the read:jobs permission
  flows:
  - clientCredentials
  scope: read:jobs
- description: Grant the read:news permission
  flows:
  - clientCredentials
  scope: read:news
- description: Grant the read:people permission
  flows:
  - clientCredentials
  scope: read:people
- description: Grant the read:search permission
  flows:
  - clientCredentials
  scope: read:search
- description: Grant the read:timeseries permission
  flows:
  - clientCredentials
  scope: read:timeseries
- description: Grant the read:transactions permission
  flows:
  - clientCredentials
  scope: read:transactions
- description: Grant the read:valuations permission
  flows:
  - clientCredentials
  scope: read:valuations
slug: dealroom-scopes
source_filename: dealroom-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/dealroom-aggregate-api-openapi.yml, openapi/dealroom-companies-api-openapi.yml,\n  openapi/dealroom-discovery-api-openapi.yml, openapi/dealroom-entities-api-openapi.yml, openapi/dealroom-filters-api-openapi.yml,\n  openapi/dealroom-founders-api-openapi.yml, openapi/dealroom-funds-api-openapi.yml, openapi/dealroom-government-ngo-api-openapi.yml,\n  openapi/dealroom-health-api-openapi.yml, openapi/dealroom-investors-api-openapi.yml, openapi/dealroom-jobs-api-openapi.yml,\n  openapi/dealroom-news-api-openapi.yml, openapi/dealroom-notes-api-openapi.yml, openapi/dealroom-people-api-openapi.yml,\n  openapi/dealroom-search-api-openapi.yml, openapi/dealroom-time-series-api-openapi.yml, openapi/dealroom-transactions-api-openapi.yml,\n  openapi/dealroom-universities-api-openapi.yml, openapi/dealroom-valuations-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/dealroom-aggregate-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-companies-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source:\
  \ openapi/dealroom-discovery-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-entities-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a\
  \ ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-filters-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-founders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations.\
  \ Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-funds-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-government-ngo-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens\
  \ are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-health-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-investors-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant.\
  \ Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-jobs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-news-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description:\
  \ OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-notes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-people-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-search-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-time-series-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-transactions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not\
  \ at token expiry.\n- name: oauth2\n  source: openapi/dealroom-universities-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\n- name: oauth2\n  source: openapi/dealroom-valuations-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.dealroom.co/oauth/token\n  description: OAuth2 client-credentials flow against the Dealroom Auth0 tenant. Use the `client_id`\n    / `client_secret` from a Programmatic API key. Tokens are valid for 24h — Swagger UI will\n    reuse the same token across operations. Revoking or deactivating a key\
  \ rejects it on the\n    next request (within a ≤5-minute server-side cache window), not at token expiry.\nscopes:\n- scope: read:aggregate\n  description: Grant the read:aggregate permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:dimensions\n  description: Grant the read:dimensions permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:entities\n  description: Grant the read:entities permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:founders\n  description: Grant the read:founders permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:investors\n  description: Grant the read:investors permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:jobs\n  description: Grant the read:jobs permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:news\n  description: Grant the read:news permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:people\n  description: Grant the read:people permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:search\n  description: Grant the read:search permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:timeseries\n  description: Grant the read:timeseries permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:transactions\n  description: Grant the read:transactions permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n- scope: read:valuations\n  description: Grant the read:valuations permission\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/dealroom-aggregate-api-openapi.yml\n  - openapi/dealroom-companies-api-openapi.yml\n  - openapi/dealroom-discovery-api-openapi.yml\n  - openapi/dealroom-entities-api-openapi.yml\n  - openapi/dealroom-filters-api-openapi.yml\n  - openapi/dealroom-founders-api-openapi.yml\n  - openapi/dealroom-funds-api-openapi.yml\n  - openapi/dealroom-government-ngo-api-openapi.yml\n  - openapi/dealroom-health-api-openapi.yml\n  - openapi/dealroom-investors-api-openapi.yml\n  - openapi/dealroom-jobs-api-openapi.yml\n  - openapi/dealroom-news-api-openapi.yml\n  - openapi/dealroom-notes-api-openapi.yml\n  - openapi/dealroom-people-api-openapi.yml\n  - openapi/dealroom-search-api-openapi.yml\n  - openapi/dealroom-time-series-api-openapi.yml\n  - openapi/dealroom-transactions-api-openapi.yml\n\
  \  - openapi/dealroom-universities-api-openapi.yml\n  - openapi/dealroom-valuations-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dealroom/scopes/dealroom-scopes.yml
summary_line: 12 scopes · clientCredentials
tags:
- Company
token_bound: false
token_urls:
- https://accounts.dealroom.co/oauth/token
---
