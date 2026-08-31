---
api_specs:
- filename: twentyci-address-match-api-openapi.yml
  format: yaml
  label: TwentyCi Address Match API
  slug: twentyci-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-address-match-api-openapi.yml
- filename: twentyci-agent-performance-api-openapi.yml
  format: yaml
  label: TwentyCi Agent Performance API
  slug: twentyci-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-agent-performance-api-openapi.yml
- filename: twentyci-authorisation-api-openapi.yml
  format: yaml
  label: TwentyCi Authorisation API
  slug: twentyci-authorisation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-authorisation-api-openapi.yml
- filename: twentyci-categories-api-openapi.yml
  format: yaml
  label: TwentyCi Categories API
  slug: twentyci-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-categories-api-openapi.yml
- filename: twentyci-properties-api-openapi.yml
  format: yaml
  label: TwentyCi Properties API
  slug: twentyci-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-properties-api-openapi.yml
- filename: twentyci-schools-api-openapi.yml
  format: yaml
  label: TwentyCi Schools API
  slug: twentyci-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-schools-api-openapi.yml
- filename: twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
  format: yaml
  label: TwentyCi This is Now | Retail Propensity To Buy Goods API
  slug: twentyci-this-is-now-retail-propensity-to-buy-goods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-this-is-now-retail-propensity-to-buy-goods-api-openapi.yml
- filename: twentyci-trigger-information-api-openapi.yml
  format: yaml
  label: TwentyCi Trigger Information API
  slug: twentyci-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-trigger-information-api-openapi.yml
- filename: twentyci-uk-housing-market-metrics-api-openapi.yml
  format: yaml
  label: TwentyCi UK Housing Market Metrics API
  slug: twentyci-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-uk-housing-market-metrics-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: Twentyci Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TwentyCi publishes 1 OAuth 2.0 scope via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TwentyCi API on a user''s behalf.


  Tokens are issued from https://api.twentyci.co.uk/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TwentyCi
provider_slug: twentyci
schemes:
- description: 'OAuth 2.0 bearer token. TwentyCi''s documentation labels the scheme "OAuth2" with flow "Implicit" but describes a resource-owner password-credentials exchange: POST /oauth/token with client_id, client_secret, username, password, grant_type=password and scope=* returns {token_type: Bearer, expires_in, access_token, refresh_token}. The token is then sent as "Authorization: Bearer <token-key>". Modelled here as the password flow because that is what the documented request body performs. No OpenID Connect discovery document is served (/.well-known/openid-configuration returned 404).'
  flows:
  - flow: password
    tokenUrl: https://api.twentyci.co.uk/oauth/token
  name: twentyapiOAuth
  source: openapi/twentyci-twentyapi-openapi.json
scope_count: 1
scope_names:
- '*'
scopes:
- description: Full access; the only scope value documented by TwentyCi.
  flows:
  - password
  scope: '*'
slug: twentyci-scopes
source_filename: twentyci-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/twentyci-twentyapi-openapi.json\nschemes:\n- name: twentyapiOAuth\n  source: openapi/twentyci-twentyapi-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: https://api.twentyci.co.uk/oauth/token\n  description: 'OAuth 2.0 bearer token. TwentyCi''s documentation labels the scheme \"OAuth2\"\n    with flow \"Implicit\" but describes a resource-owner password-credentials exchange: POST\n    /oauth/token with client_id, client_secret, username, password, grant_type=password and\n    scope=* returns {token_type: Bearer, expires_in, access_token, refresh_token}. The token\n    is then sent as \"Authorization: Bearer <token-key>\". Modelled here as the password flow\n    because that is what the documented request body performs. No OpenID Connect discovery document\n    is served (/.well-known/openid-configuration returned 404).'\nscopes:\n- scope: '*'\n  description: Full access; the only scope value documented by TwentyCi.\n\
  \  flows:\n  - password\n  sources:\n  - openapi/twentyci-twentyapi-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/scopes/twentyci-scopes.yml
summary_line: 1 scope · password
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Valuation
- AVM
- Rentals
- Address Data
- Conveyancing
- Homemover Data
- Agent Performance
- Data as a Service
token_urls:
- https://api.twentyci.co.uk/oauth/token
---
