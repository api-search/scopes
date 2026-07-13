---
api_specs:
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Authentication API
  slug: snov-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Finder API
  slug: snov-email-finder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Domain Search API
  slug: snov-domain-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Verifier API
  slug: snov-email-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Enrichment API
  slug: snov-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Prospects & Lists API
  slug: snov-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Drip Campaigns API
  slug: snov-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Sender Accounts API
  slug: snov-sender-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io Email Warm-up API
  slug: snov-warmup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
- filename: snov-openapi.yml
  format: yaml
  label: Snov.io User & Balance API
  slug: snov-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/openapi/snov-openapi.yml
authorization_urls: []
description: ''
docs: https://snov.io/api
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Snov Scopes
name_suffix: OAuth Scopes
note: Snov.io uses an OAuth2 client_credentials flow that exchanges an API User ID and Secret for a Bearer token with no scope parameter; no OAuth scopes are documented, with access governed by the account plan (https://snov.io/api).
overview: 'Snov.io uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.snov.io/v1/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snov.io
provider_slug: snov
schemes:
- description: OAuth2 client_credentials flow. POST client_id and client_secret to /v1/oauth/access_token to obtain a Bearer token, then send it in the Authorization header.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.snov.io/v1/oauth/access_token
  name: OAuth2
  source: openapi/snov-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: snov-scopes
source_filename: snov-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snov-openapi.yml\ndocs: https://snov.io/api\nnote: Snov.io uses an OAuth2 client_credentials flow that exchanges an API User ID\n  and Secret for a Bearer token with no scope parameter; no OAuth scopes are documented,\n  with access governed by the account plan (https://snov.io/api).\nschemes:\n- name: OAuth2\n  source: openapi/snov-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.snov.io/v1/oauth/access_token\n  description: OAuth2 client_credentials flow. POST client_id and client_secret to /v1/oauth/access_token\n    to obtain a Bearer token, then send it in the Authorization header.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snov/refs/heads/main/scopes/snov-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Sales Engagement
- Email Finder
- Email Verification
- Prospecting
- Drip Campaigns
- CRM
- Lead Generation
token_urls:
- https://api.snov.io/v1/oauth/access_token
---
