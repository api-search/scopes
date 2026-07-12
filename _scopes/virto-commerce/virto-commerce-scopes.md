---
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Virto Commerce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Virto Commerce publishes 72 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virto Commerce API on a user''s behalf.


  Tokens are issued from /connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virto Commerce
provider_slug: virto-commerce
schemes:
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-cart-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-catalog-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-customer-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-inventory-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-marketing-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-orders-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-platform-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-pricing-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-quote-openapi.json
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-store-openapi.json
scope_count: 72
scope_names:
- background_jobs:manage
- cache:reset
- cart:create
- cart:delete
- cart:read
- cart:update
- catalog:access
- catalog:configurations:read
- catalog:configurations:update
- catalog:create
- catalog:delete
- catalog:dictionary-property:edit
- catalog:read
- catalog:update
- customer:create
- customer:delete
- customer:invite
- customer:read
- customer:update
- inventory:fulfillment:delete
- inventory:fulfillment:edit
- inventory:fulfillment:read
- inventory:read
- inventory:update
- marketing:create
- marketing:delete
- marketing:read
- marketing:update
- measures:access
- measures:create
- measures:delete
- measures:read
- measures:update
- order:capture_payment
- order:create
- order:dashboardstatistics:view
- order:payment:execute_callback
- order:refund
- order:update_shipments
- platform:developer-tools:access
- platform:dynamic_properties:create
- platform:dynamic_properties:delete
- platform:dynamic_properties:read
- platform:dynamic_properties:update
- platform:module:manage
- platform:module:read
- platform:security:confirmEmail
- platform:security:create
- platform:security:delete
- platform:security:generateToken
- platform:security:oauth_applications:create
- platform:security:oauth_applications:delete
- platform:security:oauth_applications:read
- platform:security:oauth_applications:update
- platform:security:read
- platform:security:revokeToken
- platform:security:update
- platform:security:verifyEmail
- platform:security:verifyToken
- platform:setting:read
- platform:setting:update
- pricing:create
- pricing:delete
- pricing:read
- pricing:update
- quote:create
- quote:delete
- quote:read
- quote:update
- store:create
- store:read
- store:update
scopes:
- description: ''
  flows: []
  scope: background_jobs:manage
- description: ''
  flows: []
  scope: cache:reset
- description: ''
  flows: []
  scope: cart:create
- description: ''
  flows: []
  scope: cart:delete
- description: ''
  flows: []
  scope: cart:read
- description: ''
  flows: []
  scope: cart:update
- description: ''
  flows: []
  scope: catalog:access
- description: ''
  flows: []
  scope: catalog:configurations:read
- description: ''
  flows: []
  scope: catalog:configurations:update
- description: ''
  flows: []
  scope: catalog:create
- description: ''
  flows: []
  scope: catalog:delete
- description: ''
  flows: []
  scope: catalog:dictionary-property:edit
- description: ''
  flows: []
  scope: catalog:read
- description: ''
  flows: []
  scope: catalog:update
- description: ''
  flows: []
  scope: customer:create
- description: ''
  flows: []
  scope: customer:delete
- description: ''
  flows: []
  scope: customer:invite
- description: ''
  flows: []
  scope: customer:read
- description: ''
  flows: []
  scope: customer:update
- description: ''
  flows: []
  scope: inventory:fulfillment:delete
- description: ''
  flows: []
  scope: inventory:fulfillment:edit
- description: ''
  flows: []
  scope: inventory:fulfillment:read
- description: ''
  flows: []
  scope: inventory:read
- description: ''
  flows: []
  scope: inventory:update
- description: ''
  flows: []
  scope: marketing:create
- description: ''
  flows: []
  scope: marketing:delete
- description: ''
  flows: []
  scope: marketing:read
- description: ''
  flows: []
  scope: marketing:update
- description: ''
  flows: []
  scope: measures:access
