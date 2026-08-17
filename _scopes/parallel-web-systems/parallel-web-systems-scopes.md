---
api_specs:
- filename: parallel-web-systems-chat-api-beta-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Chat API (Beta) API
  slug: parallel-web-systems-chat-api-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-chat-api-beta-api-openapi.yml
- filename: parallel-web-systems-extract-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Extract API
  slug: parallel-web-systems-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-extract-api-openapi.yml
- filename: parallel-web-systems-findall-api-openapi.yml
  format: yaml
  label: Parallel Web Systems FindAll API
  slug: parallel-web-systems-findall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-findall-api-openapi.yml
- filename: parallel-web-systems-monitor-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Monitor API
  slug: parallel-web-systems-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-monitor-api-openapi.yml
- filename: parallel-web-systems-search-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Search API
  slug: parallel-web-systems-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-search-api-openapi.yml
- filename: parallel-web-systems-tasks-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Tasks API
  slug: parallel-web-systems-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-tasks-api-openapi.yml
- filename: parallel-web-systems-responses-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Responses API
  slug: parallel-web-systems-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-responses-api-openapi.yml
- filename: parallel-web-systems-memory-api-openapi.yml
  format: yaml
  label: Parallel Web Systems Memory API (Beta)
  slug: parallel-web-systems-memory-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/openapi/parallel-web-systems-memory-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.parallel.ai/integrations/oauth-provider
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Parallel Web Systems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Parallel Web Systems uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Parallel Web Systems
provider_slug: parallel-web-systems
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: parallel-web-systems-scopes
source_filename: parallel-web-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.parallel.ai/integrations/oauth-provider\ndocs: https://docs.parallel.ai/integrations/oauth-provider\nmetadata:\n  discovery: https://platform.parallel.ai/.well-known/oauth-authorization-server\n  file: well-known/parallel-web-systems-oauth-authorization-server.json\n  spec: RFC 8414\n  issuer: https://platform.parallel.ai\nprovider:\n  name: Parallel OAuth Provider\n  url: https://platform.parallel.ai\n  authorization_endpoint: https://platform.parallel.ai/getKeys/authorize\n  token_endpoint: https://platform.parallel.ai/getKeys/token\n  registration_endpoint: https://platform.parallel.ai/getKeys/register\n  device_authorization_endpoint: https://platform.parallel.ai/getKeys/device/code\ngrant_types:\n- authorization_code\n- urn:ietf:params:oauth:grant-type:device_code\nclient_authentication:\n  token_endpoint_auth_methods_supported:\n  - none\n  detail: Public-client design - PKCE (S256) is mandatory and there\
  \ is no client secret.\npkce:\n  required: true\n  methods:\n  - S256\nscope_count: 1\nscopes:\n- name: key:read\n  description: >-\n    Use a Parallel API key to access the API on the user's behalf. The access_token\n    returned by the token endpoint IS the user's Parallel API key, which is then sent as\n    the x-api-key header on data-plane calls.\n  source: /.well-known/oauth-authorization-server scopes_supported + OAuth Provider docs\nconsumers:\n- name: parallel-cli\n  flow: device_code\n  detail: '`parallel-cli auth` runs the RFC 8628 device-code flow (--no-browser for headless).'\n- name: A2A Deep Research agent\n  flow: authorization_code\n  detail: >-\n    The A2A agent card at api.parallel.ai declares securityScheme `parallel_oauth` with\n    the authorizationCode flow and requires scope key:read. See a2a/parallel-web-systems-a2a.yml.\n- name: Search MCP (OAuth endpoint)\n  flow: authorization_code\n  detail: >-\n    https://search.parallel.ai/mcp-oauth is the OAuth-capable\
  \ MCP endpoint; anonymous\n    requests return 401. The default /mcp endpoint does not advertise OAuth.\n- name: Third-party applications\n  flow: authorization_code\n  detail: >-\n    Applications identify by hostname as client_id and users explicitly consent per\n    application, selecting or generating an API key at consent time.\ncaveats:\n- >-\n  The scope surface is deliberately minimal. OAuth here is a key-issuance / delegation\n  layer, not a per-resource permission model - there are no read/write or per-product\n  scopes. The data plane authorizes with a single opaque API key whose entitlements are\n  set by the account, not by the token.\n- >-\n  The OpenAPI declares only ApiKeyAuth (x-api-key) and no oauth2 securityScheme, so this\n  file could not be derived from the spec; it was searched from the OAuth Provider docs,\n  the RFC 8414 metadata, and the A2A agent card.\nnotes: >-\n  derive-oauth-scopes.py found no oauth2 securityScheme in the OpenAPI (0 providers with\n  oauth2),\
  \ so this artifact is entirely searched/probed from Parallel's own published\n  OAuth surface. No scopes were invented - scopes_supported carries exactly one value.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-web-systems/refs/heads/main/scopes/parallel-web-systems-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Ai Ml
- Web Search
- Deep Research
- Data Enrichment
- Web Monitoring
- AI Agents
- MCP
- A2A
- Agent Skills
- Content Extraction
- Entity Resolution
token_urls: []
---
