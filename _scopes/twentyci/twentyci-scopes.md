---
api_specs:
- filename: twentyci-twentyapi-oauth-openapi.json
  format: json
  label: TwentyAPI OAuth Token API
  slug: twentyapi-oauth-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-oauth-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Properties API
  slug: twentyapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Agent Performance API
  slug: twentyapi-agent-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Trigger Information API
  slug: twentyapi-trigger-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Categories API
  slug: twentyapi-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Address Match API
  slug: twentyapi-address-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI Schools API
  slug: twentyapi-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI UK Housing Market Metrics API
  slug: twentyapi-uk-housing-market-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
- filename: twentyci-twentyapi-openapi.json
  format: json
  label: TwentyAPI This is Now API
  slug: twentyapi-this-is-now-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twentyci/refs/heads/main/openapi/twentyci-twentyapi-openapi.json
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
