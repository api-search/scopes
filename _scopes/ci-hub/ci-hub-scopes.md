---
api_specs:
- filename: ci-hub-assets-api-openapi.yml
  format: yaml
  label: CI HUB Assets API
  slug: ci-hub-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/openapi/ci-hub-assets-api-openapi.yml
- filename: ci-hub-auth-api-openapi.yml
  format: yaml
  label: CI HUB Auth API
  slug: ci-hub-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/openapi/ci-hub-auth-api-openapi.yml
- filename: ci-hub-system-api-openapi.yml
  format: yaml
  label: CI HUB System API
  slug: ci-hub-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/openapi/ci-hub-system-api-openapi.yml
authorization_urls: []
description: ''
docs: https://ci-hub.com/ai/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ci Hub Scopes
name_suffix: OAuth Scopes
note: 'The Access SDK HTTP API has no OAuth scope surface — it authenticates by partner-JWT token exchange plus a per-DAM connection token, so derive-oauth-scopes.py correctly found nothing there. The scope surface belongs to the MCP server: mcp.ci-hub.com is an OAuth 2.1 protected resource whose authorization server publishes RFC 8414 metadata anonymously. That metadata declares exactly one scope. Values below are read verbatim from the live document; nothing is inferred.'
overview: 'CI HUB uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CI HUB
provider_slug: ci-hub
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: ci-hub-scopes
source_filename: ci-hub-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://mcp-auth.ci-hub.com/.well-known/oauth-authorization-server\ndocs: https://ci-hub.com/ai/mcp-server\nnote: >-\n  The Access SDK HTTP API has no OAuth scope surface — it authenticates by partner-JWT token\n  exchange plus a per-DAM connection token, so derive-oauth-scopes.py correctly found nothing\n  there. The scope surface belongs to the MCP server: mcp.ci-hub.com is an OAuth 2.1 protected\n  resource whose authorization server publishes RFC 8414 metadata anonymously. That metadata\n  declares exactly one scope. Values below are read verbatim from the live document; nothing is\n  inferred.\napplies_to: ci-hub:mcp\nauthorization_server: https://mcp-auth.ci-hub.com\nendpoints:\n  authorization: https://mcp-auth.ci-hub.com/authorize\n  token: https://mcp-auth.ci-hub.com/token\n  userinfo: https://mcp-auth.ci-hub.com/userinfo\n  jwks: https://mcp-auth.ci-hub.com/jwks.json\n  registration: https://mcp-auth.ci-hub.com/register\n\
  flows:\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  response_modes:\n  - query\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  dynamic_client_registration: true\n  subject_types:\n  - public\n  id_token_signing_alg:\n  - RS256\nscopes:\n- name: cihub\n  description: >-\n    The single scope advertised by the CI HUB MCP authorization server. It is coarse: it does not\n    subdivide by asset operation, by DAM provider, or by read versus write. Effective authority\n    is not decided by this scope but downstream — each end user separately authenticates the DAM\n    accounts they want reachable, and CI HUB maps that user's existing DAM permissions onto every\n    tool call. A consumer cannot narrow an MCP client's authority through the OAuth grant; the\n    narrowing happens in the DAM.\n  source: authorization-server-metadata\nclaims_supported:\n- sub\n- iss\n-\
  \ aud\n- exp\n- iat\n- scope\nsummary:\n  scope_count: 1\n  granularity: coarse\n  read_write_split: false\n  per_provider_scopes: false\nx-evidence:\n  fetched: '2026-08-12'\n  checks:\n  - url: https://mcp-auth.ci-hub.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp-auth.ci-hub.com/.well-known/openid-configuration\n    http_status: 200\n  - url: https://mcp.ci-hub.com/.well-known/oauth-protected-resource\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ci-hub/refs/heads/main/scopes/ci-hub-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Digital Asset Management
- Content Management
- Product Information Management
- Integration
- Connectors
- Creative Tools
- Marketing
- Brand Management
- MCP
- Cloud Storage
- Germany
token_urls: []
---
