---
api_specs:
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Products API
  slug: nacelle-storefront-products-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Product Collections API
  slug: nacelle-storefront-product-collections-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Content API
  slug: nacelle-storefront-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Navigation and Spaces API
  slug: nacelle-storefront-navigation-spaces-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Admin Indexing and Ingestion API
  slug: nacelle-admin-indexing-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle-addresses-api-openapi.yml
  format: yaml
  label: Nacelle Addresses API
  slug: nacelle-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-addresses-api-openapi.yml
- filename: nacelle-checkout-api-openapi.yml
  format: yaml
  label: Nacelle Checkout API
  slug: nacelle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-checkout-api-openapi.yml
- filename: nacelle-credentials-api-openapi.yml
  format: yaml
  label: Nacelle Credentials API
  slug: nacelle-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-credentials-api-openapi.yml
- filename: nacelle-customers-api-openapi.yml
  format: yaml
  label: Nacelle Customers API
  slug: nacelle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-customers-api-openapi.yml
- filename: nacelle-entries-alpha-api-openapi.yml
  format: yaml
  label: Nacelle entries (ALPHA) API
  slug: nacelle-entries-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-alpha-api-openapi.yml
- filename: nacelle-entries-api-openapi.yml
  format: yaml
  label: Nacelle Entries API
  slug: nacelle-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-api-openapi.yml
- filename: nacelle-entries-beta-api-openapi.yml
  format: yaml
  label: Nacelle entries (BETA) API
  slug: nacelle-entries-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-beta-api-openapi.yml
- filename: nacelle-fulfillments-api-openapi.yml
  format: yaml
  label: Nacelle Fulfillments API
  slug: nacelle-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-fulfillments-api-openapi.yml
- filename: nacelle-index-api-openapi.yml
  format: yaml
  label: Nacelle Index API
  slug: nacelle-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-index-api-openapi.yml
- filename: nacelle-multiorders-api-openapi.yml
  format: yaml
  label: Nacelle Multiorders API
  slug: nacelle-multiorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-multiorders-api-openapi.yml
- filename: nacelle-orderitems-api-openapi.yml
  format: yaml
  label: Nacelle Orderitems API
  slug: nacelle-orderitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-orderitems-api-openapi.yml
- filename: nacelle-payment-api-openapi.yml
  format: yaml
  label: Nacelle Payment API
  slug: nacelle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-payment-api-openapi.yml
- filename: nacelle-paymentintent-api-openapi.yml
  format: yaml
  label: Nacelle Paymentintent API
  slug: nacelle-paymentintent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-paymentintent-api-openapi.yml
- filename: nacelle-token-api-openapi.yml
  format: yaml
  label: Nacelle Token API
  slug: nacelle-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-token-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Nacelle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nacelle publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nacelle API on a user''s behalf.


  Tokens are issued from https://authimilate.api.nacelle.com/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nacelle
provider_slug: nacelle
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://authimilate.api.nacelle.com/v1/token
  name: oauth2
  source: openapi/nacelle-auth-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://authimilate.api.nacelle.com/v1/token
  name: oauth2
  source: openapi/nacelle-order-management-api-experimental-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Grants read access
  flows:
  - clientCredentials
  scope: read
- description: Grants write access
  flows:
  - clientCredentials
  scope: write
slug: nacelle-scopes
source_filename: nacelle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/nacelle-auth-api-openapi.yml, openapi/nacelle-order-management-api-experimental-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/nacelle-auth-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authimilate.api.nacelle.com/v1/token\n- name: oauth2\n  source: openapi/nacelle-order-management-api-experimental-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://authimilate.api.nacelle.com/v1/token\nscopes:\n- scope: read\n  description: Grants read access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/nacelle-auth-api-openapi.yml\n  - openapi/nacelle-order-management-api-experimental-openapi.yml\n- scope: write\n  description: Grants write access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/nacelle-auth-api-openapi.yml\n  - openapi/nacelle-order-management-api-experimental-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/scopes/nacelle-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- GraphQL
- Content
- Data Indexing
token_bound: false
token_urls:
- https://authimilate.api.nacelle.com/v1/token
---