- description: ''
  flows: []
  scope: measures:create
- description: ''
  flows: []
  scope: measures:delete
- description: ''
  flows: []
  scope: measures:read
- description: ''
  flows: []
  scope: measures:update
- description: ''
  flows: []
  scope: order:capture_payment
- description: ''
  flows: []
  scope: order:create
- description: ''
  flows: []
  scope: order:dashboardstatistics:view
- description: ''
  flows: []
  scope: order:payment:execute_callback
- description: ''
  flows: []
  scope: order:refund
- description: ''
  flows: []
  scope: order:update_shipments
- description: ''
  flows: []
  scope: platform:developer-tools:access
- description: ''
  flows: []
  scope: platform:dynamic_properties:create
- description: ''
  flows: []
  scope: platform:dynamic_properties:delete
- description: ''
  flows: []
  scope: platform:dynamic_properties:read
- description: ''
  flows: []
  scope: platform:dynamic_properties:update
- description: ''
  flows: []
  scope: platform:module:manage
- description: ''
  flows: []
  scope: platform:module:read
- description: ''
  flows: []
  scope: platform:security:confirmEmail
- description: ''
  flows: []
  scope: platform:security:create
- description: ''
  flows: []
  scope: platform:security:delete
- description: ''
  flows: []
  scope: platform:security:generateToken
- description: ''
  flows: []
  scope: platform:security:oauth_applications:create
- description: ''
  flows: []
  scope: platform:security:oauth_applications:delete
- description: ''
  flows: []
  scope: platform:security:oauth_applications:read
- description: ''
  flows: []
  scope: platform:security:oauth_applications:update
- description: ''
  flows: []
  scope: platform:security:read
- description: ''
  flows: []
  scope: platform:security:revokeToken
- description: ''
  flows: []
  scope: platform:security:update
- description: ''
  flows: []
  scope: platform:security:verifyEmail
- description: ''
  flows: []
  scope: platform:security:verifyToken
- description: ''
  flows: []
  scope: platform:setting:read
- description: ''
  flows: []
  scope: platform:setting:update
- description: ''
  flows: []
  scope: pricing:create
- description: ''
  flows: []
  scope: pricing:delete
- description: ''
  flows: []
  scope: pricing:read
- description: ''
  flows: []
  scope: pricing:update
- description: ''
  flows: []
  scope: quote:create
- description: ''
  flows: []
  scope: quote:delete
- description: ''
  flows: []
  scope: quote:read
- description: ''
  flows: []
  scope: quote:update
- description: ''
  flows: []
  scope: store:create
- description: ''
  flows: []
  scope: store:read
- description: ''
  flows: []
  scope: store:update
