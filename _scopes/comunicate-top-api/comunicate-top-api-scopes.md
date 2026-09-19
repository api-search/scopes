---
api_specs:
- filename: comunicate-top-api-articles-api-openapi.yml
  format: yaml
  label: Comunicate.top API Articles API
  slug: comunicate-top-api-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-articles-api-openapi.yml
- filename: comunicate-top-api-balance-and-reports-api-openapi.yml
  format: yaml
  label: Comunicate.top API Balance and reports API
  slug: comunicate-top-api-balance-and-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-balance-and-reports-api-openapi.yml
- filename: comunicate-top-api-campaigns-api-openapi.yml
  format: yaml
  label: Comunicate.top API Campaigns API
  slug: comunicate-top-api-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-campaigns-api-openapi.yml
- filename: comunicate-top-api-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.top API Catalogue API
  slug: comunicate-top-api-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-catalogue-api-openapi.yml
- filename: comunicate-top-api-checks-api-openapi.yml
  format: yaml
  label: Comunicate.top API Checks API
  slug: comunicate-top-api-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-checks-api-openapi.yml
- filename: comunicate-top-api-domain-audit-api-openapi.yml
  format: yaml
  label: Comunicate.top API Domain audit API
  slug: comunicate-top-api-domain-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-domain-audit-api-openapi.yml
- filename: comunicate-top-api-key-and-permissions-api-openapi.yml
  format: yaml
  label: Comunicate.top API Key and permissions API
  slug: comunicate-top-api-key-and-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-key-and-permissions-api-openapi.yml
- filename: comunicate-top-api-media-api-openapi.yml
  format: yaml
  label: Comunicate.top API Media API
  slug: comunicate-top-api-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-media-api-openapi.yml
- filename: comunicate-top-api-public-catalogue-api-openapi.yml
  format: yaml
  label: Comunicate.top API Public catalogue API
  slug: comunicate-top-api-public-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-public-catalogue-api-openapi.yml
- filename: comunicate-top-api-publications-api-openapi.yml
  format: yaml
  label: Comunicate.top API Publications API
  slug: comunicate-top-api-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-publications-api-openapi.yml
- filename: comunicate-top-api-writing-orders-api-openapi.yml
  format: yaml
  label: Comunicate.top API Writing orders API
  slug: comunicate-top-api-writing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/openapi/comunicate-top-api-writing-orders-api-openapi.yml
authorization_urls:
- https://app.comunicate.top/api/v1/oauth/authorize
description: ''
docs: https://comunicate.top/ro/documentatie-api
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Comunicate Top Api Scopes
name_suffix: OAuth Scopes
note: 'Scope names and flow derived from the OpenAPI oauth2 scheme; descriptions enriched from the permissions section of the API docs. The same 10 scopes are listed as scopes_supported in the RFC 8414 metadata at https://app.comunicate.top/.well-known/oauth-authorization-server. Keys are scoped identically: each API key receives only the permissions chosen at issue time, and an OAuth access token is accepted everywhere a key is.'
overview: 'Comunicate.top API publishes 10 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Comunicate.top API API on a user''s behalf.


  Tokens are issued from https://app.comunicate.top/api/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Comunicate.top API
provider_slug: comunicate-top-api
schemes:
- description: OAuth 2.1 with PKCE (S256). Dynamic client registration at https://app.comunicate.top/api/v1/oauth/register. The access token is an API key and is accepted everywhere an API key is.
  flows:
  - authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.comunicate.top/api/v1/oauth/token
    tokenUrl: https://app.comunicate.top/api/v1/oauth/token
  name: oauth2
  pkce: S256 required (OAuth 2.1)
  registration: https://app.comunicate.top/api/v1/oauth/register (RFC 7591 dynamic client registration)
  source: openapi/comunicate-top-api-openapi-original.json
