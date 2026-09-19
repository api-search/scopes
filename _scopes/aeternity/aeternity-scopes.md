---
api_specs:
- filename: aeternity-accounts-api-openapi.yml
  format: yaml
  label: Aeternity Accounts API
  slug: aeternity-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-accounts-api-openapi.yml
- filename: aeternity-aex141-api-openapi.yml
  format: yaml
  label: Aeternity Aex141 API
  slug: aeternity-aex141-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-aex141-api-openapi.yml
- filename: aeternity-aex9-api-openapi.yml
  format: yaml
  label: Aeternity Aex9 API
  slug: aeternity-aex9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-aex9-api-openapi.yml
- filename: aeternity-channels-api-openapi.yml
  format: yaml
  label: Aeternity Channels API
  slug: aeternity-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-channels-api-openapi.yml
- filename: aeternity-contracts-api-openapi.yml
  format: yaml
  label: Aeternity Contracts API
  slug: aeternity-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-contracts-api-openapi.yml
- filename: aeternity-dex-api-openapi.yml
  format: yaml
  label: Aeternity Dex API
  slug: aeternity-dex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-dex-api-openapi.yml
- filename: aeternity-external-api-openapi.yml
  format: yaml
  label: Aeternity External API
  slug: aeternity-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-external-api-openapi.yml
- filename: aeternity-hyperchain-api-openapi.yml
  format: yaml
  label: Aeternity Hyperchain API
  slug: aeternity-hyperchain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-hyperchain-api-openapi.yml
- filename: aeternity-internal-api-openapi.yml
  format: yaml
  label: Aeternity Internal API
  slug: aeternity-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-internal-api-openapi.yml
- filename: aeternity-key-blocks-api-openapi.yml
  format: yaml
  label: Aeternity Key Blocks API
  slug: aeternity-key-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-key-blocks-api-openapi.yml
- filename: aeternity-micro-blocks-api-openapi.yml
  format: yaml
  label: Aeternity Micro Blocks API
  slug: aeternity-micro-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-micro-blocks-api-openapi.yml
- filename: aeternity-names-api-openapi.yml
  format: yaml
  label: Aeternity Names API
  slug: aeternity-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-names-api-openapi.yml
- filename: aeternity-oracles-api-openapi.yml
  format: yaml
  label: Aeternity Oracles API
  slug: aeternity-oracles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-oracles-api-openapi.yml
- filename: aeternity-stats-api-openapi.yml
  format: yaml
  label: Aeternity Stats API
  slug: aeternity-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-stats-api-openapi.yml
- filename: aeternity-status-api-openapi.yml
  format: yaml
  label: Aeternity Status API
  slug: aeternity-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-status-api-openapi.yml
- filename: aeternity-transactions-api-openapi.yml
  format: yaml
  label: Aeternity Transactions API
  slug: aeternity-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-transactions-api-openapi.yml
- filename: aeternity-transfers-api-openapi.yml
  format: yaml
  label: Aeternity Transfers API
  slug: aeternity-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/openapi/aeternity-transfers-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aeternity Scopes
name_suffix: OAuth Scopes
note: Neither OpenAPI declares an oauth2 securityScheme, so nothing was derivable from the specs (derive-oauth-scopes.py found 0 oauth2 schemes). The only OAuth surface æternity publishes is the MCP endpoint on aeternity.com, and its authorization-server metadata declares exactly one scope. No scope reference page exists in the documentation; these values are read verbatim from the served discovery documents, not inferred.
overview: 'Aeternity uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aeternity
provider_slug: aeternity
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: aeternity-scopes
source_filename: aeternity-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://aeternity.com/.well-known/oauth-authorization-server\nnote: >-\n  Neither OpenAPI declares an oauth2 securityScheme, so nothing was derivable from the specs\n  (derive-oauth-scopes.py found 0 oauth2 schemes). The only OAuth surface æternity publishes is the MCP\n  endpoint on aeternity.com, and its authorization-server metadata declares exactly one scope. No scope\n  reference page exists in the documentation; these values are read verbatim from the served discovery\n  documents, not inferred.\nauthorization_server: https://aeternity.com\nprotected_resource: https://aeternity.com/wp-json/mcp/mcp-oauth-server\nflows:\n  authorization_code:\n    authorization_endpoint: https://aeternity.com/oauth/authorize\n    token_endpoint: https://aeternity.com/oauth/token\n    revocation_endpoint: https://aeternity.com/oauth/revoke\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\nscopes:\n- name: mcp\n\
  \  description: >-\n    The single scope advertised in scopes_supported by both the authorization-server metadata and the\n    protected-resource metadata. The documents publish no description of what it grants, and the tool set it\n    gates could not be enumerated anonymously.\n  source: https://aeternity.com/.well-known/oauth-authorization-server\nscope_count: 1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeternity/refs/heads/main/scopes/aeternity-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Blockchain
- Layer 1
- Smart Contracts
- Cryptocurrency
- Web3
- Distributed Ledger
- Open-Source
- GraphQL
- State Channels
- Oracle
- Naming System
- Developer Tools
token_urls: []
---
