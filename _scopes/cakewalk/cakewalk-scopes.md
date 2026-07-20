---
authorization_urls: []
description: ''
docs: https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cakewalk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cakewalk publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cakewalk API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cakewalk
provider_slug: cakewalk
schemes:
- flows:
  - flow: authorizationCode
    server: https://mcp.getcakewalk.io/mcp
  name: OAuth2
  source: https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp
scope_count: 4
scope_names:
- mcp:users.read
- mcp:workapps.read
- mcp:requests.read
- mcp:requests.write
scopes:
- description: Read user profiles, directory, and access details via MCP user tools.
  flows:
  - authorizationCode
  scope: mcp:users.read
- description: Read managed work apps, permission levels, and custom fields via MCP app tools.
  flows:
  - authorizationCode
  scope: mcp:workapps.read
- description: Read recent and open access requests via MCP request tools.
  flows:
  - authorizationCode
  scope: mcp:requests.read
- description: Create or modify access requests via MCP request tools. Reserved for write-capable request tools during MCP authorization.
  flows:
  - authorizationCode
  scope: mcp:requests.write
slug: cakewalk-scopes
source_filename: cakewalk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference\ndocs: https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference\nnotes: >-\n  OAuth scopes apply to the hosted Cakewalk MCP server\n  (https://mcp.getcakewalk.io/mcp). Scopes are approved during the OAuth\n  authorization flow and gate which MCP tools an agent can call. The REST Open\n  API itself authenticates with X-API-KEY / X-API-SECRET headers (see\n  authentication/cakewalk-authentication.yml) and has no OAuth scopes.\nschemes:\n- name: OAuth2\n  source: https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp\n  flows:\n  - flow: authorizationCode\n    server: https://mcp.getcakewalk.io/mcp\nscopes:\n- scope: mcp:users.read\n  description: Read user profiles, directory, and access details via MCP user tools.\n  flows: [authorizationCode]\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference]\n\
  - scope: mcp:workapps.read\n  description: Read managed work apps, permission levels, and custom fields via MCP app tools.\n  flows: [authorizationCode]\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference]\n- scope: mcp:requests.read\n  description: Read recent and open access requests via MCP request tools.\n  flows: [authorizationCode]\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference]\n- scope: mcp:requests.write\n  description: >-\n    Create or modify access requests via MCP request tools. Reserved for\n    write-capable request tools during MCP authorization.\n  flows: [authorizationCode]\n  sources: [https://www.cakewalk.security/docs/open-api-and-mcp/introduction-to-mcp/mcp-tool-reference]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cakewalk/refs/heads/main/scopes/cakewalk-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Access Management
- Identity Governance
- IGA
- AI Agents
- Security
- Access Control
- MCP
- Provisioning
- SaaS Management
- Authentication
token_urls: []
---
