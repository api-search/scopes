---
api_specs:
- filename: paigo-customers-api-openapi.yml
  format: yaml
  label: Paigo Customers API
  slug: paigo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-customers-api-openapi.yml
- filename: paigo-dimensions-api-openapi.yml
  format: yaml
  label: Paigo Dimensions API
  slug: paigo-dimensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-dimensions-api-openapi.yml
- filename: paigo-invoices-api-openapi.yml
  format: yaml
  label: Paigo Invoices API
  slug: paigo-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-invoices-api-openapi.yml
- filename: paigo-measurements-api-openapi.yml
  format: yaml
  label: Paigo Measurements API
  slug: paigo-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-measurements-api-openapi.yml
- filename: paigo-offerings-api-openapi.yml
  format: yaml
  label: Paigo Offerings API
  slug: paigo-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-offerings-api-openapi.yml
- filename: paigo-settings-api-openapi.yml
  format: yaml
  label: Paigo Settings API
  slug: paigo-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-settings-api-openapi.yml
- filename: paigo-usage-api-openapi.yml
  format: yaml
  label: Paigo Usage API
  slug: paigo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-usage-api-openapi.yml
- filename: paigo-webhooks-api-openapi.yml
  format: yaml
  label: Paigo Webhooks API
  slug: paigo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/openapi/paigo-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Paigo Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Paigo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.paigo.tech/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Paigo
provider_slug: paigo
schemes:
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-customers-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-dimensions-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-invoices-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-measurements-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-offerings-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-settings-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-usage-api-openapi.yml
- description: Use bearer token to authenticate `Bearer <your access token>`
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.paigo.tech/oauth/token
  name: bearer
  source: openapi/paigo-webhooks-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: paigo-scopes
source_filename: paigo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/paigo-customers-api-openapi.yml, openapi/paigo-dimensions-api-openapi.yml, openapi/paigo-invoices-api-openapi.yml,\n  openapi/paigo-measurements-api-openapi.yml, openapi/paigo-offerings-api-openapi.yml, openapi/paigo-settings-api-openapi.yml,\n  openapi/paigo-usage-api-openapi.yml, openapi/paigo-webhooks-api-openapi.yml\nschemes:\n- name: bearer\n  source: openapi/paigo-customers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-dimensions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-invoices-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n\
  \  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-measurements-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-offerings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-settings-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\n- name: bearer\n  source: openapi/paigo-usage-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your\
  \ access token>`\n- name: bearer\n  source: openapi/paigo-webhooks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.paigo.tech/oauth/token\n  description: Use bearer token to authenticate `Bearer <your access token>`\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/scopes/paigo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Billing
- Usage-Based Billing
- Metering
- Invoicing
- Pricing
- Software-as-a-Service
- Subscription
- Developer Tools
- FinOps
token_bound: false
token_urls:
- https://auth.paigo.tech/oauth/token
---
