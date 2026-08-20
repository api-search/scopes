---
api_specs:
- filename: tl-dv-meetings-api-openapi.yml
  format: yaml
  label: tl;dv Meetings API
  slug: tl-dv-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-meetings-api-openapi.yml
- filename: tl-dv-notes-api-openapi.yml
  format: yaml
  label: tl;dv Notes API
  slug: tl-dv-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-notes-api-openapi.yml
- filename: tl-dv-system-api-openapi.yml
  format: yaml
  label: tl;dv System API
  slug: tl-dv-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-system-api-openapi.yml
- filename: tl-dv-transcripts-api-openapi.yml
  format: yaml
  label: tl;dv Transcripts API
  slug: tl-dv-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/openapi/tl-dv-transcripts-api-openapi.yml
authorization_urls:
- https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Tl Dv Scopes
name_suffix: OAuth Scopes
note: The tl;dv REST API has NO OAuth surface — it authenticates with a single x-api-key header and has no scopes (see authentication/tl-dv-authentication.yml). A prior round therefore omitted this artifact, correctly at the time. An OAuth scope surface does exist, but only on the hosted MCP endpoint https://mcp.tldv.io/mcp, and it was found by probe rather than in any documentation. The RFC 9728 protected-resource metadata and the RFC 8414 authorization-server metadata both resolve 200 anonymously and are saved verbatim under well-known/. Exactly ONE scope is advertised. tl;dv publishes no scopes/permissions reference page, so descriptions below are read from the metadata and the server's capability, not from prose that does not exist.
overview: 'tl;dv publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the tl;dv API on a user''s behalf.


  Tokens are issued from https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: tl;dv
provider_slug: tl-dv
schemes:
- code_challenge_methods_supported:
  - S256
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/auth
    flow: authorizationCode
    refreshUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token
    tokenUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  implementation: Keycloak
  introspection_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token/introspect
  issuer: https://keycloak.tldv.io/realms/mcp.tldv.io
  metadata_file: well-known/tl-dv-oauth-authorization-server.json
  name: MCPOAuth
  pkce_required: true
  registration_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/clients-registrations/openid-connect
  response_types_supported:
  - code
  - none
  - id_token
  - token
  - id_token token
  - code id_token
  - code token
  - code id_token token
  revocation_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/revoke
  source: https://mcp.tldv.io/.well-known/oauth-authorization-server
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Invoke the tools exposed by the tl;dv MCP server (list-meetings, get-meeting-metadata, get-transcript, get-highlights).
  flows:
  - authorizationCode
  scope: mcp:tools
slug: tl-dv-scopes
source_filename: tl-dv-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.tldv.io/.well-known/oauth-protected-resource\nnote: >\n  The tl;dv REST API has NO OAuth surface — it authenticates with a single\n  x-api-key header and has no scopes (see\n  authentication/tl-dv-authentication.yml). A prior round therefore omitted\n  this artifact, correctly at the time.\n\n  An OAuth scope surface does exist, but only on the hosted MCP endpoint\n  https://mcp.tldv.io/mcp, and it was found by probe rather than in any\n  documentation. The RFC 9728 protected-resource metadata and the RFC 8414\n  authorization-server metadata both resolve 200 anonymously and are saved\n  verbatim under well-known/. Exactly ONE scope is advertised. tl;dv publishes\n  no scopes/permissions reference page, so descriptions below are read from the\n  metadata and the server's capability, not from prose that does not exist.\napplies_to: mcp\ndocs: null\ndocs_note: No published OAuth scope or permissions reference page was\
  \ found.\nresource:\n  identifier: https://mcp.tldv.io/\n  name: MCP Demo Server\n  metadata_file: well-known/tl-dv-oauth-protected-resource.json\nschemes:\n  - name: MCPOAuth\n    type: oauth2\n    source: https://mcp.tldv.io/.well-known/oauth-authorization-server\n    metadata_file: well-known/tl-dv-oauth-authorization-server.json\n    issuer: https://keycloak.tldv.io/realms/mcp.tldv.io\n    implementation: Keycloak\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/auth\n        tokenUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token\n        refreshUrl: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token\n    grant_types_supported: [authorization_code, refresh_token]\n    response_types_supported:\n      - code\n      - none\n      - id_token\n      - token\n      - id_token token\n      - code id_token\n      - code token\n      - code id_token\
  \ token\n    code_challenge_methods_supported: [S256]\n    token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, none]\n    registration_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/clients-registrations/openid-connect\n    introspection_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token/introspect\n    revocation_endpoint: https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/revoke\n    dynamic_client_registration: true\n    pkce_required: true\nscopes:\n  - scope: mcp:tools\n    description: >-\n      Invoke the tools exposed by the tl;dv MCP server (list-meetings,\n      get-meeting-metadata, get-transcript, get-highlights).\n    flows: [authorizationCode]\n    sources: [well-known/tl-dv-oauth-protected-resource.json]\n    granularity: coarse\n    note: >\n      A single all-or-nothing scope covering every tool. There is no read/write\n      split and no per-resource scoping, so a token that can list\
  \ meetings can\n      also pull full transcripts of them. Worth noting for agent delegation:\n      least-privilege is not expressible on this surface.\nsummary:\n  scope_count: 1\n  oauth2_flows: [authorizationCode]\n  pkce: S256\n  dynamic_client_registration: true\nx-evidence:\n  - url: https://mcp.tldv.io/.well-known/oauth-protected-resource\n    http_status: 200\n    fetched: '2026-08-14'\n  - url: https://mcp.tldv.io/.well-known/oauth-authorization-server\n    http_status: 200\n    fetched: '2026-08-14'\n  - url: https://mcp.tldv.io/mcp\n    http_status: 401\n    fetched: '2026-08-14'\n    note: WWW-Authenticate Bearer challenge naming the resource_metadata document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tl-dv/refs/heads/main/scopes/tl-dv-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- Meetings
- Transcription
- Note Taking
- Conversation Intelligence
- Productivity
- Video
- Webhook
token_urls:
- https://keycloak.tldv.io/realms/mcp.tldv.io/protocol/openid-connect/token
---
