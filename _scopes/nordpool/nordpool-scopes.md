---
api_specs:
- filename: nordpool-intraday-asyncapi.yml
  format: yaml
  label: Nord Pool Intraday Trading API
  slug: nordpool-intraday-trading-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/asyncapi/nordpool-intraday-asyncapi.yml
- filename: nordpool-auction-api-openapi.yml
  format: yaml
  label: Nord Pool Auction API
  slug: nordpool-auction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-auction-api-openapi.yml
- filename: nordpool-balancemarket-api-openapi.yml
  format: yaml
  label: Nord Pool BalanceMarket API
  slug: nordpool-balancemarket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-balancemarket-api-openapi.yml
- filename: nordpool-day-ahead-prices-api-openapi.yml
  format: yaml
  label: Nord Pool Day-Ahead Prices API
  slug: nordpool-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-day-ahead-prices-api-openapi.yml
- filename: nordpool-exchangerate-api-openapi.yml
  format: yaml
  label: Nord Pool ExchangeRate API
  slug: nordpool-exchangerate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-exchangerate-api-openapi.yml
- filename: nordpool-intraday-api-openapi.yml
  format: yaml
  label: Nord Pool Intraday API
  slug: nordpool-intraday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-intraday-api-openapi.yml
- filename: nordpool-powersystem-api-openapi.yml
  format: yaml
  label: Nord Pool PowerSystem API
  slug: nordpool-powersystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-powersystem-api-openapi.yml
- filename: nordpool-pricecurves-api-openapi.yml
  format: yaml
  label: Nord Pool PriceCurves API
  slug: nordpool-pricecurves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-pricecurves-api-openapi.yml
- filename: nordpool-system-api-openapi.yml
  format: yaml
  label: Nord Pool System API
  slug: nordpool-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/openapi/nordpool-system-api-openapi.yml
authorization_urls:
- https://sts.nordpoolgroup.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Nordpool Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nord Pool publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nord Pool API on a user''s behalf.


  Tokens are issued from https://sts.nordpoolgroup.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nord Pool
provider_slug: nordpool
schemes:
- description: Oauth2 Authentication
  flows:
  - authorizationUrl: https://sts.nordpoolgroup.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://sts.nordpoolgroup.com/connect/token
  name: oauth2
  source: openapi/nordpool-market-data-openapi.yml
scope_count: 1
scope_names:
- marketdata_api
scopes:
- description: '...'
  flows:
  - authorizationCode
  scope: marketdata_api
slug: nordpool-scopes
source_filename: nordpool-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nordpool-market-data-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/nordpool-market-data-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sts.nordpoolgroup.com/connect/authorize\n    tokenUrl: https://sts.nordpoolgroup.com/connect/token\n  description: Oauth2 Authentication\nscopes:\n- scope: marketdata_api\n  description: '...'\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/nordpool-market-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordpool/refs/heads/main/scopes/nordpool-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Day-Ahead Prices
- Electricity
- Energy Markets
- Power Exchange
- Intraday Trading
- Market Data
- Europe
token_urls:
- https://sts.nordpoolgroup.com/connect/token
---
