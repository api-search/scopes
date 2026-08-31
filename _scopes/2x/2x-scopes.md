---
api_specs:
- filename: 2x-alignment-api-openapi.yml
  format: yaml
  label: 2X Alignment API
  slug: 2x-alignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-alignment-api-openapi.yml
- filename: 2x-api-keys-api-openapi.yml
  format: yaml
  label: 2X API Keys API
  slug: 2x-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-api-keys-api-openapi.yml
- filename: 2x-clients-api-openapi.yml
  format: yaml
  label: 2X Clients API
  slug: 2x-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-clients-api-openapi.yml
- filename: 2x-documentation-api-openapi.yml
  format: yaml
  label: 2X Documentation API
  slug: 2x-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-documentation-api-openapi.yml
- filename: 2x-health-api-openapi.yml
  format: yaml
  label: 2X Health API
  slug: 2x-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-health-api-openapi.yml
- filename: 2x-portfolios-api-openapi.yml
  format: yaml
  label: 2X Portfolios API
  slug: 2x-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-portfolios-api-openapi.yml
- filename: 2x-root-api-openapi.yml
  format: yaml
  label: 2X Root API
  slug: 2x-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-root-api-openapi.yml
- filename: 2x-status-api-openapi.yml
  format: yaml
  label: 2X Status API
  slug: 2x-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-status-api-openapi.yml
- filename: 2x-streams-api-openapi.yml
  format: yaml
  label: 2X Streams API
  slug: 2x-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-streams-api-openapi.yml
- filename: 2x-topics-api-openapi.yml
  format: yaml
  label: 2X Topics API
  slug: 2x-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/openapi/2x-topics-api-openapi.yml
authorization_urls:
- https://mcp.knownwell.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: 2X Scopes
name_suffix: OAuth Scopes
note: The OpenAPI for the Knownwell REST API declares no oauth2 security scheme, so derive-oauth-scopes.py found nothing there. The OAuth surface belongs to the remote MCP server on mcp.knownwell.com, whose RFC 8414 authorization-server metadata publishes the scope list below. Recorded from that live document, not from the spec. 2X publishes no human-readable scopes reference page, so the descriptions are the plain reading of the scope name and are marked as such.
overview: '2X publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 2X API on a user''s behalf.


  Tokens are issued from https://mcp.knownwell.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 2X
provider_slug: 2x
schemes:
- flows:
  - authorizationUrl: https://mcp.knownwell.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.knownwell.com/token
  issuer: https://mcp.knownwell.com/
  name: KnownwellMCPOAuth
  protected_resource: https://mcp.knownwell.com/mcp
  source: well-known/2x-oauth-authorization-server.json
scope_count: 1
scope_names:
- knownwell.read
scopes:
- description: Read access to Knownwell commercial-intelligence data. The only scope the authorization server advertises; description inferred from the scope name because no scopes reference page is published.
  flows:
  - authorizationCode
  scope: knownwell.read
slug: 2x-scopes
source_filename: 2x-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.knownwell.com/.well-known/oauth-authorization-server\nnote: >-\n  The OpenAPI for the Knownwell REST API declares no oauth2 security scheme, so\n  derive-oauth-scopes.py found nothing there. The OAuth surface belongs to the remote MCP\n  server on mcp.knownwell.com, whose RFC 8414 authorization-server metadata publishes the\n  scope list below. Recorded from that live document, not from the spec. 2X publishes no\n  human-readable scopes reference page, so the descriptions are the plain reading of the\n  scope name and are marked as such.\nschemes:\n- name: KnownwellMCPOAuth\n  source: well-known/2x-oauth-authorization-server.json\n  issuer: https://mcp.knownwell.com/\n  protected_resource: https://mcp.knownwell.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.knownwell.com/authorize\n    tokenUrl: https://mcp.knownwell.com/token\n    pkce: S256\nscopes:\n- scope: knownwell.read\n \
  \ description: >-\n    Read access to Knownwell commercial-intelligence data. The only scope the authorization\n    server advertises; description inferred from the scope name because no scopes reference\n    page is published.\n  description_source: inferred-from-name\n  flows: [authorizationCode]\n  sources: [well-known/2x-oauth-authorization-server.json]\nsummary:\n  scope_count: 1\n  write_scopes: 0\n  note: >-\n    A single read-only scope, consistent with the REST API being entirely GET operations\n    apart from API-key administration.\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://mcp.knownwell.com/.well-known/oauth-authorization-server\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2x/refs/heads/main/scopes/2x-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Marketing
- Marketing as a Service
- B2B
- MarTech
- Marketing Operations
- Consulting
- Artificial Intelligence
- Go-To-Market
- Revenue Operations
- Commercial Intelligence
- Customer Success
- Agentic AI
- Demand Generation
token_urls:
- https://mcp.knownwell.com/token
---
