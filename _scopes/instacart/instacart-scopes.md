---
api_specs:
- filename: instacart-authentication-api-openapi.yml
  format: yaml
  label: instacart Authentication API
  slug: instacart-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-authentication-api-openapi.yml
- filename: instacart-chat-api-openapi.yml
  format: yaml
  label: instacart Chat API
  slug: instacart-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-chat-api-openapi.yml
- filename: instacart-delivery-api-openapi.yml
  format: yaml
  label: instacart Delivery API
  slug: instacart-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-delivery-api-openapi.yml
- filename: instacart-items-api-openapi.yml
  format: yaml
  label: instacart Items API
  slug: instacart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-items-api-openapi.yml
- filename: instacart-last-mile-delivery-api-openapi.yml
  format: yaml
  label: instacart Last Mile Delivery API
  slug: instacart-last-mile-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-last-mile-delivery-api-openapi.yml
- filename: instacart-orders-api-openapi.yml
  format: yaml
  label: instacart Orders API
  slug: instacart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-orders-api-openapi.yml
- filename: instacart-pickup-api-openapi.yml
  format: yaml
  label: instacart Pickup API
  slug: instacart-pickup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-pickup-api-openapi.yml
- filename: instacart-products-api-openapi.yml
  format: yaml
  label: instacart Products API
  slug: instacart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-products-api-openapi.yml
- filename: instacart-replacements-api-openapi.yml
  format: yaml
  label: instacart Replacements API
  slug: instacart-replacements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-replacements-api-openapi.yml
- filename: instacart-rest-api-openapi.yml
  format: yaml
  label: instacart Rest API
  slug: instacart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/openapi/instacart-rest-api-openapi.yml
authorization_urls: []
description: 'OAuth 2.0 permissions for the Instacart Connect APIs. Scope is selected at token-request time and the resulting access token is limited to that API. Instacart''s own guidance is to request the narrowest scope for the task. Note the shape is unusual: `scope` and `grant_type` are coupled - the same capability (Order Feedback) takes a different grant type depending on whether it is implemented in the backend or the frontend - and one API (Transaction) takes no scope at all. Multiple scopes may be requested in one token request, comma-separated, only when they share a grant_type. Omitting scope on a client_credentials request yields a token covering every permitted API for that grant type, which is the opposite of least privilege and worth calling out. These scopes are documented, not declared: no oauth2 securityScheme with a scopes map appears in the harvested OpenAPI, so derive-oauth-scopes.py found zero. Everything below was read from the docs.'
docs: https://docs.instacart.com/connect/api/permissions_scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Instacart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'instacart uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: instacart
provider_slug: instacart
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: instacart-scopes
source_filename: instacart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\ndocs: https://docs.instacart.com/connect/api/permissions_scopes\nsource: >-\n  https://docs.instacart.com/connect/api/permissions_scopes and\n  https://docs.instacart.com/connect/api/access_tokens\nprovider: Instacart\nproviderId: instacart\ndescription: >-\n  OAuth 2.0 permissions for the Instacart Connect APIs. Scope is selected at token-request time and the\n  resulting access token is limited to that API. Instacart's own guidance is to request the narrowest\n  scope for the task. Note the shape is unusual: `scope` and `grant_type` are coupled - the same\n  capability (Order Feedback) takes a different grant type depending on whether it is implemented in\n  the backend or the frontend - and one API (Transaction) takes no scope at all. Multiple scopes may\n  be requested in one token request, comma-separated, only when they share a grant_type. Omitting\n  scope on a client_credentials request yields a token covering every permitted\
  \ API for that grant\n  type, which is the opposite of least privilege and worth calling out.\n  These scopes are documented, not declared: no oauth2 securityScheme with a scopes map appears in the\n  harvested OpenAPI, so derive-oauth-scopes.py found zero. Everything below was read from the docs.\nderived_from_spec: false\ntoken_endpoint: POST https://connect.instacart.com/v2/oauth/token\ntoken_lifetime: 24 hours\nrevocation_endpoint: POST /v2/oauth/revoke_access_token\nscopes:\n  - name: 'connect:fulfillment'\n    grant_type: client_credentials\n    api: Fulfillment API\n    description: >-\n      Access stores, service options, reservations, order creation and order management.\n    docs: https://docs.instacart.com/connect/api/fulfillment/overview\n  - name: 'Connect::Orders::RatingService'\n    grant_type: client_credentials\n    api: Order Feedback API (backend implementation)\n    description: Create or update order feedback from a backend implementation.\n    docs: https://docs.instacart.com/connect/api/fulfillment/overview\n\
  \  - name: 'Connect::Orders::RatingService'\n    grant_type: 'fulfillment_user_assertion | urn:ietf:params:oauth:grant-type:retailer-json-bearer'\n    api: Order Feedback API (frontend implementation)\n    description: >-\n      Create or update order feedback from a frontend implementation, on behalf of an end user.\n    docs: https://docs.instacart.com/connect/api/fulfillment/overview\n  - name: 'connect:post_checkout'\n    grant_type: fulfillment_user_assertion\n    api: Post-checkout API\n    description: Access order detail and order status for a customer's order.\n    docs: https://docs.instacart.com/connect/api/post_checkout/overview\n  - name: account_linking\n    grant_type: authorization_code\n    api: Account linking\n    description: Link a customer's Connect user account to their Instacart account.\n    docs: https://docs.instacart.com/connect/api/fulfillment/users/generate_linking_token\n  - name: 'connect:data_ingestion'\n    grant_type: client_credentials\n    api: Catalog\
  \ API\n    description: >-\n      Submit products and items to the retailer catalog. Not listed in the public permissions table;\n      captured from the bearerAuth description in Instacart's own Catalog API definition\n      (openapi/_original/instacart-catalog-api-openapi.yml).\n    source: openapi\n    docs: https://docs.instacart.com/catalog/catalog_api/overview/\nno_scope_required:\n  - api: Transaction API\n    grant_type: client_credentials\n    description: Send point of sale transaction information to Instacart. Scope value is None.\n    docs: https://docs.instacart.com/connect/api/transaction/overview\nnotes:\n  - >-\n    \"Partner retailers may have access to private APIs\" with scope values published only in partner\n    documentation, so this list is the public subset, not the complete set.\n  - >-\n    The Developer Platform API (/idp/v1) does not use OAuth at all. It uses API keys with three\n    permission levels - read-only, read-write and admin - configured in the Developer\
  \ Dashboard.\n    Those are permission tiers, not OAuth scopes, and are recorded in\n    authentication/instacart-authentication.yml and conventions/instacart-conventions.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instacart/refs/heads/main/scopes/instacart-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Grocery
- E-Commerce
- Marketplace
- Retail
- Logistics
- Last Mile Delivery
- Fulfillment
- Catalog
- Advertising
- Agents
- MCP
token_urls: []
---
