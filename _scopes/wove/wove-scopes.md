---
authorization_urls: []
description: OAuth 2.0 scopes for the Wove External API, derived from the published OpenAPI at api.wove.com/api/docs. The API uses the client_credentials grant (POST /api/v1/external/auth/token) with an optional space-separated scope parameter; the spec's securityScheme is declared as http bearer (JWT), with the scope model expressed through the TokenRequest/TokenResponse schemas and per-operation 403 "requires <scope> scope" responses. Scope names below are exactly those named in the spec; Wove publishes no standalone scopes reference page.
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Wove Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wove publishes 9 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wove API on a user''s behalf.


  Tokens are issued from https://api.wove.com/api/v1/external/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wove
provider_slug: wove
schemes:
- flows:
  - flow: clientCredentials
    revocationUrl: https://api.wove.com/api/v1/external/auth/revoke
    tokenUrl: https://api.wove.com/api/v1/external/auth/token
  name: bearerAuth
  source: openapi/wove-external-api-openapi-original.yml
  type: http (bearer JWT) issued via OAuth 2.0 client_credentials
scope_count: 9
scope_names:
- shipments:read
- documents:read
- validation:create
- tariffs:read
- rates:read
- sources:write
- tms-organizations:read
- tms-organizations:write
- tms-organizations:delete
scopes:
- description: Read access to shipments (named in TokenRequest/TokenResponse scope examples).
  flows: []
  scope: shipments:read
- description: Read access to documents (named in TokenRequest/TokenResponse scope examples).
  flows: []
  scope: documents:read
- description: Create document validation jobs (named in TokenRequest/TokenResponse scope examples).
  flows: []
  scope: validation:create
- description: Required for tariff lookup/search/batch-lookup operations (per-operation 403 responses).
  flows: []
  scope: tariffs:read
- description: Required for querying rates from query-bank sources (per-operation 403 response).
  flows: []
  scope: rates:read
- description: Required for uploading and processing rate/document sources (per-operation 403 response).
  flows: []
  scope: sources:write
- description: Read access to TMS organizations (per-operation 403 responses).
  flows: []
  scope: tms-organizations:read
- description: Create/update/import TMS organizations (per-operation 403 responses).
  flows: []
  scope: tms-organizations:write
- description: Delete TMS organizations (per-operation 403 response).
  flows: []
  scope: tms-organizations:delete
slug: wove-scopes
source_filename: wove-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/wove-external-api-openapi-original.yml\ndescription: >-\n  OAuth 2.0 scopes for the Wove External API, derived from the published\n  OpenAPI at api.wove.com/api/docs. The API uses the client_credentials grant\n  (POST /api/v1/external/auth/token) with an optional space-separated scope\n  parameter; the spec's securityScheme is declared as http bearer (JWT), with\n  the scope model expressed through the TokenRequest/TokenResponse schemas and\n  per-operation 403 \"requires <scope> scope\" responses. Scope names below are\n  exactly those named in the spec; Wove publishes no standalone scopes\n  reference page.\nschemes:\n  - name: bearerAuth\n    type: http (bearer JWT) issued via OAuth 2.0 client_credentials\n    source: openapi/wove-external-api-openapi-original.yml\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.wove.com/api/v1/external/auth/token\n        revocationUrl: https://api.wove.com/api/v1/external/auth/revoke\n\
  scopes:\n  - scope: shipments:read\n    description: Read access to shipments (named in TokenRequest/TokenResponse scope examples).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: documents:read\n    description: Read access to documents (named in TokenRequest/TokenResponse scope examples).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: validation:create\n    description: Create document validation jobs (named in TokenRequest/TokenResponse scope examples).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: tariffs:read\n    description: Required for tariff lookup/search/batch-lookup operations (per-operation 403 responses).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: rates:read\n    description: Required for querying rates from query-bank sources (per-operation 403 response).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: sources:write\n    description:\
  \ Required for uploading and processing rate/document sources (per-operation 403 response).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: tms-organizations:read\n    description: Read access to TMS organizations (per-operation 403 responses).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: tms-organizations:write\n    description: Create/update/import TMS organizations (per-operation 403 responses).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n  - scope: tms-organizations:delete\n    description: Delete TMS organizations (per-operation 403 response).\n    sources: [openapi/wove-external-api-openapi-original.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wove/refs/heads/main/scopes/wove-scopes.yml
summary_line: 9 scopes · clientCredentials
tags:
- Company
token_urls:
- https://api.wove.com/api/v1/external/auth/token
---
