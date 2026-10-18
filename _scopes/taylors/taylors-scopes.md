---
api_specs:
- filename: taylors-patrons-api-openapi.yml
  format: yaml
  label: Taylor's Library Koha REST API
  slug: library-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/openapi/taylors-patrons-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Taylors Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Taylor''s University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://librarycatalogue.taylors.edu.my/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Taylor's University
provider_slug: taylors
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-checkouts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-holds-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-item-types-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-items-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-libraries-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
  name: oauth2ClientCredentials
  source: openapi/taylors-patrons-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: taylors-scopes
source_filename: taylors-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/taylors-checkouts-api-openapi.yml, openapi/taylors-holds-api-openapi.yml, openapi/taylors-item-types-api-openapi.yml,\n  openapi/taylors-items-api-openapi.yml, openapi/taylors-libraries-api-openapi.yml, openapi/taylors-patrons-api-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/taylors-checkouts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/taylors-holds-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/taylors-item-types-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/taylors-items-api-openapi.yml\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/taylors-libraries-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\n- name: oauth2ClientCredentials\n  source: openapi/taylors-patrons-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://librarycatalogue.taylors.edu.my/api/v1/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylors/refs/heads/main/scopes/taylors-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Education
- Higher Education
- University
- Private University
- Malaysia
- Asia
- Library
- Library Catalog
- Institutional Repository
- Research Data
- OAI-PMH
- Identity Federation
- Koha
- DSpace
token_bound: false
token_urls:
- https://librarycatalogue.taylors.edu.my/api/v1/oauth/token
---
