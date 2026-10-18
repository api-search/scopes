---
api_specs:
- filename: loggi-authapi-api-openapi.yml
  format: yaml
  label: Loggi Auth API
  slug: loggi-authapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-authapi-api-openapi.yml
- filename: loggi-detailsapi-api-openapi.yml
  format: yaml
  label: Loggi Details API
  slug: loggi-detailsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-detailsapi-api-openapi.yml
- filename: loggi-dropofflocationsapi-api-openapi.yml
  format: yaml
  label: Loggi Dropoff Locations API
  slug: loggi-dropofflocationsapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-dropofflocationsapi-api-openapi.yml
- filename: loggi-integratorcompanyapi-api-openapi.yml
  format: yaml
  label: Loggi Integrator Company API
  slug: loggi-integratorcompanyapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-integratorcompanyapi-api-openapi.yml
- filename: loggi-labelapi-api-openapi.yml
  format: yaml
  label: Loggi Label API
  slug: loggi-labelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-labelapi-api-openapi.yml
- filename: loggi-packagecancelapi-api-openapi.yml
  format: yaml
  label: Loggi Package Cancel API
  slug: loggi-packagecancelapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packagecancelapi-api-openapi.yml
- filename: loggi-packageupdateapi-api-openapi.yml
  format: yaml
  label: Loggi Package Update API
  slug: loggi-packageupdateapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-packageupdateapi-api-openapi.yml
- filename: loggi-quotationapi-api-openapi.yml
  format: yaml
  label: Loggi Quotation API
  slug: loggi-quotationapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-quotationapi-api-openapi.yml
- filename: loggi-shipmentapi-api-openapi.yml
  format: yaml
  label: Loggi Shipment API
  slug: loggi-shipmentapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-shipmentapi-api-openapi.yml
- filename: loggi-trackingapi-api-openapi.yml
  format: yaml
  label: Loggi Tracking API
  slug: loggi-trackingapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/openapi/loggi-trackingapi-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Loggi Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Loggi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.loggi.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Loggi
provider_slug: loggi
schemes:
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-freight-price-quotation-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-integrator-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: oauth2/token
  name: OAuth2
  source: openapi/loggi-labels-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-package-details-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-package-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-pontos-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-shipments-openapi.yml
- description: Autenticação OAuth 2.0 para clientes da API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.loggi.com/oauth2/token
  name: OAuth2
  source: openapi/loggi-tracking-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: loggi-scopes
source_filename: loggi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/loggi-freight-price-quotation-openapi.yml, openapi/loggi-integrator-openapi.yml,\n  openapi/loggi-labels-openapi.yml, openapi/loggi-package-details-openapi.yml, openapi/loggi-package-openapi.yml,\n  openapi/loggi-pontos-openapi.yml, openapi/loggi-shipments-openapi.yml, openapi/loggi-tracking-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/loggi-freight-price-quotation-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-integrator-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-labels-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: oauth2/token\n  description: Autenticação OAuth 2.0 para clientes\
  \ da API.\n- name: OAuth2\n  source: openapi/loggi-package-details-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-package-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-pontos-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-shipments-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n  description: Autenticação OAuth 2.0 para clientes da API.\n- name: OAuth2\n  source: openapi/loggi-tracking-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.loggi.com/oauth2/token\n\
  \  description: Autenticação OAuth 2.0 para clientes da API.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loggi/refs/heads/main/scopes/loggi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Logistics
- Shipping
- Last Mile Delivery
- Freight
- Tracking
- Brazil
token_bound: false
token_urls:
- https://api.loggi.com/oauth2/token
- oauth2/token
---
