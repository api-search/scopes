---
api_specs:
- filename: comunicate-eu-public-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.eu Public catalogue API
  slug: comunicate-eu-public-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-public-catalogue-api-openapi.yml
- filename: comunicate-eu-publications-api-openapi.yml
  format: yaml
  label: Comunicate.eu Publications API
  slug: comunicate-eu-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-publications-api-openapi.yml
- filename: comunicate-eu-writing-orders-api-openapi.yml
  format: yaml
  label: Comunicate.eu Writing orders API
  slug: comunicate-eu-writing-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-writing-orders-api-openapi.yml
- filename: comunicate-eu-articles-api-openapi.yml
  format: yaml
  label: Comunicate.eu Articles API
  slug: comunicate-eu-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-articles-api-openapi.yml
- filename: comunicate-eu-balance-and-reports-api-openapi.yml
  format: yaml
  label: Comunicate.eu Balance and reports API
  slug: comunicate-eu-balance-and-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-balance-and-reports-api-openapi.yml
- filename: comunicate-eu-campaigns-api-openapi.yml
  format: yaml
  label: Comunicate.eu Campaigns API
  slug: comunicate-eu-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-campaigns-api-openapi.yml
- filename: comunicate-eu-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.eu Catalogue API
  slug: comunicate-eu-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-catalogue-api-openapi.yml
- filename: comunicate-eu-checks-api-openapi.yml
  format: yaml
  label: Comunicate.eu Checks API
  slug: comunicate-eu-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-checks-api-openapi.yml
- filename: comunicate-eu-domain-audit-api-openapi.yml
  format: yaml
  label: Comunicate.eu Domain audit API
  slug: comunicate-eu-domain-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-domain-audit-api-openapi.yml
- filename: comunicate-eu-key-and-permissions-api-openapi.yml
  format: yaml
  label: Comunicate.eu Key and permissions API
  slug: comunicate-eu-key-and-permissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-key-and-permissions-api-openapi.yml
- filename: comunicate-eu-media-api-openapi.yml
  format: yaml
  label: Comunicate.eu Media API
  slug: comunicate-eu-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comunicate-eu/openapi/comunicate-eu-media-api-openapi.yml
authorization_urls:
- https://app.comunicate.eu/api/v1/oauth/authorize
description: ''
docs: https://comunicate.eu/ro/documentatie-api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Comunicate.eu Scopes
name_suffix: OAuth Scopes
note: Scope names match the docs "Permisiuni" section verbatim; descriptions are the docs Romanian text. The same scopes are attached to bk_live_ API keys when issued from Integrations.
overview: 'Comunicate.eu publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Comunicate.eu API on a user''s behalf.


  Tokens are issued from https://app.comunicate.eu/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Comunicate.eu
provider_slug: comunicate-eu
schemes:
- description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.eu/api/v1/oauth/register. The access token is an API key and is accepted everywhere an API key is.
  flows:
  - authorizationUrl: https://app.comunicate.eu/api/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.comunicate.eu/api/v1/oauth/token
  name: oauth2
  source: openapi/comunicate-eu-openapi.yml
scope_count: 10
scope_names:
- ARTICLES_READ
- ARTICLES_WRITE
- BALANCE_READ
- CAMPAIGNS_READ
- CAMPAIGNS_WRITE
- CATALOG_READ
- MEDIA_WRITE
- PUBLICATIONS_READ
- PUBLICATIONS_WRITE
- REPORTS_READ
scopes:
- description: articles read
  flows:
  - authorizationCode
  scope: ARTICLES_READ
- description: articles write
  flows:
  - authorizationCode
  scope: ARTICLES_WRITE
- description: balance read
  flows:
  - authorizationCode
  scope: BALANCE_READ
- description: campaigns read
  flows:
  - authorizationCode
  scope: CAMPAIGNS_READ
- description: campaigns write
  flows:
  - authorizationCode
  scope: CAMPAIGNS_WRITE
- description: catalog read
  flows:
  - authorizationCode
  scope: CATALOG_READ
- description: media write
  flows:
  - authorizationCode
  scope: MEDIA_WRITE
- description: publications read
  flows:
  - authorizationCode
  scope: PUBLICATIONS_READ
- description: publications write
  flows:
  - authorizationCode
  scope: PUBLICATIONS_WRITE
- description: reports read
  flows:
  - authorizationCode
  scope: REPORTS_READ
slug: comunicate-eu-scopes
source_filename: comunicate-eu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comunicate.eu/ro/documentatie-api\nschemes:\n- name: oauth2\n  source: openapi/comunicate-eu-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.comunicate.eu/api/v1/oauth/authorize\n    tokenUrl: https://app.comunicate.eu/api/v1/oauth/token\n  description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.eu/api/v1/oauth/register.\n    The access token is an API key and is accepted everywhere an API key is.\nscopes:\n- scope: ARTICLES_READ\n  description: articles read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Citirea articolelor organizației.\n- scope: ARTICLES_WRITE\n  description: articles write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs:\
  \ Crearea și modificarea articolelor, importul de documente și din\n    Drive, cererea de redactare.\n- scope: BALANCE_READ\n  description: balance read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Citirea soldului și a pachetelor deținute.\n- scope: CAMPAIGNS_READ\n  description: campaigns read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Citirea campaniilor.\n- scope: CAMPAIGNS_WRITE\n  description: campaigns write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Crearea campaniilor.\n- scope: CATALOG_READ\n  description: catalog read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs:\
  \ Citirea catalogului de publicații și a tipurilor de campanie.\n- scope: MEDIA_WRITE\n  description: media write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Încărcarea de imagini în galerie.\n- scope: PUBLICATIONS_READ\n  description: publications read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Citirea publicărilor și a stării lor.\n- scope: PUBLICATIONS_WRITE\n  description: publications write\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n  description_docs: Cererea de publicare — singura permisiune care cheltuie credite\n    sau bani.\n- scope: REPORTS_READ\n  description: reports read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/comunicate-eu-openapi.yml\n  - https://comunicate.eu/ro/documentatie-api\n\
  \  description_docs: Citirea rapoartelor pe interval.\ndocs: https://comunicate.eu/ro/documentatie-api\nnote: Scope names match the docs \"Permisiuni\" section verbatim; descriptions are the\n  docs Romanian text. The same scopes are attached to bk_live_ API keys when issued\n  from Integrations.\n"
source_yaml_url: https://artifacts.apis.io/comunicate-eu/scopes/comunicate-eu-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Company
- Press Releases
- Advertorials
- Content Marketing
- SEO
- Publishing
- Media Marketplace
- Romania
- MCP
- PR
- Media
- Link Building
- Open Data
- Webhook
- Authentication
token_bound: false
token_urls:
- https://app.comunicate.eu/api/v1/oauth/token
---
