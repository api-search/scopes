---
api_specs:
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Products API
  slug: fourthwall-storefront-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Collections API
  slug: fourthwall-storefront-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Storefront Cart & Checkout API
  slug: fourthwall-storefront-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Orders API
  slug: fourthwall-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Products API
  slug: fourthwall-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Gifting & Giveaways API
  slug: fourthwall-gifting-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Promotions API
  slug: fourthwall-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Memberships API
  slug: fourthwall-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
- filename: fourthwall-openapi.yml
  format: yaml
  label: Fourthwall Webhooks API
  slug: fourthwall-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-openapi.yml
authorization_urls:
- https://auth.fourthwall.com/auth/realms/Fourthwall/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fourthwall Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fourthwall publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fourthwall API on a user''s behalf.


  Tokens are issued from https://api.fourthwall.com/open-api/v1.0/platform/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fourthwall
provider_slug: fourthwall
schemes:
- description: OAuth 2.0 for multi-shop platform apps.
  flows:
  - authorizationUrl: https://auth.fourthwall.com/auth/realms/Fourthwall/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://api.fourthwall.com/open-api/v1.0/platform/token
  name: oauth
  source: openapi/fourthwall-openapi.yml
scope_count: 14
scope_names:
- donation_read
- giveaway_read
- giveaway_write
- memberships_read
- memberships_write
- offer_read
- offer_write
- order_read
- order_write
- promotions_read
- promotions_write
- shop_read
- webhook_read
- webhook_write
scopes:
- description: Read donations
  flows:
  - authorizationCode
  scope: donation_read
- description: Read giveaways
  flows:
  - authorizationCode
  scope: giveaway_read
- description: Write giveaways
  flows:
  - authorizationCode
  scope: giveaway_write
- description: Read memberships
  flows:
  - authorizationCode
  scope: memberships_read
- description: Write memberships
  flows:
  - authorizationCode
  scope: memberships_write
- description: Read products, collections, and gifting
  flows:
  - authorizationCode
  scope: offer_read
- description: Write products, collections, and gifting
  flows:
  - authorizationCode
  scope: offer_write
- description: Read orders
  flows:
  - authorizationCode
  scope: order_read
- description: Write orders and fulfillments
  flows:
  - authorizationCode
  scope: order_write
- description: Read promotions
  flows:
  - authorizationCode
  scope: promotions_read
- description: Write promotions
  flows:
  - authorizationCode
  scope: promotions_write
- description: Read shop information
  flows:
  - authorizationCode
  scope: shop_read
- description: Read webhooks
  flows:
  - authorizationCode
  scope: webhook_read
- description: Write webhooks
  flows:
  - authorizationCode
  scope: webhook_write
slug: fourthwall-scopes
source_filename: fourthwall-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fourthwall-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/fourthwall-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.fourthwall.com/auth/realms/Fourthwall/protocol/openid-connect/auth\n    tokenUrl: https://api.fourthwall.com/open-api/v1.0/platform/token\n  description: OAuth 2.0 for multi-shop platform apps.\nscopes:\n- scope: donation_read\n  description: Read donations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: giveaway_read\n  description: Read giveaways\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: giveaway_write\n  description: Write giveaways\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: memberships_read\n  description: Read memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: memberships_write\n\
  \  description: Write memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: offer_read\n  description: Read products, collections, and gifting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: offer_write\n  description: Write products, collections, and gifting\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: order_read\n  description: Read orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: order_write\n  description: Write orders and fulfillments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: promotions_read\n  description: Read promotions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: promotions_write\n  description: Write promotions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope:\
  \ shop_read\n  description: Read shop information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: webhook_read\n  description: Read webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n- scope: webhook_write\n  description: Write webhooks\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fourthwall-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/scopes/fourthwall-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Creator Commerce
- Ecommerce
- Merch
- Storefront
- Memberships
- Donations
- Print on Demand
token_urls:
- https://api.fourthwall.com/open-api/v1.0/platform/token
---
