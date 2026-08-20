---
api_specs:
- filename: sp-global-auditors-api-openapi.yml
  format: yaml
  label: S&P Global LLM-Ready API (kFinance)
  slug: kensho-llm-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-auditors-api-openapi.yml
- filename: sp-global-extractions-api-openapi.yml
  format: yaml
  label: Kensho Extract API
  slug: kensho-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-extractions-api-openapi.yml
- filename: sp-global-annotations-async-api-openapi.yml
  format: yaml
  label: Kensho NERD API
  slug: kensho-nerd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-annotations-async-api-openapi.yml
- filename: sp-global-transcription-api-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v2
  slug: kensho-scribe-batch-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-transcription-api-openapi.yml
- filename: kensho-scribe-realtime-asyncapi.yml
  format: yaml
  label: Kensho Scribe Real Time API
  slug: kensho-scribe-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/asyncapi/kensho-scribe-realtime-asyncapi.yml
- filename: sp-global-transcription-api-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v1
  slug: kensho-scribe-batch-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/sp-global-transcription-api-openapi.yml
authorization_urls:
- https://kfinance.kensho.com/integrations/authorize
description: ''
docs: https://docs.kensho.com/authentication
flows:
- authorizationCode
- refresh_token
kind: oauth-scopes
layout: scope
method: searched
name: Sp Global Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'S&P Global publishes 2 OAuth 2.0 scopes via the authorizationCode and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the S&P Global API on a user''s behalf.


  Tokens are issued from https://kfinance.kensho.com/integrations/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: S&P Global
provider_slug: sp-global
schemes:
- flows:
  - authorizationUrl: https://kfinance.kensho.com/integrations/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://kfinance.kensho.com/integrations/token
  - flow: refresh_token
  issuer: https://kfinance.kensho.com/integrations
  name: Kensho OAuth 2.0 / OIDC (kFinance integrations)
  registration: https://kfinance.kensho.com/integrations/register
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
scope_count: 2
scope_names:
- kensho:app:kfinance
- offline_access
scopes:
- description: Access to the kFinance (S&P Global LLM-Ready API) application, including the hosted MCP resource.
  flows:
  - authorizationCode
  scope: kensho:app:kfinance
- description: Issue a refresh token for long-lived / unattended access.
  flows:
  - authorizationCode
  scope: offline_access
slug: sp-global-scopes
source_filename: sp-global-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://kfinance.kensho.com/.well-known/oauth-authorization-server (RFC 8414) + https://kfinance.kensho.com/.well-known/oauth-protected-resource (RFC 9728)\ndocs: https://docs.kensho.com/authentication\nnotes: >-\n  The published OpenAPI specs declare only a bearer JWT scheme (no oauth2 flows), so no scopes are\n  derivable from spec. The live RFC 8414 authorization-server metadata on kfinance.kensho.com —\n  the OAuth front door for the hosted kFinance MCP server — publishes the real scope surface.\n  Kensho auth is OIDC on OAuth 2.0 with keypair (production) or refresh-token (development,\n   7-day expiry) grants.\nschemes:\n  - name: Kensho OAuth 2.0 / OIDC (kFinance integrations)\n    issuer: https://kfinance.kensho.com/integrations\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://kfinance.kensho.com/integrations/authorize\n        tokenUrl: https://kfinance.kensho.com/integrations/token\n\
  \        pkce: S256\n      - flow: refresh_token\n    registration: https://kfinance.kensho.com/integrations/register\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\nscopes:\n  - scope: 'kensho:app:kfinance'\n    description: Access to the kFinance (S&P Global LLM-Ready API) application, including the hosted MCP resource.\n    flows: [authorizationCode]\n    sources: [well-known/sp-global-oauth-authorization-server.json]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived / unattended access.\n    flows: [authorizationCode]\n    sources: [well-known/sp-global-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/scopes/sp-global-scopes.yml
summary_line: 2 scopes · authorizationCode/refresh_token
tags:
- Capital IQ
- Commodity Insights
- Credit Ratings
- Document Extraction
- ESG
- Financial Data
- Index Data
- LLM
- MCP
- Market Intelligence
- Mobility
- Named Entity Recognition
- Speech-to-Text
token_urls:
- https://kfinance.kensho.com/integrations/token
---
