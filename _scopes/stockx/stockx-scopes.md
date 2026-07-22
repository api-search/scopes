---
api_specs:
- filename: stockx-public-openapi-original.json
  format: json
  label: StockX Public API
  slug: stockx-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/openapi/stockx-public-openapi-original.json
authorization_urls:
- https://accounts.stockx.com/authorize
description: ''
docs: https://developer.stockx.com/portal/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Stockx Scopes
name_suffix: OAuth Scopes
note: The StockX Public API OpenAPI declares only http-bearer + api-key security schemes, but access tokens are minted by StockX's Auth0 tenant via the OAuth 2.0 Authorization Code flow. The authorization request must set audience to gateway.stockx.com. Application-level authorization (catalog/selling/orders) is governed by the developer program grant tied to the API key rather than by granular OAuth scopes; the scopes below are the identity/session scopes the Auth0 authorize endpoint accepts.
overview: 'StockX publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the StockX API on a user''s behalf.


  Tokens are issued from https://accounts.stockx.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StockX
provider_slug: stockx
schemes:
- flows:
  - audience: gateway.stockx.com
    authorizationUrl: https://accounts.stockx.com/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.stockx.com/oauth/token
  name: oauth2
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: Issue an OpenID Connect ID token for the authenticating StockX user.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so the application can obtain new access tokens without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
slug: stockx-scopes
source_filename: stockx-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://accounts.stockx.com/.well-known/openid-configuration\ndocs: https://developer.stockx.com/portal/authentication\nnote: >-\n  The StockX Public API OpenAPI declares only http-bearer + api-key security\n  schemes, but access tokens are minted by StockX's Auth0 tenant via the OAuth 2.0\n  Authorization Code flow. The authorization request must set audience to\n  gateway.stockx.com. Application-level authorization (catalog/selling/orders) is\n  governed by the developer program grant tied to the API key rather than by\n  granular OAuth scopes; the scopes below are the identity/session scopes the\n  Auth0 authorize endpoint accepts.\nschemes:\n- name: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.stockx.com/authorize\n    tokenUrl: https://accounts.stockx.com/oauth/token\n    audience: gateway.stockx.com\nscopes:\n- scope: openid\n  description: Issue an OpenID Connect ID token for\
  \ the authenticating StockX user.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token so the application can obtain new access tokens without re-prompting the user.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stockx/refs/heads/main/scopes/stockx-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Marketplace
- E-Commerce
- Sneakers
- Streetwear
- Resale
- Collectibles
- Catalog
- Selling
- Orders
token_urls:
- https://accounts.stockx.com/oauth/token
---
