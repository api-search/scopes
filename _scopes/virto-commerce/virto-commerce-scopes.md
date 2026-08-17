---
api_specs:
- filename: virto-commerce-catalog-api-openapi.yml
  format: yaml
  label: Virto Commerce Catalog API
  slug: virto-commerce-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-catalog-api-openapi.yml
- filename: virto-commerce-companies-and-contacts-api-openapi.yml
  format: yaml
  label: Virto Commerce Companies and Contacts API
  slug: virto-commerce-companies-and-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-companies-and-contacts-api-openapi.yml
- filename: virto-commerce-inventory-api-openapi.yml
  format: yaml
  label: Virto Commerce Inventory API
  slug: virto-commerce-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-inventory-api-openapi.yml
- filename: virto-commerce-marketing-api-openapi.yml
  format: yaml
  label: Virto Commerce Marketing API
  slug: virto-commerce-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-marketing-api-openapi.yml
- filename: virto-commerce-order-management-api-openapi.yml
  format: yaml
  label: Virto Commerce Order Management API
  slug: virto-commerce-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-order-management-api-openapi.yml
- filename: virto-commerce-pricing-api-openapi.yml
  format: yaml
  label: Virto Commerce Pricing API
  slug: virto-commerce-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-pricing-api-openapi.yml
- filename: virto-commerce-quotes-api-openapi.yml
  format: yaml
  label: Virto Commerce Quotes API
  slug: virto-commerce-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-quotes-api-openapi.yml
- filename: virto-commerce-shopping-cart-api-openapi.yml
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: virto-commerce-shopping-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-shopping-cart-api-openapi.yml
- filename: virto-commerce-store-api-openapi.yml
  format: yaml
  label: Virto Commerce Store API
  slug: virto-commerce-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-store-api-openapi.yml
- filename: virto-commerce-virtocommerce-platform-api-openapi.yml
  format: yaml
  label: Virto Commerce VirtoCommerce Platform API
  slug: virto-commerce-virtocommerce-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
- filename: virto-commerce-webhooks-api-openapi.yml
  format: yaml
  label: Virto Commerce Webhooks API
  slug: virto-commerce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-webhooks-api-openapi.yml
- filename: virto-commerce-event-bus-api-openapi.yml
  format: yaml
  label: Virto Commerce Event Bus API
  slug: virto-commerce-event-bus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-event-bus-api-openapi.yml
- filename: virto-commerce-returns-api-openapi.yml
  format: yaml
  label: Virto Commerce Returns API
  slug: virto-commerce-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-returns-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.virtocommerce.org/platform/developer-guide/Fundamentals/Security/
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Virto Commerce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Virto Commerce publishes 84 OAuth 2.0 scopes via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virto Commerce API on a user''s behalf.


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
  source: openapi/virto-commerce-catalog-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-companies-and-contacts-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-event-bus-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-inventory-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-marketing-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-order-management-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-pricing-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-quotes-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-returns-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-shopping-cart-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-store-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    tokenUrl: /connect/token
  - flow: clientCredentials
    tokenUrl: /connect/token
  name: oauth2
  source: openapi/virto-commerce-webhooks-api-openapi.yml
scope_count: 84
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
- eventbus:events:read
- eventbus:subscriptions:delete
- eventbus:subscriptions:read
- eventbus:subscriptions:update
- eventbus:subscriptions:сreate
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
- return:delete
- return:read
- return:update
- store:create
- store:read
- store:update
- webhooks:delete
- webhooks:feed:read
- webhooks:read
- webhooks:update
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
  scope: eventbus:events:read
- description: ''
  flows: []
  scope: eventbus:subscriptions:delete
- description: ''
  flows: []
  scope: eventbus:subscriptions:read
- description: ''
  flows: []
  scope: eventbus:subscriptions:update
- description: ''
  flows: []
  scope: eventbus:subscriptions:сreate
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
  scope: return:delete
- description: ''
  flows: []
  scope: return:read
