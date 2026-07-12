---
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
