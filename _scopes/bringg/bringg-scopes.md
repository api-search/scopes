---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bringg Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bringg publishes 25 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bringg API on a user''s behalf.


  Tokens are issued from https://admin-api.bringg.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bringg
provider_slug: bringg
schemes:
- description: 'OAuth 2.0 Client Credentials Grant. Exchange your client_id and client_secret

    for an access token via POST https://admin-api.bringg.com/oauth/token (or the

    regional equivalent), then send Authorization: Bearer <access_token>.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://admin-api.bringg.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/bringg-delivery-hub-api-openapi.yml
- description: OAuth 2.0 Client Credentials Grant.
  flows:
  - flow: clientCredentials
    tokenUrl: https://admin-api.bringg.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/bringg-drivers-shifts-api-openapi.yml
- description: OAuth 2.0 Client Credentials Grant. Webhook callbacks are signed with a shared secret.
  flows:
  - flow: clientCredentials
    tokenUrl: https://admin-api.bringg.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/bringg-fleet-partners-api-openapi.yml
scope_count: 25
scope_names:
- assign_task
- cancel_order
- cancel_task
- checkin
- checkout
- complete_order
- create_customer
- create_delivery_block
- create_service_area
- create_service_plan
- create_task
- create_team
- create_user
- create_vehicle
- delete_user
- end_shift
- get_quotes
- get_task
- get_user
- request_driver
- start_shift
- update_customer
- update_driver_location
- update_task
- update_user
scopes:
- description: Assign orders to drivers
  flows:
  - clientCredentials
  scope: assign_task
- description: Cancel orders
  flows:
  - clientCredentials
  scope: cancel_order
- description: Cancel orders
  flows:
  - clientCredentials
  scope: cancel_task
- description: Driver check-in
  flows:
  - clientCredentials
  scope: checkin
- description: Driver check-out
  flows:
  - clientCredentials
  scope: checkout
- description: Complete orders
  flows:
  - clientCredentials
  scope: complete_order
- description: Create customers
  flows:
  - clientCredentials
  scope: create_customer
- description: Create delivery blocks
  flows:
  - clientCredentials
  scope: create_delivery_block
- description: Create service areas
  flows:
  - clientCredentials
  scope: create_service_area
- description: Create service plans
  flows:
  - clientCredentials
  scope: create_service_plan
- description: Create orders
  flows:
  - clientCredentials
  scope: create_task
- description: Create teams
  flows:
  - clientCredentials
  scope: create_team
- description: Create users
  flows:
  - clientCredentials
  scope: create_user
- description: Create vehicles
  flows:
  - clientCredentials
  scope: create_vehicle
- description: Delete users
  flows:
  - clientCredentials
  scope: delete_user
- description: End shifts
  flows:
  - clientCredentials
  scope: end_shift
- description: Get delivery quotes
  flows:
  - clientCredentials
  scope: get_quotes
- description: Read orders
  flows:
  - clientCredentials
  scope: get_task
- description: Read users
  flows:
  - clientCredentials
  scope: get_user
- description: Request driver fulfillment
  flows:
  - clientCredentials
  scope: request_driver
- description: Start shifts
  flows:
  - clientCredentials
  scope: start_shift
- description: Update customers
  flows:
  - clientCredentials
  scope: update_customer
- description: Update driver location
  flows:
  - clientCredentials
  scope: update_driver_location
- description: Update orders
  flows:
  - clientCredentials
  scope: update_task
- description: Update users
  flows:
  - clientCredentials
  scope: update_user
slug: bringg-scopes
source_filename: bringg-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bringg-delivery-hub-api-openapi.yml, openapi/bringg-drivers-shifts-api-openapi.yml,\n  openapi/bringg-fleet-partners-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/bringg-delivery-hub-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://admin-api.bringg.com/oauth/token\n  description: |-\n    OAuth 2.0 Client Credentials Grant. Exchange your client_id and client_secret\n    for an access token via POST https://admin-api.bringg.com/oauth/token (or the\n    regional equivalent), then send Authorization: Bearer <access_token>.\n- name: OAuth2ClientCredentials\n  source: openapi/bringg-drivers-shifts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://admin-api.bringg.com/oauth/token\n  description: OAuth 2.0 Client Credentials Grant.\n- name: OAuth2ClientCredentials\n  source: openapi/bringg-fleet-partners-api-openapi.yml\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://admin-api.bringg.com/oauth/token\n  description: OAuth 2.0 Client Credentials Grant. Webhook callbacks are signed with a shared\n    secret.\nscopes:\n- scope: assign_task\n  description: Assign orders to drivers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: cancel_order\n  description: Cancel orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-fleet-partners-api-openapi.yml\n- scope: cancel_task\n  description: Cancel orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: checkin\n  description: Driver check-in\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: checkout\n  description: Driver check-out\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: complete_order\n  description: Complete orders\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/bringg-fleet-partners-api-openapi.yml\n- scope: create_customer\n  description: Create customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: create_delivery_block\n  description: Create delivery blocks\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: create_service_area\n  description: Create service areas\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: create_service_plan\n  description: Create service plans\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: create_task\n  description: Create orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: create_team\n  description: Create teams\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n\
  - scope: create_user\n  description: Create users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: create_vehicle\n  description: Create vehicles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: delete_user\n  description: Delete users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: end_shift\n  description: End shifts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: get_quotes\n  description: Get delivery quotes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: get_task\n  description: Read orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: get_user\n  description: Read users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n\
  - scope: request_driver\n  description: Request driver fulfillment\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-fleet-partners-api-openapi.yml\n- scope: start_shift\n  description: Start shifts\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n- scope: update_customer\n  description: Update customers\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: update_driver_location\n  description: Update driver location\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n  - openapi/bringg-fleet-partners-api-openapi.yml\n- scope: update_task\n  description: Update orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-delivery-hub-api-openapi.yml\n- scope: update_user\n  description: Update users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bringg-drivers-shifts-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bringg/refs/heads/main/scopes/bringg-scopes.yml
summary_line: 25 scopes · clientCredentials
tags:
- Last-Mile Delivery
- Delivery Orchestration
- Fulfillment
- Logistics
- Retail
- Dispatch
- Routing
- Driver App
- Carrier Network
- Fleet Management
- Supply Chain
- E-commerce
- Same-Day Delivery
- Curbside Pickup
- Returns
token_urls:
- https://admin-api.bringg.com/oauth/token
---
