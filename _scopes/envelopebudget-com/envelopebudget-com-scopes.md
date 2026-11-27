---
api_specs:
- filename: envelopebudget-com-accounts-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Accounts API
  slug: envelopebudget-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-accounts-api-openapi.yml
- filename: envelopebudget-com-auth-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Auth API
  slug: envelopebudget-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-auth-api-openapi.yml
- filename: envelopebudget-com-envelopes-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Envelopes API
  slug: envelopebudget-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-envelopes-api-openapi.yml
- filename: envelopebudget-com-transactions-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Transactions API
  slug: envelopebudget-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-transactions-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: EnvelopeBudget Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'EnvelopeBudget uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: EnvelopeBudget
provider_slug: envelopebudget-com
schemes:
- flows:
  - flow: password
    tokenUrl: token
  name: OAuth2PasswordBearer
  source: openapi/envelopebudget-com-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: envelopebudget-com-scopes
source_filename: envelopebudget-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: none\nsource: openapi/envelopebudget-com-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/envelopebudget-com-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/envelopebudget-com/scopes/envelopebudget-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Finance
- Budgeting
- Personal Finance
- Couples
- Families
token_bound: false
token_urls:
- token
---
