---
api_specs:
- filename: depixapp-com-account-api-openapi.yml
  format: yaml
  label: DePix App Account API
  slug: depixapp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-account-api-openapi.yml
- filename: depixapp-com-agents-api-openapi.yml
  format: yaml
  label: DePix App Agents API
  slug: depixapp-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-agents-api-openapi.yml
- filename: depixapp-com-checkouts-api-openapi.yml
  format: yaml
  label: DePix App Checkouts API
  slug: depixapp-com-checkouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-checkouts-api-openapi.yml
- filename: depixapp-com-merchant-api-openapi.yml
  format: yaml
  label: DePix App Merchant API
  slug: depixapp-com-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-merchant-api-openapi.yml
- filename: depixapp-com-meta-api-openapi.yml
  format: yaml
  label: DePix App Meta API
  slug: depixapp-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-meta-api-openapi.yml
- filename: depixapp-com-pay-api-openapi.yml
  format: yaml
  label: DePix App Pay API
  slug: depixapp-com-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-pay-api-openapi.yml
- filename: depixapp-com-products-api-openapi.yml
  format: yaml
  label: DePix App Products API
  slug: depixapp-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-products-api-openapi.yml
- filename: depixapp-com-public-api-openapi.yml
  format: yaml
  label: DePix App Public API
  slug: depixapp-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-public-api-openapi.yml
- filename: depixapp-com-support-api-openapi.yml
  format: yaml
  label: DePix App Support API
  slug: depixapp-com-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/depixapp-com/openapi/depixapp-com-support-api-openapi.yml
authorization_urls: []
description: ''
docs: https://depixapp.com/docs/en/#scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Depixapp Com Scopes
name_suffix: OAuth Scopes
note: Scopes are attached to API keys (Bearer sk_*), chosen at key creation and immutable. No implicit hierarchy. The OpenAPI declares no oauth2 scheme; the hosted MCP OAuth 2.1 connector sessions are capped to read + merchant scopes.
overview: 'DePix App publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DePix App API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DePix App
provider_slug: depixapp-com
schemes: []
scope_count: 4
scope_names:
- merchant_read
- merchant_write
- wallet_read
- wallet_write
scopes:
- description: 'All GETs of the merchant surface: list/get checkouts, products, and GET /api/me.'
  flows: []
  scope: merchant_read
- description: 'The "receiving" side: create/simulate checkouts, the product CRUD, and editing the store''s light profile fields (PATCH /api/merchants/me).'
  flows: []
  scope: merchant_write
- description: 'Reading the wallet-side status: GET /api/deposits/:id and GET /api/withdrawals/:id. Never granted by default.'
  flows: []
  scope: wallet_read
- description: 'The "paying" side (moving money): POST /api/deposit, POST /api/withdraw. Never granted by default. Keys are born with mandatory spending limits (defaults R$ 100.00 per transaction, R$ 500.00 per day).'
  flows: []
  scope: wallet_write
slug: depixapp-com-scopes
source_filename: depixapp-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://depixapp.com/docs/en/#scopes\ndocs: https://depixapp.com/docs/en/#scopes\nnote: Scopes are attached to API keys (Bearer sk_*), chosen at key creation and immutable. No implicit hierarchy. The OpenAPI declares no oauth2 scheme; the hosted MCP OAuth 2.1 connector sessions are capped to read + merchant scopes.\nscopes:\n- name: merchant_read\n  description: 'All GETs of the merchant surface: list/get checkouts, products, and GET /api/me.'\n  default: true\n- name: merchant_write\n  description: 'The \"receiving\" side: create/simulate checkouts, the product CRUD, and editing the store''s light profile fields (PATCH /api/merchants/me).'\n  default: true\n- name: wallet_read\n  description: 'Reading the wallet-side status: GET /api/deposits/:id and GET /api/withdrawals/:id. Never granted by default.'\n  default: false\n- name: wallet_write\n  description: 'The \"paying\" side (moving money): POST /api/deposit, POST /api/withdraw.\
  \ Never granted by default. Keys are born with mandatory spending limits (defaults R$ 100.00 per transaction, R$ 500.00 per day).'\n  default: false\ninsufficient_scope: 403 with error.code = \"insufficient_scope\" and details.required_scope\n"
source_yaml_url: https://artifacts.apis.io/depixapp-com/scopes/depixapp-com-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Payments
- Pix
- Stablecoins
- Cryptocurrency
- Bitcoin
- Liquid Network
- Brazil
- MCP
token_bound: false
token_urls: []
---