scope_count: 10
scope_names:
- CATALOG_READ
- ARTICLES_READ
- ARTICLES_WRITE
- MEDIA_WRITE
- PUBLICATIONS_READ
- PUBLICATIONS_WRITE
- CAMPAIGNS_READ
- CAMPAIGNS_WRITE
- BALANCE_READ
- REPORTS_READ
scopes:
- description: Read the publication catalogue and the campaign types.
  flows:
  - authorizationCode
  scope: CATALOG_READ
- description: Read the organization's articles.
  flows:
  - authorizationCode
  scope: ARTICLES_READ
- description: Create and modify articles, import documents and from Drive, request writing orders.
  flows:
  - authorizationCode
  scope: ARTICLES_WRITE
- description: Upload images to the gallery.
  flows:
  - authorizationCode
  scope: MEDIA_WRITE
- description: Read publications and their status.
  flows:
  - authorizationCode
  scope: PUBLICATIONS_READ
- description: Request publication — the only permission that spends credits or money.
  flows:
  - authorizationCode
  scope: PUBLICATIONS_WRITE
- description: Read campaigns.
  flows:
  - authorizationCode
  scope: CAMPAIGNS_READ
- description: Create campaigns.
  flows:
  - authorizationCode
  scope: CAMPAIGNS_WRITE
- description: Read the balance and the packages held.
  flows:
  - authorizationCode
  scope: BALANCE_READ
- description: Read reports over a period.
  flows:
  - authorizationCode
  scope: REPORTS_READ
slug: comunicate-top-api-scopes
source_filename: comunicate-top-api-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/comunicate-top-api-openapi-original.json\ndocs: https://comunicate.top/ro/documentatie-api\nnote: >-\n  Scope names and flow derived from the OpenAPI oauth2 scheme; descriptions enriched from the\n  permissions section of the API docs. The same 10 scopes are listed as scopes_supported in the\n  RFC 8414 metadata at https://app.comunicate.top/.well-known/oauth-authorization-server. Keys are\n  scoped identically: each API key receives only the permissions chosen at issue time, and an OAuth\n  access token is accepted everywhere a key is.\nschemes:\n  - name: oauth2\n    source: openapi/comunicate-top-api-openapi-original.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.comunicate.top/api/v1/oauth/authorize\n        tokenUrl: https://app.comunicate.top/api/v1/oauth/token\n        refreshUrl: https://app.comunicate.top/api/v1/oauth/token\n    registration: https://app.comunicate.top/api/v1/oauth/register\
  \ (RFC 7591 dynamic client registration)\n    pkce: S256 required (OAuth 2.1)\n    description: >-\n      OAuth 2.1 with PKCE (S256). Dynamic client registration at\n      https://app.comunicate.top/api/v1/oauth/register. The access token is an API key and is\n      accepted everywhere an API key is.\nscopes:\n  - scope: CATALOG_READ\n    description: Read the publication catalogue and the campaign types.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: ARTICLES_READ\n    description: Read the organization's articles.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: ARTICLES_WRITE\n    description: Create and modify articles, import documents and from Drive, request writing orders.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: MEDIA_WRITE\n    description: Upload images to the gallery.\n    flows: [authorizationCode]\n\
  \    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: PUBLICATIONS_READ\n    description: Read publications and their status.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: PUBLICATIONS_WRITE\n    description: Request publication — the only permission that spends credits or money.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: CAMPAIGNS_READ\n    description: Read campaigns.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: CAMPAIGNS_WRITE\n    description: Create campaigns.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: BALANCE_READ\n    description: Read the balance and the packages held.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n  - scope: REPORTS_READ\n    description:\
  \ Read reports over a period.\n    flows: [authorizationCode]\n    sources: [openapi/comunicate-top-api-openapi-original.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comunicate-top-api/refs/heads/main/scopes/comunicate-top-api-scopes.yml
summary_line: 10 scopes · authorizationCode
tags:
- Press Releases
- Advertorials
- PR
- Publishing
- Media
- SEO
- Link Building
- Content Marketing
- Romania
- MCP
- Open Data
- Webhook
- Authentication
token_urls:
- https://app.comunicate.top/api/v1/oauth/token
---
