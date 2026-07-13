---
api_specs:
- filename: etsy-openapi-original.yml
  format: yaml
  label: Etsy Open API v3
  slug: open-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/openapi/etsy-openapi-original.yml
- filename: etsy-webhooks-asyncapi.yml
  format: yaml
  label: Etsy Open API v3 Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/asyncapi/etsy-webhooks-asyncapi.yml
authorization_urls:
- https://www.etsy.com/oauth/connect
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Etsy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Etsy publishes 20 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Etsy API on a user''s behalf.


  Tokens are issued from https://openapi.etsy.com/v3/public/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Etsy
provider_slug: etsy
schemes:
- description: Open API v3 supports authenticating via OAuth 2.0. More information about Etsy's specific implementation of OAuth2 can be found [here](/documentation/essentials/oauth2).
  flows:
  - authorizationUrl: https://www.etsy.com/oauth/connect
    flow: authorizationCode
    tokenUrl: https://openapi.etsy.com/v3/public/oauth/token
  name: oauth2
  source: openapi/etsy-openapi-original.yml
scope_count: 20
scope_names:
- address_r
- address_w
- billing_r
- cart_r
- cart_w
- email_r
- favorites_r
- favorites_w
- feedback_r
- listings_d
- listings_r
- listings_w
- profile_r
- profile_w
- recommend_r
- recommend_w
- shops_r
- shops_w
- transactions_r
- transactions_w
scopes:
- description: see billing and shipping addresses
  flows:
  - authorizationCode
  scope: address_r
- description: update billing and shipping addresses
  flows:
  - authorizationCode
  scope: address_w
- description: see all billing statement data
  flows:
  - authorizationCode
  scope: billing_r
- description: read shopping carts
  flows:
  - authorizationCode
  scope: cart_r
- description: add/remove from shopping carts
  flows:
  - authorizationCode
  scope: cart_w
- description: read a user profile
  flows:
  - authorizationCode
  scope: email_r
- description: see private favorites
  flows:
  - authorizationCode
  scope: favorites_r
- description: add/remove favorites
  flows:
  - authorizationCode
  scope: favorites_w
- description: see purchase info in feedback
  flows:
  - authorizationCode
  scope: feedback_r
- description: delete listings
  flows:
  - authorizationCode
  scope: listings_d
- description: see all listings (including expired etc)
  flows:
  - authorizationCode
  scope: listings_r
- description: create/edit listings
  flows:
  - authorizationCode
  scope: listings_w
- description: see all profile data
  flows:
  - authorizationCode
  scope: profile_r
- description: update user profile, avatar, etc
  flows:
  - authorizationCode
  scope: profile_w
- description: see recommended listings
  flows:
  - authorizationCode
  scope: recommend_r
- description: accept/reject recommended listings
  flows:
  - authorizationCode
  scope: recommend_w
- description: see private shop info
  flows:
  - authorizationCode
  scope: shops_r
- description: update shop
  flows:
  - authorizationCode
  scope: shops_w
- description: see all checkout/payment data
  flows:
  - authorizationCode
  scope: transactions_r
- description: update receipts
  flows:
  - authorizationCode
  scope: transactions_w
slug: etsy-scopes
source_filename: etsy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/etsy-openapi-original.yml\nschemes:\n- name: oauth2\n  source: openapi/etsy-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.etsy.com/oauth/connect\n    tokenUrl: https://openapi.etsy.com/v3/public/oauth/token\n  description: Open API v3 supports authenticating via OAuth 2.0. More information about Etsy's\n    specific implementation of OAuth2 can be found [here](/documentation/essentials/oauth2).\nscopes:\n- scope: address_r\n  description: see billing and shipping addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: address_w\n  description: update billing and shipping addresses\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: billing_r\n  description: see all billing statement data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope:\
  \ cart_r\n  description: read shopping carts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: cart_w\n  description: add/remove from shopping carts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: email_r\n  description: read a user profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: favorites_r\n  description: see private favorites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: favorites_w\n  description: add/remove favorites\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: feedback_r\n  description: see purchase info in feedback\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: listings_d\n  description: delete listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope:\
  \ listings_r\n  description: see all listings (including expired etc)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: listings_w\n  description: create/edit listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: profile_r\n  description: see all profile data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: profile_w\n  description: update user profile, avatar, etc\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: recommend_r\n  description: see recommended listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: recommend_w\n  description: accept/reject recommended listings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: shops_r\n  description: see private shop info\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/etsy-openapi-original.yml\n- scope: shops_w\n  description: update shop\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: transactions_r\n  description: see all checkout/payment data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n- scope: transactions_w\n  description: update receipts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/etsy-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etsy/refs/heads/main/scopes/etsy-scopes.yml
summary_line: 20 scopes · authorizationCode
tags:
- Marketplace
- Ecommerce
- Handmade
- Listings
- Orders
- Payments
- Reviews
- Shipping
- Taxonomy
- OAuth2
token_urls:
- https://openapi.etsy.com/v3/public/oauth/token
---
