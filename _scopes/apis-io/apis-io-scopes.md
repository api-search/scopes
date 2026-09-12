---
api_specs:
- filename: apis-io-submit-api-openapi.yml
  format: yaml
  label: APIs.io Submit API
  slug: apisio-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-submit-api-openapi.yml
- filename: apis-io-apis-api-openapi.yml
  format: yaml
  label: APIs.io APIs API
  slug: apis-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-apis-api-openapi.yml
- filename: apis-io-areas-api-openapi.yml
  format: yaml
  label: APIs.io Areas API
  slug: apis-io-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-areas-api-openapi.yml
- filename: apis-io-artifact-types-api-openapi.yml
  format: yaml
  label: APIs.io Artifact Types API
  slug: apis-io-artifact-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-artifact-types-api-openapi.yml
- filename: apis-io-industries-api-openapi.yml
  format: yaml
  label: APIs.io Industries API
  slug: apis-io-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-industries-api-openapi.yml
- filename: apis-io-insights-api-openapi.yml
  format: yaml
  label: APIs.io Insights API
  slug: apis-io-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-insights-api-openapi.yml
- filename: apis-io-providers-api-openapi.yml
  format: yaml
  label: APIs.io Providers API
  slug: apis-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-providers-api-openapi.yml
- filename: apis-io-ratings-api-openapi.yml
  format: yaml
  label: APIs.io Ratings API
  slug: apis-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-ratings-api-openapi.yml
- filename: apis-io-regions-api-openapi.yml
  format: yaml
  label: APIs.io Regions API
  slug: apis-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-regions-api-openapi.yml
- filename: apis-io-search-api-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: apis-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-search-api-openapi.yml
- filename: apis-io-synthesis-api-openapi.yml
  format: yaml
  label: APIs.io Synthesis API
  slug: apis-io-synthesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-synthesis-api-openapi.yml
- filename: apis-io-tags-api-openapi.yml
  format: yaml
  label: APIs.io Tags API
  slug: apis-io-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-tags-api-openapi.yml
- filename: apis-io-cohorts-api-openapi.yml
  format: yaml
  label: APIs.io Cohorts API
  slug: apis-io-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-cohorts-api-openapi.yml
- filename: apis-io-editorial-api-openapi.yml
  format: yaml
  label: APIs.io Editorial API
  slug: apis-io-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-editorial-api-openapi.yml
- filename: apis-io-export-api-openapi.yml
  format: yaml
  label: APIs.io Export API
  slug: apis-io-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-export-api-openapi.yml
- filename: apis-io-resolve-enrich-api-openapi.yml
  format: yaml
  label: APIs.io Resolve & Enrich API
  slug: apis-io-resolve-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-resolve-enrich-api-openapi.yml
- filename: apis-io-saved-workspace-api-openapi.yml
  format: yaml
  label: APIs.io Saved Workspace API
  slug: apis-io-saved-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-saved-workspace-api-openapi.yml
- filename: apis-io-venture-capital-api-openapi.yml
  format: yaml
  label: APIs.io Venture Capital API
  slug: apis-io-venture-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-venture-capital-api-openapi.yml
authorization_urls:
- https://apis.io/api/v1/auth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Apis Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'APIs.io publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the APIs.io API on a user''s behalf.


  Tokens are issued from https://apis.io/api/v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: APIs.io
provider_slug: apis-io
schemes:
- description: The machine path to the same tiers, and the better of the two options for an agent. APIs.io runs its own OAuth 2.1 authorization server -- RFC 8414 metadata at /.well-known/oauth-authorization-server, a JWKS at /.well-known/jwks.json, PKCE (S256 only), RFC 7591 dynamic client registration, and RFC 8707 resource indicators -- so a client can earn access through a protocol handshake instead of a human pasting a key. An access token resolves to the same tier and the same per-user quota as that user's API key. Declared here as of 2026-08-30; the server has been live since before that, and an agent reading this contract to decide how to authenticate could not previously discover it.
  flows:
  - authorizationUrl: https://apis.io/api/v1/auth/authorize
    flow: authorizationCode
    tokenUrl: https://apis.io/api/v1/auth/token
  name: OAuth2
  source: openapi/apis-io-v1-openapi.yml
scope_count: 3
scope_names:
- apis:pro
- apis:read
- offline_access
scopes:
- description: The tier-gated resources -- ratings, insights, demand depth, the Saved Workspace.
  flows:
  - authorizationCode
  scope: apis:pro
- description: Read the catalog. Granted to every caller.
  flows:
  - authorizationCode
  scope: apis:read
- description: Issue a refresh token. Authorization-server scope only; no resource asks for it.
  flows:
  - authorizationCode
  scope: offline_access
slug: apis-io-scopes
source_filename: apis-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: derived\nsource: openapi/apis-io-v1-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/apis-io-v1-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apis.io/api/v1/auth/authorize\n    tokenUrl: https://apis.io/api/v1/auth/token\n  description: The machine path to the same tiers, and the better of the two options for an\n    agent. APIs.io runs its own OAuth 2.1 authorization server -- RFC 8414 metadata at /.well-known/oauth-authorization-server,\n    a JWKS at /.well-known/jwks.json, PKCE (S256 only), RFC 7591 dynamic client registration,\n    and RFC 8707 resource indicators -- so a client can earn access through a protocol handshake\n    instead of a human pasting a key. An access token resolves to the same tier and the same\n    per-user quota as that user's API key. Declared here as of 2026-08-30; the server has been\n    live since before that, and an agent reading this contract to decide how to authenticate\n\
  \    could not previously discover it.\nscopes:\n- scope: apis:pro\n  description: The tier-gated resources -- ratings, insights, demand depth, the Saved Workspace.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apis-io-v1-openapi.yml\n- scope: apis:read\n  description: Read the catalog. Granted to every caller.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apis-io-v1-openapi.yml\n- scope: offline_access\n  description: Issue a refresh token. Authorization-server scope only; no resource asks for\n    it.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/apis-io-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/scopes/apis-io-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engines
- API Catalog
- Agent Discovery
- MCP
- Agent Skills
- OpenAPI
- API Governance
token_urls:
- https://apis.io/api/v1/auth/token
---
