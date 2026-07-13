---
api_specs:
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Shops API
  slug: tekmetric-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Customers API
  slug: tekmetric-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Vehicles API
  slug: tekmetric-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Repair Orders API
  slug: tekmetric-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Jobs API
  slug: tekmetric-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Employees API
  slug: tekmetric-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Appointments API
  slug: tekmetric-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Inventory API
  slug: tekmetric-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Canned Jobs API
  slug: tekmetric-canned-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
authorization_urls: []
description: ''
docs: https://api.tekmetric.com
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tekmetric Scopes
name_suffix: OAuth Scopes
note: Tekmetric does not publish OAuth permission scopes - the API uses an OAuth 2.0 client credentials grant behind a partner approval gate (https://api.tekmetric.com), and the token response's scope field carries the space-separated Shop IDs the client is authorized for rather than permission scopes.
overview: 'Tekmetric uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://shop.tekmetric.com/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tekmetric
provider_slug: tekmetric
schemes:
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: tekmetric-scopes
source_filename: tekmetric-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tekmetric-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/tekmetric-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\ndocs: https://api.tekmetric.com\nnote: Tekmetric does not publish OAuth permission scopes - the API uses an OAuth 2.0\n  client credentials grant behind a partner approval gate (https://api.tekmetric.com),\n  and the token response's scope field carries the space-separated Shop IDs the client\n  is authorized for rather than permission scopes.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/scopes/tekmetric-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automotive
- Auto Repair
- Shop Management
- Fleet
- Vertical SaaS
token_urls:
- https://shop.tekmetric.com/api/v1/oauth/token
---
