---
authorization_urls:
- https://www.stackadapt.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Stackadapt Scopes
name_suffix: OAuth Scopes
note: 'StackAdapt publishes no OpenAPI, so these scopes are NOT derived from a spec — they are read verbatim from the two machine-readable OAuth discovery documents StackAdapt serves. No public scopes/permissions reference page exists: docs.stackadapt.com disallows all crawlers in its robots.txt, so the descriptions below are inferred from the scope names and their resource, not quoted from StackAdapt documentation. Treat the descriptions as ours and the scope strings as theirs.'
overview: 'StackAdapt publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the StackAdapt API on a user''s behalf.


  Tokens are issued from https://www.stackadapt.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: StackAdapt
provider_slug: stackadapt
schemes:
- authorization_server: https://www.stackadapt.com/
  code_challenge_methods:
  - S256
  - plain
  dynamic_client_registration: https://www.stackadapt.com/oauth/register
  flows:
  - authorizationUrl: https://www.stackadapt.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://www.stackadapt.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://www.stackadapt.com/oauth/token
  name: MCPOAuth
  resource: https://mcp.stackadapt.com/
  source: https://mcp.stackadapt.com/.well-known/oauth-protected-resource
scope_count: 2
scope_names:
- graphql-public:read
- graphql-public:write
scopes:
- description: Read access to the StackAdapt GraphQL Public API surface via the MCP resource.
  flows:
  - authorizationCode
  - clientCredentials
  scope: graphql-public:read
- description: Write access to the StackAdapt GraphQL Public API surface via the MCP resource.
  flows:
  - authorizationCode
  - clientCredentials
  scope: graphql-public:write
slug: stackadapt-scopes
source_filename: stackadapt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://mcp.stackadapt.com/.well-known/oauth-protected-resource (RFC 9728) and\n  https://api.stackadapt.com/.well-known/oauth-authorization-server (RFC 8414)\ndocs: null\nnote: >-\n  StackAdapt publishes no OpenAPI, so these scopes are NOT derived from a spec — they are read\n  verbatim from the two machine-readable OAuth discovery documents StackAdapt serves. No public\n  scopes/permissions reference page exists: docs.stackadapt.com disallows all crawlers in its\n  robots.txt, so the descriptions below are inferred from the scope names and their resource,\n  not quoted from StackAdapt documentation. Treat the descriptions as ours and the scope\n  strings as theirs.\n\nschemes:\n- name: MCPOAuth\n  source: https://mcp.stackadapt.com/.well-known/oauth-protected-resource\n  resource: https://mcp.stackadapt.com/\n  authorization_server: https://www.stackadapt.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://www.stackadapt.com/oauth/authorize\n    tokenUrl: https://www.stackadapt.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://www.stackadapt.com/oauth/token\n  code_challenge_methods: [S256, plain]\n  dynamic_client_registration: https://www.stackadapt.com/oauth/register\n\nscopes:\n- scope: graphql-public:read\n  description: Read access to the StackAdapt GraphQL Public API surface via the MCP resource.\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - https://mcp.stackadapt.com/.well-known/oauth-protected-resource\n  - https://api.stackadapt.com/.well-known/oauth-authorization-server\n  description_provenance: inferred-from-scope-name\n- scope: graphql-public:write\n  description: Write access to the StackAdapt GraphQL Public API surface via the MCP resource.\n  flows: [authorizationCode, clientCredentials]\n  sources:\n  - https://mcp.stackadapt.com/.well-known/oauth-protected-resource\n  description_provenance: inferred-from-scope-name\n  note:\
  \ >-\n    Advertised by the MCP protected-resource metadata but NOT by the authorization server\n    metadata, whose scopes_supported lists only graphql-public:read. The two documents\n    disagree; a client should expect the authorization server to be the binding constraint.\n\ndivergence:\n  authorization_server_scopes_supported: [graphql-public:read]\n  protected_resource_scopes_supported: [graphql-public:read, graphql-public:write]\n  note: >-\n    Recorded as observed. This is a real inconsistency between StackAdapt's RFC 8414 and\n    RFC 9728 documents, not a harvesting artefact — both were fetched anonymously on\n    2026-08-13 and both returned 200.\n\nsummary:\n  scope_count: 2\n  granularity: coarse\n  note: >-\n    Two scopes cover the entire GraphQL surface (55 root queries and 97 root mutations in\n    graphql/stackadapt-schema.graphql). There is no per-resource or per-product scoping, so a\n    read token sees every campaign, advertiser, segment and pixel the account can\
  \ reach.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackadapt/refs/heads/main/scopes/stackadapt-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Programmatic Advertising
- Digital Advertising
- Campaign Management
- AdTech
- DSP
- Demand-Side Platform
- Native Advertising
- Display Advertising
- Video Advertising
- Connected TV
- Audience Targeting
- Real-Time Bidding
- Conversion Tracking
- Performance Reporting
token_urls:
- https://www.stackadapt.com/oauth/token
---
