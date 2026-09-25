---
api_specs:
- filename: tessa-tech-agent-directory-openapi.yml
  format: yaml
  label: TESSA Agent Directory API
  slug: tessa-agent-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/openapi/tessa-tech-agent-directory-openapi.yml
authorization_urls:
- https://tessa.tech/oauth/authorize
description: ''
docs: https://tessa.tech/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tessa Tech Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 scheme, so 0-working/derive-oauth-scopes.py produced nothing; this file is built from the RFC 8414 / RFC 9728 documents TESSA publishes for its WordPress MCP server. Exactly one scope is advertised and no scope reference page exists, so descriptions are as thin as the source. The anonymous MCP server on aiagent.tessa.tech has no scopes at all.
overview: 'TESSA Marketing & Technology publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TESSA Marketing & Technology API on a user''s behalf.


  Tokens are issued from https://tessa.tech/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TESSA Marketing & Technology
provider_slug: tessa-tech
schemes:
- flows:
  - authorizationUrl: https://tessa.tech/oauth/authorize
    client_auth: none (public clients)
    client_registration: client_id metadata document (client_id_metadata_document_supported true)
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://tessa.tech/oauth/token
  issuer: https://tessa.tech
  name: wordpress-mcp-oauth
  resource: https://tessa.tech/wp-json/mcp/mcp-oauth-server
  source: well-known/tessa-tech-oauth-authorization-server.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Sole scope advertised by both the authorization-server metadata (scopes_supported) and the protected-resource metadata; grants access to the WordPress MCP server. No finer-grained read/write split is published.
  flows:
  - authorizationCode
  scope: mcp
slug: tessa-tech-scopes
source_filename: tessa-tech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://tessa.tech/.well-known/oauth-authorization-server\nsource: well-known/tessa-tech-oauth-authorization-server.json + well-known/tessa-tech-oauth-protected-resource.json\nnote: >-\n  The OpenAPI declares no oauth2 scheme, so 0-working/derive-oauth-scopes.py produced nothing; this file is built\n  from the RFC 8414 / RFC 9728 documents TESSA publishes for its WordPress MCP server. Exactly one scope is\n  advertised and no scope reference page exists, so descriptions are as thin as the source. The anonymous MCP\n  server on aiagent.tessa.tech has no scopes at all.\nschemes:\n  - name: wordpress-mcp-oauth\n    issuer: https://tessa.tech\n    resource: https://tessa.tech/wp-json/mcp/mcp-oauth-server\n    source: well-known/tessa-tech-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://tessa.tech/oauth/authorize\n        tokenUrl: https://tessa.tech/oauth/token\n   \
  \     pkce: S256\n        client_auth: none (public clients)\n        client_registration: client_id metadata document (client_id_metadata_document_supported true)\nscope_count: 1\nscopes:\n  - scope: mcp\n    description: Sole scope advertised by both the authorization-server metadata (scopes_supported) and the protected-resource metadata; grants access to the WordPress MCP server. No finer-grained read/write split is published.\n    flows: [authorizationCode]\n    sources: [well-known/tessa-tech-oauth-authorization-server.json, well-known/tessa-tech-oauth-protected-resource.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/scopes/tessa-tech-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Digital Marketing
- SEO
- Web Development
- Accessibility
- AI Agent Readiness
- Professional Services
- Agent Directory
- A2A
- MCP
- Agent-Native
- Company
token_urls:
- https://tessa.tech/oauth/token
---
