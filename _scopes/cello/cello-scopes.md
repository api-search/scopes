---
api_specs:
- filename: cello-events-api-openapi.yml
  format: yaml
  label: Cello Events API
  slug: cello-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-events-api-openapi.yml
- filename: cello-new-users-api-openapi.yml
  format: yaml
  label: Cello New Users API
  slug: cello-new-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-new-users-api-openapi.yml
- filename: cello-referral-codes-api-openapi.yml
  format: yaml
  label: Cello Referral Codes API
  slug: cello-referral-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referral-codes-api-openapi.yml
- filename: cello-referrers-api-openapi.yml
  format: yaml
  label: Cello Referrers API
  slug: cello-referrers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-referrers-api-openapi.yml
- filename: cello-token-api-openapi.yml
  format: yaml
  label: Cello Token API
  slug: cello-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-token-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.cello.so/mcp/introduction
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Cello Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cello uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cello
provider_slug: cello
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: cello-scopes
source_filename: cello-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.cello.so/.well-known/oauth-protected-resource\ndocs: https://docs.cello.so/mcp/introduction\nsummary: >-\n  Cello's OAuth surface belongs to the hosted MCP server, not to the REST API. The MCP server\n  publishes RFC 9728 protected-resource metadata declaring two resource scopes, mcp:read and\n  mcp:write, and names https://auth.cello.so as its authorization server. The REST API at\n  api.cello.so declares no oauth2 securityScheme and no scopes at all — it authenticates with an\n  accessKeyId/secretAccessKey exchange at POST /token that returns an opaque bearer accessToken,\n  which carries no scope claim in any documented response.\nresource:\n  identifier: https://mcp.cello.so\n  authorization_servers:\n  - https://auth.cello.so\n  bearer_methods_supported:\n  - header\nscopes:\n- name: mcp:read\n  source: https://mcp.cello.so/.well-known/oauth-protected-resource\n  description: >-\n    Read access to the Cello\
  \ MCP server. Cello's own tool reference states that all MCP tools are\n    currently read-only, so this is the scope every published tool needs — program metrics,\n    referrers, top referrers, integration status, events, recommendations, knowledge-base search,\n    and the docs filesystem query.\n  applies_to_tools:\n  - cello_get_program_metrics\n  - cello_get_referrers\n  - cello_get_top_referrers\n  - cello_get_integration_status\n  - cello_get_events\n  - cello_get_recommendations\n  - search_cello\n  - query_docs_filesystem_cello\n  evidence: https://docs.cello.so/mcp/tools\n- name: mcp:write\n  source: https://mcp.cello.so/.well-known/oauth-protected-resource\n  description: >-\n    Write access to the Cello MCP server. Advertised in the protected-resource metadata but not\n    exercised by any tool Cello currently documents; the tool reference says the assistant points\n    you to the Cello Portal to make changes. Recorded as declared-but-unused.\n  applies_to_tools: []\n  status:\
  \ declared-unused\nauthorization_server:\n  issuer: https://auth.cello.so\n  metadata: ../well-known/cello-oauth-authorization-server.json\n  authorization_endpoint: https://auth.cello.so/oauth2/auth\n  token_endpoint: https://auth.cello.so/oauth2/token\n  registration_endpoint: https://auth.cello.so/oauth2/register\n  revocation_endpoint: https://auth.cello.so/oauth2/revoke\n  jwks_uri: https://auth.cello.so/.well-known/jwks.json\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  scopes_supported:\n  - offline_access\n  - offline\n  - openid\n  note: >-\n    The authorization server advertises only the three OIDC/offline scopes in scopes_supported;\n    the mcp:read and mcp:write resource scopes appear solely in the MCP protected-resource\n    document. A client requesting them relies on the resource indicator, not on the\
  \ AS metadata.\nrest_api:\n  oauth2: false\n  note: >-\n    No oauth2 securityScheme in openapi/_original/cello-openapi-original.json — the only scheme is\n    bearerAuth (type http, scheme bearer). derive-oauth-scopes.py reports 0 oauth2 schemes for\n    this provider; nothing here was derived from the spec.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - {url: 'https://mcp.cello.so/.well-known/oauth-protected-resource', http_status: 200}\n  - {url: 'https://auth.cello.so/.well-known/oauth-authorization-server', http_status: 200}\n  - {url: 'https://auth.cello.so/.well-known/openid-configuration', http_status: 200}\n  - {url: 'https://mcp.cello.so/mcp', http_status: 401, note: 'POST tools/list returned WWW-Authenticate: Bearer resource_metadata=...'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/scopes/cello-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- Software-as-a-Service
- Attribution
- Partner Programs
- Ai Enterprise Software
token_urls: []
---
