---
authorization_urls:
- /oauth/authorize
- https://cloud.lightspeedapp.com/oauth/authorize.php
- https://secure.retail.lightspeed.app/connect
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lightspeed Pos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightspeed publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightspeed API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightspeed
provider_slug: lightspeed-pos
schemes:
- description: 'The Lightspeed Restaurant K-Series APIs support OAuth2 authentication using the [authorization code grant flow](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/).

    See our [Authorization Quick Start Guide](https://api-portal.lsk.lightspeed.app/quick-start/authentication/authorization-overview) for more details on how to authenticate.'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: OAuth2
  source: openapi/lightspeed-pos-restaurant-k-series-openapi.yml
- description: OAuth 2.0 authorization-code flow with scope-based access control.
  flows:
  - authorizationUrl: https://cloud.lightspeedapp.com/oauth/authorize.php
    flow: authorizationCode
    tokenUrl: https://cloud.lightspeedapp.com/oauth/access_token.php
  name: OAuth2
  source: openapi/lightspeed-pos-retail-r-series-openapi.yml
- description: OAuth 2.0 authorization-code flow with scope-based access.
  flows:
  - authorizationUrl: https://secure.retail.lightspeed.app/connect
    flow: authorizationCode
    tokenUrl: https://{domainPrefix}.retail.lightspeed.app/api/1.0/token
  name: OAuth2
  source: openapi/lightspeed-pos-retail-x-series-openapi.yml
scope_count: 24
scope_names:
- customers.read
- customers.write
- employee:admin
- employee:all
- employee:customers
- employee:customers_read
- employee:inventory
- employee:inventory_read
- employee:register
- employee:reports
- financial-api
- id-cards
- items
- orders-api
- products.read
- products.write
- propertymanagement
- reservation-***
- reservation-platform-code
- reservations-api
- sales.read
- sales.write
- staff-api
- user-token-by-authorization-code
scopes:
- description: Read customers.
  flows:
  - authorizationCode
  scope: customers.read
- description: Create or modify customers.
  flows:
  - authorizationCode
  scope: customers.write
- description: Manage employees and shops.
  flows:
  - authorizationCode
  scope: employee:admin
- description: Full access to all account resources.
  flows:
  - authorizationCode
  scope: employee:all
- description: Create and modify customers.
  flows:
  - authorizationCode
  scope: employee:customers
- description: Read customers.
  flows:
  - authorizationCode
  scope: employee:customers_read
- description: Create and modify inventory items.
  flows:
  - authorizationCode
  scope: employee:inventory
- description: Read inventory items and catalog.
  flows:
  - authorizationCode
  scope: employee:inventory_read
- description: Create sales at the register.
  flows:
  - authorizationCode
  scope: employee:register
- description: Read sales and reporting data.
  flows:
  - authorizationCode
  scope: employee:reports
- description: Read financial data
  flows:
  - authorizationCode
  scope: financial-api
- description: Create and manage ID card batches and cards.
  flows:
  - authorizationCode
  scope: id-cards
- description: Read and write items
  flows:
  - authorizationCode
  scope: items
- description: Read business information, floors, menus, discounts, and production instructions. Read and write orders and payments. Read [Rich Item](https://api-docs.lsk.lightspeed.app/prod/group/endpoint-rich-item) data.
  flows:
  - authorizationCode
  scope: orders-api
- description: Read products, brands, and inventory.
  flows:
  - authorizationCode
  scope: products.read
- description: Create or modify products, brands, and inventory.
  flows:
  - authorizationCode
  scope: products.write
- description: Read and write Property Management System configurations.
  flows:
  - authorizationCode
  scope: propertymanagement
- description: Platform reservations scope. The `***` will be replaced by the [platform-code](https://api-docs.lsk.lightspeed.app/operation/operation-reservation-servicesetbyplatformcode#operation-reservation-servicesetbyplatformcode-platform-code) of the reservation platform.
  flows:
  - authorizationCode
  scope: reservation-***
- description: ''
  flows: []
  scope: reservation-platform-code
- description: Configure *legacy* reservation integrations. **Note:** This API will eventually be deprecated in favour of the new [Reservations for Platforms](https://api-docs.lsk.lightspeed.app/group/endpoint-reservations-for-platforms) API. More information on the new reservations workflows can be found in the [Integration Guide](https://api-portal.lsk.lightspeed.app/category/reservations).
  flows:
  - authorizationCode
  scope: reservations-api
- description: Read sales transactions.
  flows:
  - authorizationCode
  scope: sales.read
- description: Create or modify sales.
  flows:
  - authorizationCode
  scope: sales.write
- description: Read shift information, read and write user information.
  flows:
  - authorizationCode
  scope: staff-api
- description: ''
  flows: []
  scope: user-token-by-authorization-code
slug: lightspeed-pos-scopes
source_filename: lightspeed-pos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightspeed-pos-restaurant-k-series-openapi.yml, openapi/lightspeed-pos-retail-r-series-openapi.yml,\n  openapi/lightspeed-pos-retail-x-series-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  description: |-\n    The Lightspeed Restaurant K-Series APIs support OAuth2 authentication using the [authorization code grant flow](https://www.oauth.com/oauth2-servers/server-side-apps/authorization-code/).\n    See our [Authorization Quick Start Guide](https://api-portal.lsk.lightspeed.app/quick-start/authentication/authorization-overview) for more details on how to authenticate.\n- name: OAuth2\n  source: openapi/lightspeed-pos-retail-r-series-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cloud.lightspeedapp.com/oauth/authorize.php\n\
  \    tokenUrl: https://cloud.lightspeedapp.com/oauth/access_token.php\n  description: OAuth 2.0 authorization-code flow with scope-based access control.\n- name: OAuth2\n  source: openapi/lightspeed-pos-retail-x-series-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.retail.lightspeed.app/connect\n    tokenUrl: https://{domainPrefix}.retail.lightspeed.app/api/1.0/token\n  description: OAuth 2.0 authorization-code flow with scope-based access.\nscopes:\n- scope: customers.read\n  description: Read customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: customers.write\n  description: Create or modify customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: employee:admin\n  description: Manage employees and shops.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope:\
  \ employee:all\n  description: Full access to all account resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:customers\n  description: Create and modify customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:customers_read\n  description: Read customers.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:inventory\n  description: Create and modify inventory items.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:inventory_read\n  description: Read inventory items and catalog.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:register\n  description: Create sales at the register.\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: employee:reports\n  description: Read sales and reporting data.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-r-series-openapi.yml\n- scope: financial-api\n  description: Read financial data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: id-cards\n  description: Create and manage ID card batches and cards.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: items\n  description: Read and write items\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: orders-api\n  description: |-\n    Read business information, floors, menus, discounts, and production instructions.\n    Read and write orders and payments. Read [Rich Item](https://api-docs.lsk.lightspeed.app/prod/group/endpoint-rich-item) data.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: products.read\n  description: Read products, brands, and inventory.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: products.write\n  description: Create or modify products, brands, and inventory.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: propertymanagement\n  description: Read and write Property Management System configurations.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: reservation-***\n  description: Platform reservations scope. The `***` will be replaced by the [platform-code](https://api-docs.lsk.lightspeed.app/operation/operation-reservation-servicesetbyplatformcode#operation-reservation-servicesetbyplatformcode-platform-code)\n    of the reservation platform.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: reservation-platform-code\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: reservations-api\n  description: |-\n    Configure *legacy* reservation integrations.\n    **Note:** This API will eventually be deprecated in favour of the new [Reservations for Platforms](https://api-docs.lsk.lightspeed.app/group/endpoint-reservations-for-platforms) API.\n    More information on the new reservations workflows can be found in the [Integration Guide](https://api-portal.lsk.lightspeed.app/category/reservations).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: sales.read\n  description: Read sales transactions.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: sales.write\n  description: Create or modify sales.\n  flows:\n  - authorizationCode\n  sources:\n \
  \ - openapi/lightspeed-pos-retail-x-series-openapi.yml\n- scope: staff-api\n  description: Read shift information, read and write user information.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n- scope: user-token-by-authorization-code\n  sources:\n  - openapi/lightspeed-pos-restaurant-k-series-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightspeed-pos/refs/heads/main/scopes/lightspeed-pos-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- POS
- Retail
- Restaurant
- Ecommerce
token_urls:
- /oauth/token
- https://cloud.lightspeedapp.com/oauth/access_token.php
- https://{domainPrefix}.retail.lightspeed.app/api/1.0/token
---
