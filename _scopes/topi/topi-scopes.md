---
api_specs:
- filename: topi-seller-api-openapi-original.yaml
  format: yaml
  label: topi Seller API
  slug: topi-seller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-seller-api-openapi-original.yaml
authorization_urls: []
description: ''
docs: https://developer.topi.eu/docs/integration-guide/syncing-your-catalog
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Topi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Topi publishes 13 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Topi API on a user''s behalf.


  Tokens are issued from https://identity.topi.eu/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Topi
provider_slug: topi
schemes:
- description: Read our [Integration Guide](https://developer.topi.eu/docs/get-started/introduction) for detailed instructions on how to authenticate.
  flows:
  - flow: clientCredentials
    tokenUrl: https://identity.topi.eu/oauth2/token
  name: OAuth2Seller_header_Authorization
  source: openapi/topi-seller-api-openapi-original.yaml
scope_count: 13
scope_names:
- seller-branding:read
- seller-catalog:edit
- seller-catalog:read
- seller-metrics:read
- seller-offer:edit
- seller-offer:read
- seller-order:edit
- seller-order:read
- seller-scenario-simulations:run
- seller-shipment:edit
- seller-shipping-method:edit
- seller-shipping-method:read
- user-info:read
scopes:
- description: read seller branding config
  flows:
  - clientCredentials
  scope: seller-branding:read
- description: add product to catalog
  flows:
  - clientCredentials
  scope: seller-catalog:edit
- description: view and search catalog
  flows:
  - clientCredentials
  scope: seller-catalog:read
- description: read metrics urls
  flows:
  - clientCredentials
  scope: seller-metrics:read
- description: edit offer details
  flows:
  - clientCredentials
  scope: seller-offer:edit
- description: read offer details
  flows:
  - clientCredentials
  scope: seller-offer:read
- description: edit order details
  flows:
  - clientCredentials
  scope: seller-order:edit
- description: read order details
  flows:
  - clientCredentials
  scope: seller-order:read
- description: run scenario simulations
  flows:
  - clientCredentials
  scope: seller-scenario-simulations:run
- description: edit shipment details
  flows:
  - clientCredentials
  scope: seller-shipment:edit
- description: edit seller shipping method details
  flows:
  - clientCredentials
  scope: seller-shipping-method:edit
- description: read seller shipping method details
  flows:
  - clientCredentials
  scope: seller-shipping-method:read
- description: read user info
  flows:
  - clientCredentials
  scope: user-info:read
slug: topi-scopes
source_filename: topi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/topi-seller-api-openapi-original.yaml\ndocs: https://developer.topi.eu/docs/integration-guide/syncing-your-catalog\nschemes:\n- name: OAuth2Seller_header_Authorization\n  source: openapi/topi-seller-api-openapi-original.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://identity.topi.eu/oauth2/token\n  description: Read our [Integration Guide](https://developer.topi.eu/docs/get-started/introduction)\n    for detailed instructions on how to authenticate.\nscopes:\n- scope: seller-branding:read\n  description: read seller branding config\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-catalog:edit\n  description: add product to catalog\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-catalog:read\n  description: view and search catalog\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-metrics:read\n  description: read metrics urls\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-offer:edit\n  description: edit offer details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-offer:read\n  description: read offer details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-order:edit\n  description: edit order details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-order:read\n  description: read order details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-scenario-simulations:run\n  description: run scenario simulations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n\
  - scope: seller-shipment:edit\n  description: edit shipment details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-shipping-method:edit\n  description: edit seller shipping method details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: seller-shipping-method:read\n  description: read seller shipping method details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n- scope: user-info:read\n  description: read user info\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/topi-seller-api-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/scopes/topi-scopes.yml
summary_line: 13 scopes · clientCredentials
tags:
- Company
- Fintech
- Hardware as a Service
- Rental
- Embedded Finance
- B2B Payments
- Financing
- Checkout
- Germany
- API
token_urls:
- https://identity.topi.eu/oauth2/token
---
