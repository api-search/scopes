---
api_specs:
- filename: triple-whale-api-keys-api-openapi.yml
  format: yaml
  label: Triple Whale API Keys API
  slug: triple-whale-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-api-keys-api-openapi.yml
- filename: triple-whale-compliance-api-openapi.yml
  format: yaml
  label: Triple Whale Compliance API
  slug: triple-whale-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-compliance-api-openapi.yml
- filename: triple-whale-data-in-api-openapi.yml
  format: yaml
  label: Triple Whale Data In API
  slug: triple-whale-data-in-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-in-api-openapi.yml
- filename: triple-whale-data-out-api-openapi.yml
  format: yaml
  label: Triple Whale Data Out API
  slug: triple-whale-data-out-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-data-out-api-openapi.yml
- filename: triple-whale-bi-benchmarks-openapi.json
  format: json
  label: Triple Whale Benchmarks API
  slug: triple-whale-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/openapi/triple-whale-bi-benchmarks-openapi.json
authorization_urls: []
description: ''
docs: https://triplewhale.readme.io/reference/creating-and-managing-triple-whale-api-keys
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Triple Whale Scopes
name_suffix: OAuth Scopes
note: Two independent scope systems exist and they are not the same vocabulary. The REST API uses named scopes attached to an API key at creation time in the app (Data > APIs); the hosted MCP server uses OAuth 2.1 scopes advertised in its RFC 9728 protected-resource metadata. Neither appears in any published OpenAPI — the derive pass over openapi/ found zero oauth2 security schemes, so every scope below was read from the provider's own documentation or from live metadata.
overview: 'Triple Whale uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Triple Whale
provider_slug: triple-whale
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: triple-whale-scopes
source_filename: triple-whale-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://triplewhale.readme.io/reference/creating-and-managing-triple-whale-api-keys\ndocs: https://triplewhale.readme.io/reference/creating-and-managing-triple-whale-api-keys\nnote: >-\n  Two independent scope systems exist and they are not the same vocabulary. The\n  REST API uses named scopes attached to an API key at creation time in the app\n  (Data > APIs); the hosted MCP server uses OAuth 2.1 scopes advertised in its\n  RFC 9728 protected-resource metadata. Neither appears in any published OpenAPI —\n  the derive pass over openapi/ found zero oauth2 security schemes, so every scope\n  below was read from the provider's own documentation or from live metadata.\n\napi_key_scopes:\n  mechanism: named scopes bound to an API key\n  issuance: https://app.triplewhale.com/api-keys\n  verification_endpoint: GET /api/v2/users/api-keys/me\n  scopes:\n  - scope: 'Summary Page: Read'\n    description: Retrieve data from the Summary\
  \ Page endpoint.\n    operations: [get-summary-page-data]\n  - scope: 'Pixel Attribution: Read'\n    description: Access customer journey data from the Attribution endpoint.\n    operations: [get-customer-journey-attribution-data]\n  - scope: 'MCP: Read'\n    description: Access Triple Whale data through the Model Context Protocol server.\n    operations: []\n    surface: mcp\n  - scope: 'Ads: Write'\n    description: Upload ad records to the Ads Data-In endpoint.\n    operations: [create-ad-record]\n  - scope: 'Orders: Write'\n    description: >-\n      Upload order records to the Orders Data-In endpoint, or enrich order records\n      via the Enrich Orders Data endpoint.\n    operations: [create-order-record, bulk-create-order-records, enrich-orders-data]\n  - scope: 'Customers: Write'\n    description: Upload customer records to the Customers Data-In endpoint.\n    operations: [create-customer-record]\n  - scope: 'Products: Write'\n    description: Upload product records to the Products\
  \ Data-In endpoint.\n    operations: [create-product-record, enrich-products-data]\n  - scope: 'PPS: Write'\n    description: Upload post-purchase survey records to the PPS Data-In endpoint.\n    operations: [create-pps-record]\n  - scope: 'Subscriptions: Write'\n    description: Upload subscription records to the Subscriptions Data-In endpoint.\n    operations: [create-subscription-record]\n  - scope: 'Compliance: Write'\n    description: Submit data deletion requests to the Compliance endpoint.\n    operations: [create-compliance-request]\n  undocumented_scope_note: >-\n    The troubleshooting guide also references a \"Data Out\" scope covering the SQL\n    and Moby endpoints, but that name does not appear in the scope-selection list on\n    the key-creation page. Recorded as an inconsistency rather than resolved.\n\noauth2:\n  surface: https://mcp.triplewhale.com/sse\n  metadata:\n    authorization_server: https://mcp.triplewhale.com/.well-known/oauth-authorization-server\n    protected_resource:\
  \ https://mcp.triplewhale.com/.well-known/oauth-protected-resource\n    file: well-known/triple-whale-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.triplewhale.com/authorize\n    tokenUrl: https://mcp.triplewhale.com/token\n    registrationUrl: https://mcp.triplewhale.com/register\n    pkce: S256\n  grant_types: [authorization_code, refresh_token]\n  scopes:\n  - scope: moby:read\n    description: Read access to Triple Whale data through the Moby MCP server.\n  - scope: offline\n    description: Issue a refresh token.\n  - scope: offline_access\n    description: Issue a refresh token (RFC 6749 / OIDC spelling).\n  method: probed\n  probed: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-whale/refs/heads/main/scopes/triple-whale-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- E-Commerce
- Analytics
- Attribution
- Shopify
- Pixel Tracking
- ROAS
- Direct to Consumer
- Marketing
token_urls: []
---
