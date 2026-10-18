---
api_specs:
- filename: pomelo-authentication-api-openapi.yml
  format: yaml
  label: Pomelo Authentication API
  slug: pomelo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-authentication-api-openapi.yml
- filename: pomelo-card-accounts-api-openapi.yml
  format: yaml
  label: Pomelo Card Accounts API
  slug: pomelo-card-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-card-accounts-api-openapi.yml
- filename: pomelo-cards-api-openapi.yml
  format: yaml
  label: Pomelo Cards API
  slug: pomelo-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-cards-api-openapi.yml
- filename: pomelo-transactions-api-openapi.yml
  format: yaml
  label: Pomelo Transactions API
  slug: pomelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-transactions-api-openapi.yml
- filename: pomelo-transfers-api-openapi.yml
  format: yaml
  label: Pomelo Transfers API
  slug: pomelo-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-transfers-api-openapi.yml
- filename: pomelo-users-api-openapi.yml
  format: yaml
  label: Pomelo Users API
  slug: pomelo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/openapi/pomelo-users-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Pomelo Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Pomelo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.pomelo.la/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pomelo
provider_slug: pomelo
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-authentication-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-card-accounts-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-cards-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-transactions-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-transfers-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.pomelo.la/oauth/token
  name: oauth2
  source: openapi/pomelo-users-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: pomelo-scopes
source_filename: pomelo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/pomelo-authentication-api-openapi.yml, openapi/pomelo-card-accounts-api-openapi.yml,\n  openapi/pomelo-cards-api-openapi.yml, openapi/pomelo-transactions-api-openapi.yml, openapi/pomelo-transfers-api-openapi.yml,\n  openapi/pomelo-users-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pomelo-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n- name: oauth2\n  source: openapi/pomelo-card-accounts-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n- name: oauth2\n  source: openapi/pomelo-cards-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n- name: oauth2\n  source: openapi/pomelo-transactions-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n- name: oauth2\n  source: openapi/pomelo-transfers-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\n- name: oauth2\n  source: openapi/pomelo-users-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.pomelo.la/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pomelo/refs/heads/main/scopes/pomelo-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Fintech
- Card Issuing
- Embedded Finance
- Payments
- Latin America
token_bound: false
token_urls:
- https://auth.pomelo.la/oauth/token
---
