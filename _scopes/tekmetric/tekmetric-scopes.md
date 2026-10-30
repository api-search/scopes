---
api_specs:
- filename: tekmetric-appointments-api-openapi.yml
  format: yaml
  label: Tekmetric Appointments API
  slug: tekmetric-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-appointments-api-openapi.yml
- filename: tekmetric-canned-jobs-api-openapi.yml
  format: yaml
  label: Tekmetric Canned Jobs API
  slug: tekmetric-canned-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-canned-jobs-api-openapi.yml
- filename: tekmetric-customers-api-openapi.yml
  format: yaml
  label: Tekmetric Customers API
  slug: tekmetric-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-customers-api-openapi.yml
- filename: tekmetric-employees-api-openapi.yml
  format: yaml
  label: Tekmetric Employees API
  slug: tekmetric-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-employees-api-openapi.yml
- filename: tekmetric-inventory-api-openapi.yml
  format: yaml
  label: Tekmetric Inventory API
  slug: tekmetric-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-inventory-api-openapi.yml
- filename: tekmetric-jobs-api-openapi.yml
  format: yaml
  label: Tekmetric Jobs API
  slug: tekmetric-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-jobs-api-openapi.yml
- filename: tekmetric-repair-orders-api-openapi.yml
  format: yaml
  label: Tekmetric Repair Orders API
  slug: tekmetric-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-repair-orders-api-openapi.yml
- filename: tekmetric-shops-api-openapi.yml
  format: yaml
  label: Tekmetric Shops API
  slug: tekmetric-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-shops-api-openapi.yml
- filename: tekmetric-vehicles-api-openapi.yml
  format: yaml
  label: Tekmetric Vehicles API
  slug: tekmetric-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-vehicles-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Tekmetric Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/tekmetric-appointments-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-canned-jobs-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-customers-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-employees-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-inventory-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-jobs-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-repair-orders-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-shops-api-openapi.yml
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  source: openapi/tekmetric-vehicles-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: tekmetric-scopes
source_filename: tekmetric-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/tekmetric-appointments-api-openapi.yml, openapi/tekmetric-canned-jobs-api-openapi.yml,\n  openapi/tekmetric-customers-api-openapi.yml, openapi/tekmetric-employees-api-openapi.yml,\n  openapi/tekmetric-inventory-api-openapi.yml, openapi/tekmetric-jobs-api-openapi.yml, openapi/tekmetric-repair-orders-api-openapi.yml,\n  openapi/tekmetric-shops-api-openapi.yml, openapi/tekmetric-vehicles-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/tekmetric-appointments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-canned-jobs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n\
  \  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-customers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-employees-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-inventory-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-jobs-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-repair-orders-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-shops-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n- name: oauth2\n  source: openapi/tekmetric-vehicles-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/scopes/tekmetric-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Automotive
- Auto Repair
- Shop Management
- Fleet Management
- Vertical SaaS
token_bound: false
token_urls:
- https://shop.tekmetric.com/api/v1/oauth/token
---
