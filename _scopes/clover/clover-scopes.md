---
authorization_urls:
- https://www.clover.com/oauth/authorize
description: ''
docs: https://docs.clover.com/dev/docs/permissions
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Clover Scopes
name_suffix: OAuth Scopes
note: Clover does not use an OAuth scope parameter; access is governed by Read/Write app permissions per category, configured in the Developer Dashboard and granted by the merchant when installing the app via the OAuth flow (https://docs.clover.com/dev/docs/permissions, https://docs.clover.com/dev/docs/ecommerce-app-permissions).
overview: 'Clover publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clover API on a user''s behalf.


  Tokens are issued from https://api.clover.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clover
provider_slug: clover
schemes:
- description: OAuth 2.0 token or Ecommerce (PAKMS) API key.
  flows:
  - authorizationUrl: https://www.clover.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.clover.com/oauth/token
  name: OAuth2
  source: openapi/clover-ecommerce-api-openapi.yml
scope_count: 13
scope_names:
- Read customers
- Write customers
- Read employees
- Write employees
- Read inventory
- Write inventory
- Read merchant
- Write merchant
- Read orders
- Write orders
- Read payments
- Write payments
- Online payments
scopes:
- description: Required to read customer information.
  flows: []
  scope: Read customers
- description: Required to add and update customer information.
  flows: []
  scope: Write customers
- description: Required to read employee information, for example, to view who created an order.
  flows: []
  scope: Read employees
- description: Required to add and update employees.
  flows: []
  scope: Write employees
- description: Required to read inventory.
  flows: []
  scope: Read inventory
- description: Required to add and update inventory.
  flows: []
  scope: Write inventory
- description: Required to read merchant properties, for example, to view basic information for a merchant.
  flows: []
  scope: Read merchant
- description: Required to update merchant properties.
  flows: []
  scope: Write merchant
- description: Required to read order information.
  flows: []
  scope: Read orders
- description: Required to add and update an order.
  flows: []
  scope: Write orders
- description: Required to read payment information.
  flows: []
  scope: Read payments
- description: Required to add and update payment records.
  flows: []
  scope: Write payments
- description: Ecommerce API permission for Clover apps providing card-not-present payments; required to create charges and process payments.
  flows: []
  scope: Online payments
slug: clover-scopes
source_filename: clover-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/clover-ecommerce-api-openapi.yml\ndocs: https://docs.clover.com/dev/docs/permissions\nnote: Clover does not use an OAuth scope parameter; access is governed by Read/Write\n  app permissions per category, configured in the Developer Dashboard and granted\n  by the merchant when installing the app via the OAuth flow\n  (https://docs.clover.com/dev/docs/permissions,\n  https://docs.clover.com/dev/docs/ecommerce-app-permissions).\nschemes:\n- name: OAuth2\n  source: openapi/clover-ecommerce-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.clover.com/oauth/authorize\n    tokenUrl: https://api.clover.com/oauth/token\n  description: OAuth 2.0 token or Ecommerce (PAKMS) API key.\nscopes:\n- scope: Read customers\n  description: Required to read customer information.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write customers\n  description: Required to add\
  \ and update customer information.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Read employees\n  description: Required to read employee information, for example, to view who created\n    an order.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write employees\n  description: Required to add and update employees.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Read inventory\n  description: Required to read inventory.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write inventory\n  description: Required to add and update inventory.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Read merchant\n  description: Required to read merchant properties, for example, to view basic information\n    for a merchant.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write merchant\n  description: Required to update merchant properties.\n  sources:\n  -\
  \ https://docs.clover.com/dev/docs/permissions\n- scope: Read orders\n  description: Required to read order information.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write orders\n  description: Required to add and update an order.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Read payments\n  description: Required to read payment information.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Write payments\n  description: Required to add and update payment records.\n  sources:\n  - https://docs.clover.com/dev/docs/permissions\n- scope: Online payments\n  description: Ecommerce API permission for Clover apps providing card-not-present\n    payments; required to create charges and process payments.\n  sources:\n  - https://docs.clover.com/dev/docs/ecommerce-app-permissions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover/refs/heads/main/scopes/clover-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Restaurant
- POS
- Payments
- Retail
- SMB
- Hardware
token_urls:
- https://api.clover.com/oauth/token
---
