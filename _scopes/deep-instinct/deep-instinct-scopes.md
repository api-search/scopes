---
authorization_urls:
- https://portal.deepinstinct.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Deep Instinct Scopes
name_suffix: OAuth Scopes
note: Deep Instinct publishes no OpenAPI with oauth2 securitySchemes, so there is no spec to derive from. These scopes were read verbatim from the live RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata on portal.deepinstinct.com, which front the portal MCP server. The DSX management REST API uses an API key rather than OAuth and contributes no scopes.
overview: 'Deep Instinct publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deep Instinct API on a user''s behalf.


  Tokens are issued from https://portal.deepinstinct.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deep Instinct
provider_slug: deep-instinct
schemes:
- flows:
  - authorizationUrl: https://portal.deepinstinct.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    refreshUrl: https://portal.deepinstinct.com/oauth/token
    tokenUrl: https://portal.deepinstinct.com/oauth/token
  issuer: https://portal.deepinstinct.com
  name: portal-oauth
  source: https://portal.deepinstinct.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access through the portal MCP server. Description is not published by Deep Instinct; the scope string is verbatim from scopes_supported in both discovery documents.
  flows:
  - authorizationCode
  scope: mcp:read
- description: Write access through the portal MCP server. Description is not published by Deep Instinct; the scope string is verbatim from scopes_supported in both discovery documents.
  flows:
  - authorizationCode
  scope: mcp:write
slug: deep-instinct-scopes
source_filename: deep-instinct-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://portal.deepinstinct.com/.well-known/oauth-authorization-server\nnote: >-\n  Deep Instinct publishes no OpenAPI with oauth2 securitySchemes, so there is no spec to derive from.\n  These scopes were read verbatim from the live RFC 8414 authorization-server metadata and the RFC 9728\n  protected-resource metadata on portal.deepinstinct.com, which front the portal MCP server. The DSX\n  management REST API uses an API key rather than OAuth and contributes no scopes.\nschemes:\n- name: portal-oauth\n  type: oauth2\n  issuer: https://portal.deepinstinct.com\n  source: https://portal.deepinstinct.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://portal.deepinstinct.com/oauth/authorize\n    tokenUrl: https://portal.deepinstinct.com/oauth/token\n    refreshUrl: https://portal.deepinstinct.com/oauth/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: mcp:read\n\
  \  description: >-\n    Read access through the portal MCP server. Description is not published by Deep Instinct; the scope\n    string is verbatim from scopes_supported in both discovery documents.\n  flows: [authorizationCode]\n  sources:\n  - well-known/deep-instinct-oauth-authorization-server.json\n  - well-known/deep-instinct-oauth-protected-resource.json\n- scope: mcp:write\n  description: >-\n    Write access through the portal MCP server. Description is not published by Deep Instinct; the scope\n    string is verbatim from scopes_supported in both discovery documents.\n  flows: [authorizationCode]\n  sources:\n  - well-known/deep-instinct-oauth-authorization-server.json\n  - well-known/deep-instinct-oauth-protected-resource.json\nresource:\n  resource: https://portal.deepinstinct.com/mcp\n  authorization_servers: [https://portal.deepinstinct.com]\n  bearer_methods_supported: [header]\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://portal.deepinstinct.com/.well-known/oauth-authorization-server\n\
  \  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-instinct/refs/heads/main/scopes/deep-instinct-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- cybersecurity
- endpoint-security
- malware-prevention
- ransomware
- deep-learning
- threat-prevention
- data-security
- edr
- soc-automation
- mcp
token_urls:
- https://portal.deepinstinct.com/oauth/token
---
