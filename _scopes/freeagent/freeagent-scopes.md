---
api_specs:
- filename: postman-freeagent-api-collection
  format: yaml
  label: FreeAgent REST API
  slug: rest-api
  spec_type: Postman
  url: https://github.com/fac/postman-freeagent-api-collection
- filename: freeagent-contacts-api-openapi.yml
  format: yaml
  label: FreeAgent Contacts API
  slug: freeagent-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/openapi/freeagent-contacts-api-openapi.yml
- filename: freeagent-invoices-api-openapi.yml
  format: yaml
  label: FreeAgent Invoices API
  slug: freeagent-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/openapi/freeagent-invoices-api-openapi.yml
- filename: freeagent-bank-accounts-api-openapi.yml
  format: yaml
  label: FreeAgent Bank Accounts API
  slug: freeagent-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/openapi/freeagent-bank-accounts-api-openapi.yml
authorization_urls:
- https://api.freeagent.com/v2/approve_app
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Freeagent Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'FreeAgent uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.freeagent.com/v2/token_endpoint.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FreeAgent
provider_slug: freeagent
schemes:
- description: 'OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;

    refresh tokens used to obtain new access tokens.'
  flows:
  - authorizationUrl: https://api.freeagent.com/v2/approve_app
    flow: authorizationCode
    tokenUrl: https://api.freeagent.com/v2/token_endpoint
  name: oauth2
  source: openapi/freeagent-bank-accounts-api-openapi.yml
- description: 'OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;

    refresh tokens used to obtain new access tokens.'
  flows:
  - authorizationUrl: https://api.freeagent.com/v2/approve_app
    flow: authorizationCode
    tokenUrl: https://api.freeagent.com/v2/token_endpoint
  name: oauth2
  source: openapi/freeagent-contacts-api-openapi.yml
- description: 'OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;

    refresh tokens used to obtain new access tokens.'
  flows:
  - authorizationUrl: https://api.freeagent.com/v2/approve_app
    flow: authorizationCode
    tokenUrl: https://api.freeagent.com/v2/token_endpoint
  name: oauth2
  source: openapi/freeagent-invoices-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: freeagent-scopes
source_filename: freeagent-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/freeagent-bank-accounts-api-openapi.yml, openapi/freeagent-contacts-api-openapi.yml,\n  openapi/freeagent-invoices-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/freeagent-bank-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freeagent.com/v2/approve_app\n    tokenUrl: https://api.freeagent.com/v2/token_endpoint\n  description: |-\n    OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;\n    refresh tokens used to obtain new access tokens.\n- name: oauth2\n  source: openapi/freeagent-contacts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freeagent.com/v2/approve_app\n    tokenUrl: https://api.freeagent.com/v2/token_endpoint\n  description: |-\n    OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;\n    refresh tokens used to obtain new access tokens.\n- name: oauth2\n  source: openapi/freeagent-invoices-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.freeagent.com/v2/approve_app\n    tokenUrl: https://api.freeagent.com/v2/token_endpoint\n  description: |-\n    OAuth 2.0 authorization code flow. Access tokens valid for ~1 hour;\n    refresh tokens used to obtain new access tokens.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeagent/refs/heads/main/scopes/freeagent-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Accounting
- Small Business
- Invoicing
- Bookkeeping
- Expenses
- Payroll
- VAT
- HMRC
- Making Tax Digital
token_bound: false
token_urls:
- https://api.freeagent.com/v2/token_endpoint
---
