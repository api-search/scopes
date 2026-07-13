---
api_specs:
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Sales Orders API
  slug: fulfil-io-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Products & Variants API
  slug: fulfil-io-products-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Inventory & Stock API
  slug: fulfil-io-inventory-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Customers API
  slug: fulfil-io-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Shipments API
  slug: fulfil-io-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Purchases API
  slug: fulfil-io-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Manufacturing API
  slug: fulfil-io-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Webhooks API
  slug: fulfil-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
- filename: fulfil-io-openapi.yml
  format: yaml
  label: Fulfil Model Interface API
  slug: fulfil-io-model-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/openapi/fulfil-io-openapi.yml
authorization_urls:
- https://{merchant_id}.fulfil.io/oauth/authorize
description: ''
docs: https://developers.fulfil.io/rest_api/oauth/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Fulfil Io Scopes
name_suffix: OAuth Scopes
note: Fulfil documents an OAuth 2.0 authorization code flow with scopes passed as a comma-separated list, but does not publish a complete public scopes reference - the current OAuth docs (https://developers.fulfil.io/rest_api/oauth/) redirect to a workspace login; only the scopes shown in the official OAuth guide (archived) and the official fulfil-python-api client examples are recorded here, which follow a model:permission pattern (e.g. sale.channel:read) plus offline_access as an access_type for offline tokens.
overview: 'Fulfil publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fulfil API on a user''s behalf.


  Tokens are issued from https://{merchant_id}.fulfil.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fulfil
provider_slug: fulfil-io
schemes:
- description: OAuth 2.0 authorization code flow for public apps.
  flows:
  - authorizationUrl: https://{merchant_id}.fulfil.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://{merchant_id}.fulfil.io/oauth/token
  name: oauth2
  source: openapi/fulfil-io-openapi.yml
scope_count: 2
scope_names:
- user_session
- sale.channel:read
scopes:
- description: Grants an API session acting on behalf of the authorizing user; shown as the granted scope in the OAuth token response example in Fulfil's official OAuth guide and used in the official Python client's OAuth session example.
  flows: []
  scope: user_session
- description: Read access to the sale.channel model; used in Fulfil's official headless offline-access example, illustrating the model:permission scope pattern Fulfil uses for granting access to individual ERP models.
  flows: []
  scope: sale.channel:read
slug: fulfil-io-scopes
source_filename: fulfil-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/fulfil-io-openapi.yml\ndocs: https://developers.fulfil.io/rest_api/oauth/\nnote: Fulfil documents an OAuth 2.0 authorization code flow with scopes passed as a\n  comma-separated list, but does not publish a complete public scopes reference -\n  the current OAuth docs (https://developers.fulfil.io/rest_api/oauth/) redirect to\n  a workspace login; only the scopes shown in the official OAuth guide (archived)\n  and the official fulfil-python-api client examples are recorded here, which follow\n  a model:permission pattern (e.g. sale.channel:read) plus offline_access as an\n  access_type for offline tokens.\nschemes:\n- name: oauth2\n  source: openapi/fulfil-io-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{merchant_id}.fulfil.io/oauth/authorize\n    tokenUrl: https://{merchant_id}.fulfil.io/oauth/token\n  description: OAuth 2.0 authorization code flow for public apps.\nscopes:\n- scope:\
  \ user_session\n  description: Grants an API session acting on behalf of the authorizing user; shown\n    as the granted scope in the OAuth token response example in Fulfil's official\n    OAuth guide and used in the official Python client's OAuth session example.\n  sources:\n  - https://web.archive.org/web/20190308042755/http://developers.fulfil.io/getting-started/oauth2.html\n  - https://github.com/fulfilio/fulfil-python-api\n- scope: sale.channel:read\n  description: Read access to the sale.channel model; used in Fulfil's official\n    headless offline-access example, illustrating the model:permission scope pattern\n    Fulfil uses for granting access to individual ERP models.\n  sources:\n  - https://web.archive.org/web/20190308042755/http://developers.fulfil.io/getting-started/oauth2.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fulfil-io/refs/heads/main/scopes/fulfil-io-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- ERP
- E-commerce
- Order Management
- Inventory
- Warehouse Management
- Manufacturing
- Operations
token_urls:
- https://{merchant_id}.fulfil.io/oauth/token
---
