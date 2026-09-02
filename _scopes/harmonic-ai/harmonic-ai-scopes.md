---
api_specs:
- filename: harmonic-ai-companies-api-openapi.yml
  format: yaml
  label: Harmonic REST & GraphQL API
  slug: harmonic-rest-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/openapi/harmonic-ai-companies-api-openapi.yml
authorization_urls:
- https://mcp.api.harmonic.ai/authorize
description: ''
docs: https://console.harmonic.ai/docs/api-reference/introduction
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Harmonic Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Harmonic.ai publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Harmonic.ai API on a user''s behalf.


  Tokens are issued from https://mcp.api.harmonic.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Harmonic.ai
provider_slug: harmonic-ai
schemes:
- flows:
  - authorizationUrl: https://mcp.api.harmonic.ai/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.api.harmonic.ai/token
  name: oauth2
  source: well-known/harmonic-ai-mcp-oauth-authorization-server.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to Harmonic data (companies, people, investors, saved searches, lists) via the OAuth-protected MCP server.
  flows:
  - authorizationCode
  scope: read
- description: Write access — create/update lists, list entries, and custom field values via the OAuth-protected MCP server.
  flows:
  - authorizationCode
  scope: write
slug: harmonic-ai-scopes
source_filename: harmonic-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://mcp.api.harmonic.ai/.well-known/oauth-authorization-server\ndocs: https://console.harmonic.ai/docs/api-reference/introduction\nschemes:\n  - name: oauth2\n    source: well-known/harmonic-ai-mcp-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.api.harmonic.ai/authorize\n        tokenUrl: https://mcp.api.harmonic.ai/token\n        pkce: S256\nscopes:\n  - scope: read\n    description: Read access to Harmonic data (companies, people, investors, saved searches, lists) via the OAuth-protected MCP server.\n    flows: [authorizationCode]\n    sources: [well-known/harmonic-ai-mcp-oauth-authorization-server.json]\n  - scope: write\n    description: Write access — create/update lists, list entries, and custom field values via the OAuth-protected MCP server.\n    flows: [authorizationCode]\n    sources: [well-known/harmonic-ai-mcp-oauth-authorization-server.json]\n\
  notes: >-\n  Scopes are advertised by the MCP OAuth authorization-server and protected-resource metadata\n  (scopes_supported: [read, write]). The REST/GraphQL API is API-key authenticated and exposes no\n  additional OAuth scope surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic-ai/refs/heads/main/scopes/harmonic-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Startup Intelligence
- Venture Capital
- Company Data
- People Data
- investor-data
- Funding Data
- Data Enrichment
- Sales Intelligence
- Market Intelligence
- GraphQL
- MCP
- agent-native
token_urls:
- https://mcp.api.harmonic.ai/token
---
