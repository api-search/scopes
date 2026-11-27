---
api_specs:
- filename: helious-io-agent-sign-in-and-a2a-api-openapi.yml
  format: yaml
  label: Helious Agent sign-in and A2A API
  slug: helious-io-agent-sign-in-and-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-agent-sign-in-and-a2a-api-openapi.yml
- filename: helious-io-ask-helious-api-openapi.yml
  format: yaml
  label: Helious Ask Helious API
  slug: helious-io-ask-helious-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-ask-helious-api-openapi.yml
- filename: helious-io-boards-api-openapi.yml
  format: yaml
  label: Helious Boards API
  slug: helious-io-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-boards-api-openapi.yml
- filename: helious-io-economic-data-api-openapi.yml
  format: yaml
  label: Helious Economic data API
  slug: helious-io-economic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-economic-data-api-openapi.yml
- filename: helious-io-news-and-feed-api-openapi.yml
  format: yaml
  label: Helious News and feed API
  slug: helious-io-news-and-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-news-and-feed-api-openapi.yml
- filename: helious-io-rates-and-curve-api-openapi.yml
  format: yaml
  label: Helious Rates and curve API
  slug: helious-io-rates-and-curve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-rates-and-curve-api-openapi.yml
- filename: helious-io-reference-api-openapi.yml
  format: yaml
  label: Helious Reference API
  slug: helious-io-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-reference-api-openapi.yml
- filename: helious-io-series-api-openapi.yml
  format: yaml
  label: Helious Series API
  slug: helious-io-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-series-api-openapi.yml
- filename: helious-io-the-fed-api-openapi.yml
  format: yaml
  label: Helious The Fed API
  slug: helious-io-the-fed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-the-fed-api-openapi.yml
- filename: helious-io-the-squawk-api-openapi.yml
  format: yaml
  label: Helious The squawk API
  slug: helious-io-the-squawk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-the-squawk-api-openapi.yml
- filename: helious-io-treasury-auctions-api-openapi.yml
  format: yaml
  label: Helious Treasury auctions API
  slug: helious-io-treasury-auctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-treasury-auctions-api-openapi.yml
- filename: helious-io-your-key-api-openapi.yml
  format: yaml
  label: Helious Your key API
  slug: helious-io-your-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-your-key-api-openapi.yml
authorization_urls:
- https://helious.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Helious Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Helious publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Helious API on a user''s behalf.


  Tokens are issued from https://api.helious.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Helious
provider_slug: helious-io
schemes:
- description: Sign the person in instead of asking them for a key. Dynamic client registration is open, so your client can enrol itself; the one human step is the consent screen. Access tokens last an hour; ask for offline_access to get a rotating refresh token. Full details at https://helious.io/auth.md.
  flows:
  - authorizationUrl: https://helious.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.helious.io/oauth/token
  name: helious_oauth
  source: openapi/helious-io-openapi.json
scope_count: 4
scope_names:
- account:read
- market:read
- offline_access
- openid
scopes:
- description: See which plan the account is on.
  flows:
  - authorizationCode
  scope: account:read
- description: Read Helious market data at that plan level.
  flows:
  - authorizationCode
  scope: market:read
- description: Get a refresh token so you stay connected.
  flows:
  - authorizationCode
  scope: offline_access
- description: Confirm the account identity to your app.
  flows:
  - authorizationCode
  scope: openid
slug: helious-io-scopes
source_filename: helious-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/helious-io-openapi.json\nschemes:\n- name: helious_oauth\n  source: openapi/helious-io-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://helious.io/oauth/authorize\n    tokenUrl: https://api.helious.io/oauth/token\n  description: Sign the person in instead of asking them for a key. Dynamic client registration\n    is open, so your client can enrol itself; the one human step is the consent screen. Access\n    tokens last an hour; ask for offline_access to get a rotating refresh token. Full details\n    at https://helious.io/auth.md.\nscopes:\n- scope: account:read\n  description: See which plan the account is on.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/helious-io-openapi.json\n- scope: market:read\n  description: Read Helious market data at that plan level.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/helious-io-openapi.json\n- scope: offline_access\n  description:\
  \ Get a refresh token so you stay connected.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/helious-io-openapi.json\n- scope: openid\n  description: Confirm the account identity to your app.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/helious-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/helious-io/scopes/helious-io-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Finance
- Market Data
- News
- Economic Calendar
- Treasury
token_bound: false
token_urls:
- https://api.helious.io/oauth/token
---
