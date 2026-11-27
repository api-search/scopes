---
api_specs:
- filename: obraaberta-com-br-construtoras-api-openapi.yml
  format: yaml
  label: ObraAberta Construtoras API
  slug: obraaberta-com-br-construtoras-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-construtoras-api-openapi.yml
- filename: obraaberta-com-br-dados-api-openapi.yml
  format: yaml
  label: ObraAberta Dados API
  slug: obraaberta-com-br-dados-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-dados-api-openapi.yml
- filename: obraaberta-com-br-metabuscador-api-openapi.yml
  format: yaml
  label: ObraAberta Metabuscador API
  slug: obraaberta-com-br-metabuscador-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-metabuscador-api-openapi.yml
- filename: obraaberta-com-br-partner-api-api-openapi.yml
  format: yaml
  label: ObraAberta Partner API
  slug: obraaberta-com-br-partner-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-partner-api-api-openapi.yml
- filename: obraaberta-com-br-projetos-api-openapi.yml
  format: yaml
  label: ObraAberta Projetos API
  slug: obraaberta-com-br-projetos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-projetos-api-openapi.yml
- filename: obraaberta-com-br-sistema-api-openapi.yml
  format: yaml
  label: ObraAberta Sistema API
  slug: obraaberta-com-br-sistema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-sistema-api-openapi.yml
- filename: obraaberta-com-br-transpar-ncia-condominial-api-openapi.yml
  format: yaml
  label: ObraAberta Transparência condominial API
  slug: obraaberta-com-br-transpar-ncia-condominial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obraaberta-com-br/openapi/obraaberta-com-br-transpar-ncia-condominial-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: ObraAberta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ObraAberta publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ObraAberta API on a user''s behalf.


  Tokens are issued from https://obraaberta.com.br/api/v1/partners/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ObraAberta
provider_slug: obraaberta-com-br
schemes:
- description: OAuth 2.0 Client Credentials para a Partner API sandbox.
  flows:
  - flow: clientCredentials
    tokenUrl: https://obraaberta.com.br/api/v1/partners/oauth/token
  name: partnerOAuth2
  source: openapi/obraaberta-com-br-openapi.yml
scope_count: 2
scope_names:
- catalog:read
- catalog:write
scopes:
- description: Consultar produtos, lotes e erros do próprio parceiro.
  flows:
  - clientCredentials
  scope: catalog:read
- description: Validar, inserir ou desativar produtos na sandbox.
  flows:
  - clientCredentials
  scope: catalog:write
slug: obraaberta-com-br-scopes
source_filename: obraaberta-com-br-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/obraaberta-com-br-openapi.yml\nschemes:\n- name: partnerOAuth2\n  source: openapi/obraaberta-com-br-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://obraaberta.com.br/api/v1/partners/oauth/token\n  description: OAuth 2.0 Client Credentials para a Partner API sandbox.\nscopes:\n- scope: catalog:read\n  description: Consultar produtos, lotes e erros do próprio parceiro.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n- scope: catalog:write\n  description: Validar, inserir ou desativar produtos na sandbox.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/obraaberta-com-br-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/obraaberta-com-br/scopes/obraaberta-com-br-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Construction
- Transparency
- Brazil
- Real Estate
- Public Data
token_bound: false
token_urls:
- https://obraaberta.com.br/api/v1/partners/oauth/token
---
