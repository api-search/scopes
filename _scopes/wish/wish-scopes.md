---
api_specs:
- filename: wish-marketplace-v3-openapi.json
  format: json
  label: Wish Marketplace V3 API
  slug: wish-marketplace-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/openapi/wish-marketplace-v3-openapi.json
authorization_urls:
- https://merchant.wish.com/v3/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wish Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wish publishes 39 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wish API on a user''s behalf.


  Tokens are issued from https://merchant.wish.com/api/v3/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wish
provider_slug: wish
schemes:
- flows:
  - authorizationUrl: https://merchant.wish.com/v3/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://merchant.wish.com/api/v3/oauth/access_token
  name: OAuth2
  source: openapi/wish-marketplace-v3-openapi.json
scope_count: 39
scope_names:
- announcements:read
- compliance:read
- compliance:write
- epc:read
- epc:write
- fbs:read
- fbw:read
- fbw:write
- infractions:read
- infractions:write
- listing_quality:read
- merchant:read
- merchant:write
- notifications:read
- notifications:write
- orders:read
- orders:write
- payments:read
- payments:write
- penalties:read
- penalties:write
- product_boost:read
- product_boost:write
- products:read
- products:write
- promotions:read
- promotions:write
- qoo10:read
- ratings:read
- returns:read
- returns:write
- tickets:read
- tickets:write
- videos:read
- videos:write
- webhook:read
- webhook:write
- wps_parcel:read
- wps_parcel:write
scopes:
- description: Read announcements
  flows:
  - authorizationCode
  scope: announcements:read
- description: Read Compliance
  flows:
  - authorizationCode
  scope: compliance:read
- description: Write Compliance
  flows:
  - authorizationCode
  scope: compliance:write
- description: read EPC info
  flows:
  - authorizationCode
  scope: epc:read
- description: write EPC info
  flows:
  - authorizationCode
  scope: epc:write
- description: Read FBS
  flows:
  - authorizationCode
  scope: fbs:read
- description: Read FBW
  flows:
  - authorizationCode
  scope: fbw:read
- description: Write FBW
  flows:
  - authorizationCode
  scope: fbw:write
- description: Read infractions
  flows:
  - authorizationCode
  scope: infractions:read
- description: Write infractions
  flows:
  - authorizationCode
  scope: infractions:write
- description: Read listing quality
  flows:
  - authorizationCode
  scope: listing_quality:read
- description: Read merchant
  flows:
  - authorizationCode
  scope: merchant:read
- description: Write merchant
  flows:
  - authorizationCode
  scope: merchant:write
- description: Read notifications
  flows:
  - authorizationCode
  scope: notifications:read
- description: Write notifications
  flows:
  - authorizationCode
  scope: notifications:write
- description: Read orders
  flows:
  - authorizationCode
  scope: orders:read
- description: Update orders
  flows:
  - authorizationCode
  scope: orders:write
- description: Read payments
  flows:
  - authorizationCode
  scope: payments:read
- description: Update payments
  flows:
  - authorizationCode
  scope: payments:write
- description: Read penalties
  flows:
  - authorizationCode
  scope: penalties:read
- description: Update penalties
  flows:
  - authorizationCode
  scope: penalties:write
- description: Read ProductBoost
  flows:
  - authorizationCode
  scope: product_boost:read
- description: Write ProductBoost
  flows:
  - authorizationCode
  scope: product_boost:write
- description: Read products
  flows:
  - authorizationCode
  scope: products:read
- description: Write products
  flows:
  - authorizationCode
  scope: products:write
- description: ''
  flows: []
  scope: promotions:read
- description: ''
  flows: []
  scope: promotions:write
- description: Read Qoo10
  flows:
  - authorizationCode
  scope: qoo10:read
- description: Read ratings
  flows:
  - authorizationCode
  scope: ratings:read
- description: Read returns
  flows:
  - authorizationCode
  scope: returns:read
- description: Write returns
  flows:
  - authorizationCode
  scope: returns:write
- description: Read customer tickets
  flows:
  - authorizationCode
  scope: tickets:read
- description: Write customer tickets
  flows:
  - authorizationCode
  scope: tickets:write
- description: Read videos
  flows:
  - authorizationCode
  scope: videos:read
- description: Write videos
  flows:
  - authorizationCode
  scope: videos:write
- description: Read webhook
  flows:
  - authorizationCode
  scope: webhook:read
- description: Write webhook
  flows:
  - authorizationCode
  scope: webhook:write
- description: Read WishParcel
  flows:
  - authorizationCode
  scope: wps_parcel:read
- description: Write WishParcel
  flows:
  - authorizationCode
  scope: wps_parcel:write
slug: wish-scopes
source_filename: wish-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wish-marketplace-v3-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/wish-marketplace-v3-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://merchant.wish.com/v3/oauth/authorize\n    tokenUrl: https://merchant.wish.com/api/v3/oauth/access_token\nscopes:\n- scope: announcements:read\n  description: Read announcements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: compliance:read\n  description: Read Compliance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: compliance:write\n  description: Write Compliance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: epc:read\n  description: read EPC info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: epc:write\n  description: write\
  \ EPC info\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: fbs:read\n  description: Read FBS\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: fbw:read\n  description: Read FBW\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: fbw:write\n  description: Write FBW\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: infractions:read\n  description: Read infractions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: infractions:write\n  description: Write infractions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: listing_quality:read\n  description: Read listing quality\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: merchant:read\n  description:\
  \ Read merchant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: merchant:write\n  description: Write merchant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: notifications:read\n  description: Read notifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: notifications:write\n  description: Write notifications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: orders:read\n  description: Read orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: orders:write\n  description: Update orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: payments:read\n  description: Read payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope:\
  \ payments:write\n  description: Update payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: penalties:read\n  description: Read penalties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: penalties:write\n  description: Update penalties\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: product_boost:read\n  description: Read ProductBoost\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: product_boost:write\n  description: Write ProductBoost\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: products:read\n  description: Read products\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: products:write\n  description: Write products\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n\
  - scope: promotions:read\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: promotions:write\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: qoo10:read\n  description: Read Qoo10\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: ratings:read\n  description: Read ratings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: returns:read\n  description: Read returns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: returns:write\n  description: Write returns\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: tickets:read\n  description: Read customer tickets\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: tickets:write\n  description: Write customer tickets\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/wish-marketplace-v3-openapi.json\n- scope: videos:read\n  description: Read videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: videos:write\n  description: Write videos\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: webhook:read\n  description: Read webhook\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: webhook:write\n  description: Write webhook\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: wps_parcel:read\n  description: Read WishParcel\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n- scope: wps_parcel:write\n  description: Write WishParcel\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wish-marketplace-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wish/refs/heads/main/scopes/wish-scopes.yml
summary_line: 39 scopes · authorizationCode
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Merchants
- Orders
- Products
- Fulfillment
- Shopping
- OAuth
token_urls:
- https://merchant.wish.com/api/v3/oauth/access_token
---
