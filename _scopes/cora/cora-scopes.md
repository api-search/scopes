---
api_specs:
- filename: cora-balance-api-openapi.yml
  format: yaml
  label: Cora Balance API
  slug: cora-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-balance-api-openapi.yml
- filename: cora-banks-api-openapi.yml
  format: yaml
  label: Cora Banks API
  slug: cora-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-banks-api-openapi.yml
- filename: cora-boletos-v2-api-openapi.yml
  format: yaml
  label: Cora Boletos V2 API
  slug: cora-boletos-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-boletos-v2-api-openapi.yml
- filename: cora-businesses-api-openapi.yml
  format: yaml
  label: Cora Businesses API
  slug: cora-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-businesses-api-openapi.yml
- filename: cora-credentials-api-openapi.yml
  format: yaml
  label: Cora Credentials API
  slug: cora-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-credentials-api-openapi.yml
- filename: cora-dados-de-conta-api-openapi.yml
  format: yaml
  label: Cora Dados De Conta API
  slug: cora-dados-de-conta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-dados-de-conta-api-openapi.yml
- filename: cora-initiate-api-openapi.yml
  format: yaml
  label: Cora Initiate API
  slug: cora-initiate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-initiate-api-openapi.yml
- filename: cora-issuer-api-openapi.yml
  format: yaml
  label: Cora Issuer API
  slug: cora-issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-issuer-api-openapi.yml
- filename: cora-notifica-es-api-openapi.yml
  format: yaml
  label: Cora Notificações API
  slug: cora-notifica-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-notifica-es-api-openapi.yml
- filename: cora-notifications-api-openapi.yml
  format: yaml
  label: Cora Notifications API
  slug: cora-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-notifications-api-openapi.yml
- filename: cora-pagamento-de-impostos-api-openapi.yml
  format: yaml
  label: Cora Pagamento De Impostos API
  slug: cora-pagamento-de-impostos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-pagamento-de-impostos-api-openapi.yml
- filename: cora-pay-api-openapi.yml
  format: yaml
  label: Cora Pay API
  slug: cora-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-pay-api-openapi.yml
- filename: cora-service-receipt-api-openapi.yml
  format: yaml
  label: Cora Service Receipt API
  slug: cora-service-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-service-receipt-api-openapi.yml
- filename: cora-statement-api-openapi.yml
  format: yaml
  label: Cora Statement API
  slug: cora-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/openapi/cora-statement-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: none
name: Cora Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Cora uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cora
provider_slug: cora
schemes:
- flows: []
  name: sec0
  source: openapi/cora-base-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-boletos-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-boletos-v2-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-dados-de-conta-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-extrato-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-nota-fiscal-de-servi-o-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-notifica-es-openapi.yml
- flows: []
  name: sec0
  source: openapi/cora-pagamento-de-impostos-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: cora-scopes
source_filename: cora-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/cora-base-openapi.yml, openapi/cora-boletos-openapi.yml, openapi/cora-boletos-v2-openapi.yml,\n  openapi/cora-dados-de-conta-openapi.yml, openapi/cora-extrato-openapi.yml, openapi/cora-nota-fiscal-de-servi-o-openapi.yml,\n  openapi/cora-notifica-es-openapi.yml, openapi/cora-pagamento-de-impostos-openapi.yml\nschemes:\n- name: sec0\n  source: openapi/cora-base-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-boletos-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-boletos-v2-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-dados-de-conta-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-extrato-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-nota-fiscal-de-servi-o-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-notifica-es-openapi.yml\n  flows: []\n- name: sec0\n  source: openapi/cora-pagamento-de-impostos-openapi.yml\n  flows: []\nscopes:\
  \ []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cora/refs/heads/main/scopes/cora-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Banking
- Brazil
- Payments
- Pix
- Boleto
- Invoicing
- Small Business
- Fintech
- Banking as a Service
token_bound: false
token_urls: []
---
