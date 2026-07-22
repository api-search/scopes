---
authorization_urls:
- https://docsend.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Docsend Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DocSend publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the DocSend API on a user''s behalf.


  Tokens are issued from https://docsend.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DocSend
provider_slug: docsend
schemes:
- flows:
  - authorizationUrl: https://docsend.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://docsend.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://docsend.com/oauth/token
  name: OAuth2
  source: well-known/docsend-oauth-authorization-server.json
scope_count: 2
scope_names:
- mcp:read
- mcp:write
scopes:
- description: Read access exposed through the DocSend hosted MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:read
- description: Write access exposed through the DocSend hosted MCP server.
  flows:
  - authorizationCode
  - clientCredentials
  scope: mcp:write
slug: docsend-scopes
source_filename: docsend-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://docsend.com/.well-known/oauth-authorization-server (scopes_supported)\n  + WWW-Authenticate scope challenge on https://mcp.docsend.com/mcp\nschemes:\n- name: OAuth2\n  source: well-known/docsend-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://docsend.com/oauth/authorize\n    tokenUrl: https://docsend.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://docsend.com/oauth/token\nscopes:\n- scope: mcp:read\n  description: Read access exposed through the DocSend hosted MCP server.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/docsend-oauth-authorization-server.json]\n- scope: mcp:write\n  description: Write access exposed through the DocSend hosted MCP server.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/docsend-oauth-authorization-server.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsend/refs/heads/main/scopes/docsend-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Company
- Enterprise
- Document Sharing
- Sales Enablement
- Analytics
- Data Room
- E-Signature
- MCP
- Dropbox
token_urls:
- https://docsend.com/oauth/token
---
