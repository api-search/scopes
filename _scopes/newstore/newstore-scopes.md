---
api_specs:
- filename: newstore-api-openapi-original.json
  format: json
  label: NewStore Omnichannel API
  slug: newstore-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/openapi/newstore-api-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Newstore Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Newstore publishes 29 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Newstore API on a user''s behalf.


  Tokens are issued from https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Newstore
provider_slug: newstore
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token
  name: oauth
  source: openapi/newstore-api-openapi-original.json
scope_count: 29
scope_names:
- audit-events:read
- catalog:import-schemas:read
- catalog:import-schemas:write
- catalog:pricebook-export:read
- catalog:product-export:read
- checkout:carts:read
- checkout:carts:write
- clienteling:profile:read
- customer:profile:read
- customer:profile:write
- fiscalization:orders:read
- fiscalization:orders:write
- iam:providers:read
- iam:providers:write
- iam:roles:read
- iam:roles:write
- iam:users:read
- iam:users:write
- inventory:reservations:read
- inventory:reservations:write
- newstore:configuration:read
- newstore:configuration:write
- promotions:config:read
- promotions:config:write
- promotions:reason-codes:read
- promotions:reason-codes:write
- shipments:read
- taxes:preview-transactions:write
- taxes:transactions:read
scopes:
- description: Grants read access to the tenant's audit events.
  flows:
  - clientCredentials
  scope: audit-events:read
- description: Grants privileges to read import schema
  flows:
  - clientCredentials
  scope: catalog:import-schemas:read
- description: Grants privileges to write import schema
  flows:
  - clientCredentials
  scope: catalog:import-schemas:write
- description: Grants privileges to export pricebook data
  flows:
  - clientCredentials
  scope: catalog:pricebook-export:read
- description: Grants privileges to export product data
  flows:
  - clientCredentials
  scope: catalog:product-export:read
- description: Grants privileges to read cart data
  flows:
  - clientCredentials
  scope: checkout:carts:read
- description: Grants privileges to write cart data
  flows:
  - clientCredentials
  scope: checkout:carts:write
- description: Grants privileges to read clienteling profiles
  flows:
  - clientCredentials
  scope: clienteling:profile:read
- description: Grants privileges to read API customer data
  flows:
  - clientCredentials
  scope: customer:profile:read
- description: Grants privileges to modify API customer data
  flows:
  - clientCredentials
  scope: customer:profile:write
- description: View orders with fiscal transactions and signatures
  flows:
  - clientCredentials
  scope: fiscalization:orders:read
- description: Create orders with fiscal transactions and signatures
  flows:
  - clientCredentials
  scope: fiscalization:orders:write
- description: Grants read privileges to provider resources
  flows:
  - clientCredentials
  scope: iam:providers:read
- description: Grants write privileges to provider resources
  flows:
  - clientCredentials
  scope: iam:providers:write
- description: Grants privileges to read roles data
  flows:
  - clientCredentials
  scope: iam:roles:read
- description: Grants privileges to write roles data
  flows:
  - clientCredentials
  scope: iam:roles:write
- description: Grants privileges to read user data
  flows:
  - clientCredentials
  scope: iam:users:read
- description: Grants privileges to write user data
  flows:
  - clientCredentials
  scope: iam:users:write
- description: Allows access to retrieve reservations
  flows:
  - clientCredentials
  scope: inventory:reservations:read
- description: Allows access to create and update reservations
  flows:
  - clientCredentials
  scope: inventory:reservations:write
- description: Grants privileges to read configuration
  flows:
  - clientCredentials
  scope: newstore:configuration:read
- description: Grants privileges to write configuration
  flows:
  - clientCredentials
  scope: newstore:configuration:write
- description: Grants privileges to read configuration
  flows:
  - clientCredentials
  scope: promotions:config:read
- description: Grants privileges to write into configuration
  flows:
  - clientCredentials
  scope: promotions:config:write
- description: Grants privileges to list reason codes
  flows:
  - clientCredentials
  scope: promotions:reason-codes:read
- description: Grants privileges to create and update reason codes
  flows:
  - clientCredentials
  scope: promotions:reason-codes:write
- description: Read Shipping Options and Audits
  flows:
  - clientCredentials
  scope: shipments:read
- description: Preview tax transactions
  flows:
  - clientCredentials
  scope: taxes:preview-transactions:write
- description: Read tax transactions
  flows:
  - clientCredentials
  scope: taxes:transactions:read
slug: newstore-scopes
source_filename: newstore-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/newstore-api-openapi-original.json\nschemes:\n- name: oauth\n  source: openapi/newstore-api-openapi-original.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token\nscopes:\n- scope: audit-events:read\n  description: Grants read access to the tenant's audit events.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: catalog:import-schemas:read\n  description: Grants privileges to read import schema\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: catalog:import-schemas:write\n  description: Grants privileges to write import schema\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: catalog:pricebook-export:read\n  description: Grants privileges to export pricebook data\n  flows:\n\
  \  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: catalog:product-export:read\n  description: Grants privileges to export product data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: checkout:carts:read\n  description: Grants privileges to read cart data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: checkout:carts:write\n  description: Grants privileges to write cart data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: clienteling:profile:read\n  description: Grants privileges to read clienteling profiles\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: customer:profile:read\n  description: Grants privileges to read API customer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n\
  - scope: customer:profile:write\n  description: Grants privileges to modify API customer data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: fiscalization:orders:read\n  description: View orders with fiscal transactions and signatures\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: fiscalization:orders:write\n  description: Create orders with fiscal transactions and signatures\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:providers:read\n  description: Grants read privileges to provider resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:providers:write\n  description: Grants write privileges to provider resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:roles:read\n  description: Grants\
  \ privileges to read roles data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:roles:write\n  description: Grants privileges to write roles data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:users:read\n  description: Grants privileges to read user data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: iam:users:write\n  description: Grants privileges to write user data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: inventory:reservations:read\n  description: Allows access to retrieve reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: inventory:reservations:write\n  description: Allows access to create and update reservations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n\
  - scope: newstore:configuration:read\n  description: Grants privileges to read configuration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: newstore:configuration:write\n  description: Grants privileges to write configuration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: promotions:config:read\n  description: Grants privileges to read configuration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: promotions:config:write\n  description: Grants privileges to write into configuration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: promotions:reason-codes:read\n  description: Grants privileges to list reason codes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: promotions:reason-codes:write\n  description: Grants privileges\
  \ to create and update reason codes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: shipments:read\n  description: Read Shipping Options and Audits\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: taxes:preview-transactions:write\n  description: Preview tax transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n- scope: taxes:transactions:read\n  description: Read tax transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/newstore-api-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newstore/refs/heads/main/scopes/newstore-scopes.yml
summary_line: 29 scopes · clientCredentials
tags:
- Company
- Retail
- Omnichannel
- Order Management
- Point of Sale
- Ecommerce
- Fulfillment
- Inventory
- Store Operations
- REST
token_urls:
- https://id.p.newstore.net/auth/realms/dodici-demo/protocol/openid-connect/token
---
