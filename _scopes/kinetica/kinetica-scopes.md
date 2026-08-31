---
authorization_urls:
- https://app.toolbelt.ai/oauth/authorize
description: ''
docs: https://www.kinetica.com/agents
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Kinetica Scopes
name_suffix: OAuth Scopes
note: Kinetica's database REST API uses HTTP Basic / bearer tokens and has no OAuth scope surface. The scopes below belong to the Toolbelt MCP server, and were read from live RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata — not from documentation prose.
overview: 'Kinetica publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kinetica API on a user''s behalf.


  Tokens are issued from https://app.toolbelt.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kinetica
provider_slug: kinetica
schemes:
- flows:
  - authorizationUrl: https://app.toolbelt.ai/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://app.toolbelt.ai/oauth/register
    tokenUrl: https://app.toolbelt.ai/oauth/token
  issuer: https://app.toolbelt.ai
  name: toolbeltOAuth2
  source: well-known/kinetica-toolbelt-oauth-authorization-server.json
  surface: Kinetica Toolbelt MCP Server
scope_count: 2
scope_names:
- mcp:tools
- openid
scopes:
- description: Invoke the Toolbelt MCP tools (toolbelt_sql, toolbelt_vector_search, toolbelt_graph_traversal, toolbelt_schema_introspection, toolbelt_ingestion_job_inspection) against the connected Kinetica database.
  flows:
  - authorizationCode
  scope: mcp:tools
- description: OpenID Connect subject identity for the authenticated Toolbelt user.
  flows:
  - authorizationCode
  scope: openid
slug: kinetica-scopes
source_filename: kinetica-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://app.toolbelt.ai/.well-known/oauth-authorization-server\ndocs: https://www.kinetica.com/agents\nnote: Kinetica's database REST API uses HTTP Basic / bearer tokens and has no OAuth\n  scope surface. The scopes below belong to the Toolbelt MCP server, and were read\n  from live RFC 8414 authorization-server metadata and RFC 9728 protected-resource\n  metadata — not from documentation prose.\nschemes:\n- name: toolbeltOAuth2\n  surface: Kinetica Toolbelt MCP Server\n  source: well-known/kinetica-toolbelt-oauth-authorization-server.json\n  issuer: https://app.toolbelt.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.toolbelt.ai/oauth/authorize\n    tokenUrl: https://app.toolbelt.ai/oauth/token\n    registrationUrl: https://app.toolbelt.ai/oauth/register\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: mcp:tools\n  description: Invoke the Toolbelt MCP tools (toolbelt_sql, toolbelt_vector_search,\n\
  \    toolbelt_graph_traversal, toolbelt_schema_introspection, toolbelt_ingestion_job_inspection)\n    against the connected Kinetica database.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kinetica-toolbelt-oauth-authorization-server.json\n  - well-known/kinetica-toolbelt-oauth-protected-resource.json\n  advertised_on_resource: true\n- scope: openid\n  description: OpenID Connect subject identity for the authenticated Toolbelt user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/kinetica-toolbelt-oauth-authorization-server.json\n  advertised_on_resource: false\nprotected_resources:\n- resource: https://mcp.toolbelt.ai/mcp\n  authorization_servers:\n  - https://app.toolbelt.ai\n  scopes_supported:\n  - mcp:tools\n  bearer_methods_supported:\n  - header\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://app.toolbelt.ai/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - url: https://mcp.toolbelt.ai/.well-known/oauth-protected-resource\n\
  \    http_status: 200\n    content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinetica/refs/heads/main/scopes/kinetica-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Database
- Analytics
- gpu-acceleration
- real-time-analytics
- vector-search
- graph-analytics
- geospatial
- time-series
- SQL
- streaming
- data-infrastructure
- MCP
- agent-native
- RAG
token_urls:
- https://app.toolbelt.ai/oauth/token
---
