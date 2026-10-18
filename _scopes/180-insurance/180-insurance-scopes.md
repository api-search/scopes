---
api_specs:
- filename: 180-insurance-cota-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Cotações API
  slug: 180-insurance-cota-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-cota-es-api-openapi.yml
- filename: 180-insurance-produtos-api-openapi.yml
  format: yaml
  label: 180 Insurance Produtos API
  slug: 180-insurance-produtos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-produtos-api-openapi.yml
- filename: 180-insurance-propostas-api-openapi.yml
  format: yaml
  label: 180 Insurance Propostas API
  slug: 180-insurance-propostas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-propostas-api-openapi.yml
- filename: 180-insurance-renova-es-api-openapi.yml
  format: yaml
  label: 180 Insurance Renovações API
  slug: 180-insurance-renova-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-renova-es-api-openapi.yml
- filename: 180-insurance-sinistros-api-openapi.yml
  format: yaml
  label: 180 Insurance Sinistros API
  slug: 180-insurance-sinistros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-sinistros-api-openapi.yml
- filename: 180-insurance-vendas-api-openapi.yml
  format: yaml
  label: 180 Insurance Vendas API
  slug: 180-insurance-vendas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-vendas-api-openapi.yml
- filename: 180-insurance-webhooks-api-openapi.yml
  format: yaml
  label: 180 Insurance Webhooks API
  slug: 180-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/openapi/180-insurance-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: 180 Insurance Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: '180 Insurance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://180s-staging.us.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 180 Insurance
provider_slug: 180-insurance
schemes:
- description: Adicione client_id e client_secret para obter um token válido.
  flows:
  - flow: clientCredentials
    tokenUrl: https://180s-staging.us.auth0.com/oauth/token
  name: oauth
  source: openapi/180-insurance-sagas-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: 180-insurance-scopes
source_filename: 180-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/180-insurance-sagas-api-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/180-insurance-sagas-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://180s-staging.us.auth0.com/oauth/token\n  description: Adicione client_id e client_secret para obter um token válido.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/180-insurance/refs/heads/main/scopes/180-insurance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Insurtech
- Insurance
- Embedded Insurance
- Brazil
- Fintech
- Webhook
token_bound: false
token_urls:
- https://180s-staging.us.auth0.com/oauth/token
---
