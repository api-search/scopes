---
api_specs:
- filename: banksapi-openapi-generated.yml
  format: yaml
  label: fineconomy API
  slug: banksapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/banksapi/openapi/_ae-authored/banksapi-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Banksapi Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'fineconomy publishes 5 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the fineconomy API on a user''s behalf.


  Tokens are issued from /auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: fineconomy
provider_slug: banksapi
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /auth/oauth2/token
  name: OAuth2
  source: openapi/banksapi-openapi-generated.yml
scope_count: 5
scope_names:
- auth/tenants/users/create
- http://banksapi.io/customer/modify
- http://banksapi.io/customer/read
- http://banksapi.io/customer/ueberweisung
- http://banksapi.io/provider/read
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: auth/tenants/users/create
- description: ''
  flows:
  - clientCredentials
  scope: http://banksapi.io/customer/modify
- description: ''
  flows:
  - clientCredentials
  scope: http://banksapi.io/customer/read
- description: ''
  flows:
  - clientCredentials
  scope: http://banksapi.io/customer/ueberweisung
- description: ''
  flows:
  - clientCredentials
  scope: http://banksapi.io/provider/read
slug: banksapi-scopes
source_filename: banksapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/banksapi-openapi-generated.yml\nschemes:\n- name: OAuth2\n  source: openapi/banksapi-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/oauth2/token\nscopes:\n- scope: auth/tenants/users/create\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/banksapi-openapi-generated.yml\n- scope: http://banksapi.io/customer/modify\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/banksapi-openapi-generated.yml\n- scope: http://banksapi.io/customer/read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/banksapi-openapi-generated.yml\n- scope: http://banksapi.io/customer/ueberweisung\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/banksapi-openapi-generated.yml\n- scope: http://banksapi.io/provider/read\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/banksapi-openapi-generated.yml\n"
source_yaml_url: https://artifacts.apis.io/banksapi/scopes/banksapi-scopes.yml
summary_line: 5 scopes · clientCredentials
tags:
- Banking
- API
- FinTech
- Payments
- DataAnalytics
token_bound: false
token_urls:
- /auth/oauth2/token
---
