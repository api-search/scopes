---
api_specs:
- filename: shopware-account-api-openapi.yml
  format: yaml
  label: Shopware Account API
  slug: shopware-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-account-api-openapi.yml
- filename: shopware-bulk-api-openapi.yml
  format: yaml
  label: Shopware Bulk API
  slug: shopware-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-bulk-api-openapi.yml
- filename: shopware-cart-api-openapi.yml
  format: yaml
  label: Shopware Cart API
  slug: shopware-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-cart-api-openapi.yml
- filename: shopware-category-api-openapi.yml
  format: yaml
  label: Shopware Category API
  slug: shopware-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-category-api-openapi.yml
- filename: shopware-checkout-api-openapi.yml
  format: yaml
  label: Shopware Checkout API
  slug: shopware-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-checkout-api-openapi.yml
- filename: shopware-customer-api-openapi.yml
  format: yaml
  label: Shopware Customer API
  slug: shopware-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-customer-api-openapi.yml
- filename: shopware-navigation-api-openapi.yml
  format: yaml
  label: Shopware Navigation API
  slug: shopware-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-navigation-api-openapi.yml
- filename: shopware-order-api-openapi.yml
  format: yaml
  label: Shopware Order API
  slug: shopware-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-order-api-openapi.yml
- filename: shopware-product-api-openapi.yml
  format: yaml
  label: Shopware Product API
  slug: shopware-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-product-api-openapi.yml
- filename: shopware-search-api-openapi.yml
  format: yaml
  label: Shopware Search API
  slug: shopware-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/openapi/shopware-search-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
- password
kind: oauth-scopes
layout: scope
method: derived
name: Shopware Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shopware publishes 1 OAuth 2.0 scope via the clientCredentials and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shopware API on a user''s behalf.


  Tokens are issued from /api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shopware
provider_slug: shopware
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /api/oauth/token
  - flow: password
    tokenUrl: /api/oauth/token
  name: oAuth2
  source: openapi/shopware-admin-api-openapi.yml
scope_count: 1
scope_names:
- write:all
scopes:
- description: Full write access to all Admin API resources
  flows:
  - clientCredentials
  - password
  scope: write:all
slug: shopware-scopes
source_filename: shopware-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shopware-admin-api-openapi.yml\nschemes:\n- name: oAuth2\n  source: openapi/shopware-admin-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /api/oauth/token\n  - flow: password\n    tokenUrl: /api/oauth/token\nscopes:\n- scope: write:all\n  description: Full write access to all Admin API resources\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/shopware-admin-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopware/refs/heads/main/scopes/shopware-scopes.yml
summary_line: 1 scope · clientCredentials/password
tags:
- E-Commerce
- Open-Source
- Headless Commerce
- B2B
- B2C
- REST
- Authentication
token_urls:
- /api/oauth/token
---