- description: ''
  flows: []
  scope: return:update
- description: ''
  flows: []
  scope: store:create
- description: ''
  flows: []
  scope: store:read
- description: ''
  flows: []
  scope: store:update
- description: ''
  flows: []
  scope: webhooks:delete
- description: ''
  flows: []
  scope: webhooks:feed:read
- description: ''
  flows: []
  scope: webhooks:read
- description: ''
  flows: []
  scope: webhooks:update
slug: virto-commerce-scopes
source_filename: virto-commerce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: 'openapi/virto-commerce-catalog-api-openapi.yml, openapi/virto-commerce-companies-and-contacts-api-openapi.yml,\n  openapi/virto-commerce-event-bus-api-openapi.yml, openapi/virto-commerce-inventory-api-openapi.yml,\n  openapi/virto-commerce-marketing-api-openapi.yml, openapi/virto-commerce-order-management-api-openapi.yml,\n  openapi/virto-commerce-pricing-api-openapi.yml, openapi/virto-commerce-quotes-api-openapi.yml, openapi/virto-commerce-returns-api-openapi.yml,\n  openapi/virto-commerce-shopping-cart-api-openapi.yml, openapi/virto-commerce-store-api-openapi.yml,\n  openapi/virto-commerce-virtocommerce-platform-api-openapi.yml, openapi/virto-commerce-webhooks-api-openapi.yml\n\n  ; upgraded 2026-08-13 with the live discovery document https://virtostart-demo-admin.govirto.com/.well-known/openid-configuration\n  (HTTP 200)'\nschemes:\n- name: oauth2\n  source: openapi/virto-commerce-catalog-api-openapi.yml\n  flows:\n  -\
  \ flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-event-bus-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-inventory-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-marketing-api-openapi.yml\n\
  \  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-order-management-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-pricing-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-quotes-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-returns-api-openapi.yml\n\
  \  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-shopping-cart-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-store-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\n- name: oauth2\n  source: openapi/virto-commerce-webhooks-api-openapi.yml\n\
  \  flows:\n  - flow: password\n    tokenUrl: /connect/token\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n  description: OAuth2 Resource Owner Password Grant flow\nscopes:\n- scope: background_jobs:manage\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: cache:reset\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: cart:create\n  sources:\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n- scope: cart:delete\n  sources:\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n- scope: cart:read\n  sources:\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n- scope: cart:update\n  sources:\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n- scope: catalog:access\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:configurations:read\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:configurations:update\n  sources:\n\
  \  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:create\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:delete\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:dictionary-property:edit\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:read\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: catalog:update\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: customer:create\n  sources:\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n- scope: customer:delete\n  sources:\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n- scope: customer:invite\n  sources:\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n- scope: customer:read\n  sources:\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n- scope: customer:update\n  sources:\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n\
  - scope: eventbus:events:read\n  sources:\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n- scope: eventbus:subscriptions:delete\n  sources:\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n- scope: eventbus:subscriptions:read\n  sources:\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n- scope: eventbus:subscriptions:update\n  sources:\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n- scope: eventbus:subscriptions:сreate\n  sources:\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n- scope: inventory:fulfillment:delete\n  sources:\n  - openapi/virto-commerce-inventory-api-openapi.yml\n- scope: inventory:fulfillment:edit\n  sources:\n  - openapi/virto-commerce-inventory-api-openapi.yml\n- scope: inventory:fulfillment:read\n  sources:\n  - openapi/virto-commerce-inventory-api-openapi.yml\n- scope: inventory:read\n  sources:\n  - openapi/virto-commerce-inventory-api-openapi.yml\n- scope: inventory:update\n  sources:\n  - openapi/virto-commerce-inventory-api-openapi.yml\n\
  - scope: marketing:create\n  sources:\n  - openapi/virto-commerce-marketing-api-openapi.yml\n- scope: marketing:delete\n  sources:\n  - openapi/virto-commerce-marketing-api-openapi.yml\n- scope: marketing:read\n  sources:\n  - openapi/virto-commerce-marketing-api-openapi.yml\n- scope: marketing:update\n  sources:\n  - openapi/virto-commerce-marketing-api-openapi.yml\n- scope: measures:access\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: measures:create\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: measures:delete\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: measures:read\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: measures:update\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n- scope: order:capture_payment\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n- scope: order:create\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n\
  \  - openapi/virto-commerce-quotes-api-openapi.yml\n- scope: order:dashboardstatistics:view\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n- scope: order:payment:execute_callback\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n- scope: order:refund\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n- scope: order:update_shipments\n  sources:\n  - openapi/virto-commerce-order-management-api-openapi.yml\n- scope: platform:developer-tools:access\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:dynamic_properties:create\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:dynamic_properties:delete\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:dynamic_properties:read\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:dynamic_properties:update\n\
  \  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:module:manage\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:module:read\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:confirmEmail\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:create\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:delete\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:generateToken\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:oauth_applications:create\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:oauth_applications:delete\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n\
  - scope: platform:security:oauth_applications:read\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:oauth_applications:update\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:read\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:revokeToken\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:update\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:verifyEmail\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:security:verifyToken\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:setting:read\n  sources:\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: platform:setting:update\n  sources:\n\
  \  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n- scope: pricing:create\n  sources:\n  - openapi/virto-commerce-pricing-api-openapi.yml\n- scope: pricing:delete\n  sources:\n  - openapi/virto-commerce-pricing-api-openapi.yml\n- scope: pricing:read\n  sources:\n  - openapi/virto-commerce-pricing-api-openapi.yml\n- scope: pricing:update\n  sources:\n  - openapi/virto-commerce-pricing-api-openapi.yml\n- scope: quote:create\n  sources:\n  - openapi/virto-commerce-quotes-api-openapi.yml\n- scope: quote:delete\n  sources:\n  - openapi/virto-commerce-quotes-api-openapi.yml\n- scope: quote:read\n  sources:\n  - openapi/virto-commerce-quotes-api-openapi.yml\n- scope: quote:update\n  sources:\n  - openapi/virto-commerce-quotes-api-openapi.yml\n- scope: return:delete\n  sources:\n  - openapi/virto-commerce-returns-api-openapi.yml\n- scope: return:read\n  sources:\n  - openapi/virto-commerce-returns-api-openapi.yml\n- scope: return:update\n  sources:\n  - openapi/virto-commerce-returns-api-openapi.yml\n\
  - scope: store:create\n  sources:\n  - openapi/virto-commerce-store-api-openapi.yml\n- scope: store:read\n  sources:\n  - openapi/virto-commerce-store-api-openapi.yml\n- scope: store:update\n  sources:\n  - openapi/virto-commerce-store-api-openapi.yml\n- scope: webhooks:delete\n  sources:\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- scope: webhooks:feed:read\n  sources:\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- scope: webhooks:read\n  sources:\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- scope: webhooks:update\n  sources:\n  - openapi/virto-commerce-webhooks-api-openapi.yml\ndocs: https://docs.virtocommerce.org/platform/developer-guide/Fundamentals/Security/\nscopes_supported_live:\n- openid\n- offline_access\nfinding: The OAuth2 securitySchemes declare an empty scopes map in every one of the 13 module documents,\n  and the live authorization server advertises only openid and offline_access. Virto Commerce does NOT\n  use OAuth scopes for API authorization\
  \ — access is governed by the platform permission system (colon-namespaced\n  strings such as webhooks:read, catalog:update) attached to roles. Any scope names listed below are derived\n  from the spec structure, not an authorization vocabulary a client can request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/scopes/virto-commerce-scopes.yml
summary_line: 84 scopes · password/clientCredentials
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
- Webhooks
- Event-Driven
- CloudEvents
- GraphQL
- Returns
- MCP
- B2B Quotes
token_urls:
- /connect/token
---
