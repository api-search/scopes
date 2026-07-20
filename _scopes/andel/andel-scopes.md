---
api_specs:
- filename: andel-data-exchange-openapi.yaml
  format: yaml
  label: Data Exchange API
  slug: data-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/openapi/andel-data-exchange-openapi.yaml
authorization_urls: []
description: ''
docs: https://build.andel.org/dataexchange/overview/overview
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Andel Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Andel publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Andel API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Andel
provider_slug: andel
schemes:
- grant: clientCredentials
  name: andelDescopeClientCredentials
  token_url: https://api.descope.com/oauth2/v1/apps/token
scope_count: 1
scope_names:
- purchases:read
scopes:
- description: Read access to member purchase events on the Data Exchange API. Required to call GET /purchases and GET /purchases/{purchase_id}. Tokens additionally carry a `plans` claim that scopes visibility to the plans the tenant is authorized for.
  flows: []
  scope: purchases:read
slug: andel-scopes
source_filename: andel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/andel-data-exchange-openapi.yaml\ndocs: https://build.andel.org/dataexchange/overview/overview\nissuer: Descope\ntoken_url: https://api.descope.com/oauth2/v1/apps/token\nschemes:\n- name: andelDescopeClientCredentials\n  grant: clientCredentials\n  token_url: https://api.descope.com/oauth2/v1/apps/token\nscopes:\n- scope: purchases:read\n  description: >-\n    Read access to member purchase events on the Data Exchange API. Required to\n    call GET /purchases and GET /purchases/{purchase_id}. Tokens additionally\n    carry a `plans` claim that scopes visibility to the plans the tenant is\n    authorized for.\n  grants:\n  - clientCredentials\n  operations:\n  - listPurchases\n  - getPurchase\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/scopes/andel-scopes.yml
summary_line: 1 scope
tags:
- Company
- Healthcare
- Pharmacy
- Pharmacy Benefits
- Drug Pricing
- Specialty Medications
- Data Exchange
- Webhooks
token_urls: []
---
