---
api_specs:
- filename: google-merchant-center-accounts-api-openapi.yml
  format: yaml
  label: Google Merchant Center Accounts API
  slug: google-merchant-center-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-accounts-api-openapi.yml
- filename: google-merchant-center-inventories-api-openapi.yml
  format: yaml
  label: Google Merchant Center Inventories API
  slug: google-merchant-center-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-inventories-api-openapi.yml
- filename: google-merchant-center-products-api-openapi.yml
  format: yaml
  label: Google Merchant Center Products API
  slug: google-merchant-center-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-products-api-openapi.yml
- filename: google-merchant-center-promotions-api-openapi.yml
  format: yaml
  label: Google Merchant Center Promotions API
  slug: google-merchant-center-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-promotions-api-openapi.yml
- filename: google-merchant-center-reports-api-openapi.yml
  format: yaml
  label: Google Merchant Center Reports API
  slug: google-merchant-center-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/openapi/google-merchant-center-reports-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Merchant Center Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Merchant Center publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Merchant Center API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Merchant Center
provider_slug: google-merchant-center
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/content
scopes:
- description: Manage Google Shopping data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/content
slug: google-merchant-center-scopes
source_filename: google-merchant-center-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/content\n  description: Manage Google Shopping data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-merchant-center/refs/heads/main/scopes/google-merchant-center-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- E-Commerce
- Google Shopping
- Inventory
- Merchant Center
- Product
- Promotions
- Shopping
token_urls:
- https://oauth2.googleapis.com/token
---
