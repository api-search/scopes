---
api_specs:
- filename: trioptima-trireduce-api-openapi.yml
  format: yaml
  label: Trioptima triReduce API
  slug: trireduce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/openapi/trioptima-trireduce-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Trioptima Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Trioptima publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Trioptima API on a user''s behalf.


  Tokens are issued from https://auth.trireduce.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Trioptima
provider_slug: trioptima
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.trireduce.com/oauth/token
  name: oauth2
  source: openapi/trioptima-trireduce-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read-only access to cycles, trades, and results
  flows:
  - clientCredentials
  scope: read
- description: Full access to submit trades, risk data, and confirmations
  flows:
  - clientCredentials
  scope: write
slug: trioptima-scopes
source_filename: trioptima-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trioptima-trireduce-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/trioptima-trireduce-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.trireduce.com/oauth/token\nscopes:\n- scope: read\n  description: Read-only access to cycles, trades, and results\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trioptima-trireduce-api-openapi.yml\n- scope: write\n  description: Full access to submit trades, risk data, and confirmations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trioptima-trireduce-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trioptima/refs/heads/main/scopes/trioptima-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- CME Group
- Derivatives
- Financial Services
- OSTTRA
- Portfolio Compression
- Post-Trade Services
- Reconciliation
- Risk Management
token_urls:
- https://auth.trireduce.com/oauth/token
---
