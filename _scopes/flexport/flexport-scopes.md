---
authorization_urls: []
description: ''
docs: https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Flexport Scopes
name_suffix: OAuth Scopes
note: The core Flexport REST API (api.flexport.com) uses OAuth 2.0 client credentials with per-credential access controls and publishes no scopes (https://apidocs.flexport.com/v2/tag/Authentication/); the scopes below are the documented permission scopes for the Flexport Logistics API OAuth authorization code flow (https://docs.logistics-api.flexport.com/2026-02/tag/OAuth/).
overview: 'Flexport publishes 22 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flexport API on a user''s behalf.


  Tokens are issued from https://api.flexport.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flexport
provider_slug: flexport
schemes:
- description: OAuth 2.0 client credentials issued from the Flexport admin console
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.flexport.com/oauth/token
  name: oauth2
  source: openapi/flexport-openapi.yml
scope_count: 22
scope_names:
- read_logistics_products
- write_logistics_products
- read_logistics_inbounds
- write_logistics_inbounds
- read_logistics_orders
- write_logistics_orders
- read_logistics_orders_b2b
- write_logistics_orders_b2b
- read_logistics_bundles
- write_logistics_bundles
- read_logistics_parcels
- write_logistics_parcels
- read_logistics_returns
- write_logistics_returns
- read_logistics_warehouses
- read_logistics_webhooks
- write_logistics_webhooks
- read_logistics_events
- read_logistics_reports
- write_logistics_reports
- read_logistics_freight
- write_logistics_freight
scopes:
- description: Read the product catalog (SKUs, dimensions, barcodes).
  flows: []
  scope: read_logistics_products
- description: Create and update products in the catalog.
  flows: []
  scope: write_logistics_products
- description: Read inbound shipments and their contents.
  flows: []
  scope: read_logistics_inbounds
- description: Create, cancel, and modify inbound shipments.
  flows: []
  scope: write_logistics_inbounds
- description: Read outbound (D2C) orders and shipments.
  flows: []
  scope: read_logistics_orders
- description: Create, cancel, and modify outbound (D2C) orders.
  flows: []
  scope: write_logistics_orders
- description: Read B2B orders and shipments. (2024-07 and later.)
  flows: []
  scope: read_logistics_orders_b2b
- description: Create, cancel, and modify B2B orders. (2024-07 and later.)
  flows: []
  scope: write_logistics_orders_b2b
- description: Read bundle (kit) definitions.
  flows: []
  scope: read_logistics_bundles
- description: Create and update bundle definitions.
  flows: []
  scope: write_logistics_bundles
- description: Read parcel labels, rates, and master cartons.
  flows: []
  scope: read_logistics_parcels
- description: Purchase parcel labels and create/link master cartons.
  flows: []
  scope: write_logistics_parcels
- description: Read return shipments and their contents.
  flows: []
  scope: read_logistics_returns
- description: Create and update return shipments.
  flows: []
  scope: write_logistics_returns
- description: Read the list of warehouses available to the account. (2025-03 and later.)
  flows: []
  scope: read_logistics_warehouses
- description: Read webhook subscriptions.
  flows: []
  scope: read_logistics_webhooks
- description: Create, update, and delete webhook subscriptions.
  flows: []
  scope: write_logistics_webhooks
- description: Read the event stream that backs webhook deliveries.
  flows: []
  scope: read_logistics_events
- description: Read generated reports.
  flows: []
  scope: read_logistics_reports
- description: Request new reports.
  flows: []
  scope: write_logistics_reports
- description: Listed as an accepted scope value on the OAuth AuthorizationRedirect call; covers experimental freight endpoints available only in the unstable API version.
  flows: []
  scope: read_logistics_freight
- description: Listed as an accepted scope value on the OAuth AuthorizationRedirect call; covers experimental freight endpoints available only in the unstable API version.
  flows: []
  scope: write_logistics_freight
slug: flexport-scopes
source_filename: flexport-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/flexport-openapi.yml\ndocs: https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\nnote: >-\n  The core Flexport REST API (api.flexport.com) uses OAuth 2.0 client credentials\n  with per-credential access controls and publishes no scopes\n  (https://apidocs.flexport.com/v2/tag/Authentication/); the scopes below are the\n  documented permission scopes for the Flexport Logistics API OAuth authorization\n  code flow (https://docs.logistics-api.flexport.com/2026-02/tag/OAuth/).\nschemes:\n- name: oauth2\n  source: openapi/flexport-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.flexport.com/oauth/token\n  description: OAuth 2.0 client credentials issued from the Flexport admin console\nscopes:\n- scope: read_logistics_products\n  description: Read the product catalog (SKUs, dimensions, barcodes).\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n\
  - scope: write_logistics_products\n  description: Create and update products in the catalog.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_inbounds\n  description: Read inbound shipments and their contents.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_inbounds\n  description: Create, cancel, and modify inbound shipments.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_orders\n  description: Read outbound (D2C) orders and shipments.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_orders\n  description: Create, cancel, and modify outbound (D2C) orders.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n\
  - scope: read_logistics_orders_b2b\n  description: Read B2B orders and shipments. (2024-07 and later.)\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_orders_b2b\n  description: Create, cancel, and modify B2B orders. (2024-07 and later.)\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_bundles\n  description: Read bundle (kit) definitions.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_bundles\n  description: Create and update bundle definitions.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_parcels\n  description: Read parcel labels, rates, and master cartons.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n\
  - scope: write_logistics_parcels\n  description: Purchase parcel labels and create/link master cartons.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_returns\n  description: Read return shipments and their contents.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_returns\n  description: Create and update return shipments.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_warehouses\n  description: Read the list of warehouses available to the account. (2025-03 and later.)\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_webhooks\n  description: Read webhook subscriptions.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n\
  - scope: write_logistics_webhooks\n  description: Create, update, and delete webhook subscriptions.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_events\n  description: Read the event stream that backs webhook deliveries.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_reports\n  description: Read generated reports.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: write_logistics_reports\n  description: Request new reports.\n  sources:\n  - https://docs.logistics-api.flexport.com/2026-02/#section/Common-Resources/Permission-Scopes\n- scope: read_logistics_freight\n  description: Listed as an accepted scope value on the OAuth AuthorizationRedirect\n    call; covers experimental freight endpoints available only in the unstable API\n    version.\n \
  \ sources:\n  - https://docs.logistics-api.flexport.com/2023-10/tag/OAuth/\n- scope: write_logistics_freight\n  description: Listed as an accepted scope value on the OAuth AuthorizationRedirect\n    call; covers experimental freight endpoints available only in the unstable API\n    version.\n  sources:\n  - https://docs.logistics-api.flexport.com/2023-10/tag/OAuth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexport/refs/heads/main/scopes/flexport-scopes.yml
summary_line: 22 scopes · clientCredentials
tags:
- Logistics
- Freight
- Supply Chain
- Customs
- B2B
token_urls:
- https://api.flexport.com/oauth/token
---