slug: virto-commerce-scopes
source_filename: virto-commerce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/virto-commerce-cart-openapi.json, openapi/virto-commerce-catalog-openapi.json,\n  openapi/virto-commerce-customer-openapi.json, openapi/virto-commerce-inventory-openapi.json,\n  openapi/virto-commerce-marketing-openapi.json, openapi/virto-commerce-orders-openapi.json,\n  openapi/virto-commerce-platform-openapi.json, openapi/virto-commerce-pricing-openapi.json,\n  openapi/virto-commerce-quote-openapi.json, openapi/virto-commerce-store-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/virto-commerce-cart-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-catalog-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner\
  \ Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-customer-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-inventory-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-marketing-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-orders-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password\
  \ Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-platform-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-pricing-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-quote-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-store-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n\
  scopes:\n- scope: background_jobs:manage\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: cache:reset\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: cart:create\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n- scope: cart:delete\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n- scope: cart:read\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n- scope: cart:update\n  sources:\n  - openapi/virto-commerce-cart-openapi.json\n- scope: catalog:access\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:configurations:read\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:configurations:update\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:create\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:delete\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:dictionary-property:edit\n\
  \  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:read\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: catalog:update\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: customer:create\n  sources:\n  - openapi/virto-commerce-customer-openapi.json\n- scope: customer:delete\n  sources:\n  - openapi/virto-commerce-customer-openapi.json\n- scope: customer:invite\n  sources:\n  - openapi/virto-commerce-customer-openapi.json\n- scope: customer:read\n  sources:\n  - openapi/virto-commerce-customer-openapi.json\n- scope: customer:update\n  sources:\n  - openapi/virto-commerce-customer-openapi.json\n- scope: inventory:fulfillment:delete\n  sources:\n  - openapi/virto-commerce-inventory-openapi.json\n- scope: inventory:fulfillment:edit\n  sources:\n  - openapi/virto-commerce-inventory-openapi.json\n- scope: inventory:fulfillment:read\n  sources:\n  - openapi/virto-commerce-inventory-openapi.json\n- scope: inventory:read\n  sources:\n\
  \  - openapi/virto-commerce-inventory-openapi.json\n- scope: inventory:update\n  sources:\n  - openapi/virto-commerce-inventory-openapi.json\n- scope: marketing:create\n  sources:\n  - openapi/virto-commerce-marketing-openapi.json\n- scope: marketing:delete\n  sources:\n  - openapi/virto-commerce-marketing-openapi.json\n- scope: marketing:read\n  sources:\n  - openapi/virto-commerce-marketing-openapi.json\n- scope: marketing:update\n  sources:\n  - openapi/virto-commerce-marketing-openapi.json\n- scope: measures:access\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: measures:create\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: measures:delete\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: measures:read\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: measures:update\n  sources:\n  - openapi/virto-commerce-catalog-openapi.json\n- scope: order:capture_payment\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n\
  - scope: order:create\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n  - openapi/virto-commerce-quote-openapi.json\n- scope: order:dashboardstatistics:view\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n- scope: order:payment:execute_callback\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n- scope: order:refund\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n- scope: order:update_shipments\n  sources:\n  - openapi/virto-commerce-orders-openapi.json\n- scope: platform:developer-tools:access\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:dynamic_properties:create\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:dynamic_properties:delete\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:dynamic_properties:read\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:dynamic_properties:update\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n\
  - scope: platform:module:manage\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:module:read\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:confirmEmail\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:create\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:delete\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:generateToken\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:oauth_applications:create\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:oauth_applications:delete\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:oauth_applications:read\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:oauth_applications:update\n  sources:\n\
  \  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:read\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:revokeToken\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:update\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:verifyEmail\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:security:verifyToken\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:setting:read\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: platform:setting:update\n  sources:\n  - openapi/virto-commerce-platform-openapi.json\n- scope: pricing:create\n  sources:\n  - openapi/virto-commerce-pricing-openapi.json\n- scope: pricing:delete\n  sources:\n  - openapi/virto-commerce-pricing-openapi.json\n- scope: pricing:read\n  sources:\n  - openapi/virto-commerce-pricing-openapi.json\n- scope:\
  \ pricing:update\n  sources:\n  - openapi/virto-commerce-pricing-openapi.json\n- scope: quote:create\n  sources:\n  - openapi/virto-commerce-quote-openapi.json\n- scope: quote:delete\n  sources:\n  - openapi/virto-commerce-quote-openapi.json\n- scope: quote:read\n  sources:\n  - openapi/virto-commerce-quote-openapi.json\n- scope: quote:update\n  sources:\n  - openapi/virto-commerce-quote-openapi.json\n- scope: store:create\n  sources:\n  - openapi/virto-commerce-store-openapi.json\n- scope: store:read\n  sources:\n  - openapi/virto-commerce-store-openapi.json\n- scope: store:update\n  sources:\n  - openapi/virto-commerce-store-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/scopes/virto-commerce-scopes.yml
summary_line: 72 scopes · password/clientCredentials
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscriptions
- Headless Commerce
- Open Source
- .NET
token_urls:
- /connect/token
---
