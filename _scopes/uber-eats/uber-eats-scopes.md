---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Uber Eats Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Uber Eats publishes 8 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Uber Eats API on a user''s behalf.


  Tokens are issued from https://auth.uber.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Uber Eats
provider_slug: uber-eats
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.uber.com/oauth/v2/token
  name: oauth2
  source: openapi/uber-direct-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.uber.com/oauth/v2/token
  name: oauth2
  source: openapi/uber-eats-openapi.yml
scope_count: 8
scope_names:
- eats.deliveries
- eats.menu
- eats.menu.read
- eats.menu.write
- eats.order
- eats.store
- eats.store.orders.read
- eats.store.status.write
scopes:
- description: Create and manage Uber Direct deliveries
  flows:
  - clientCredentials
  scope: eats.deliveries
- description: Manage menus
  flows:
  - clientCredentials
  scope: eats.menu
- description: Read menus
  flows:
  - clientCredentials
  scope: eats.menu.read
- description: Write menus
  flows:
  - clientCredentials
  scope: eats.menu.write
- description: Manage orders
  flows:
  - clientCredentials
  scope: eats.order
- description: Access to store operations
  flows:
  - clientCredentials
  scope: eats.store
- description: Read store orders
  flows:
  - clientCredentials
  scope: eats.store.orders.read
- description: Update store status
  flows:
  - clientCredentials
  scope: eats.store.status.write
slug: uber-eats-scopes
source_filename: uber-eats-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uber-direct-openapi.yml, openapi/uber-eats-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/uber-direct-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.uber.com/oauth/v2/token\n- name: oauth2\n  source: openapi/uber-eats-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.uber.com/oauth/v2/token\nscopes:\n- scope: eats.deliveries\n  description: Create and manage Uber Direct deliveries\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-direct-openapi.yml\n- scope: eats.menu\n  description: Manage menus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n- scope: eats.menu.read\n  description: Read menus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n- scope: eats.menu.write\n  description: Write menus\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n\
  - scope: eats.order\n  description: Manage orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n- scope: eats.store\n  description: Access to store operations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n- scope: eats.store.orders.read\n  description: Read store orders\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n- scope: eats.store.status.write\n  description: Update store status\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/uber-eats-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uber-eats/refs/heads/main/scopes/uber-eats-scopes.yml
summary_line: 8 scopes · clientCredentials
tags:
- Uber Eats
- Uber Direct
- Food Delivery
- Last-Mile Logistics
- Restaurants
- Menus
- Orders
- Fulfillment
- Courier
- OAuth2
token_urls:
- https://auth.uber.com/oauth/v2/token
---
