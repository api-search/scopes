---
authorization_urls: []
description: ''
docs: https://convika.com/docs/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Convika Scopes
name_suffix: OAuth Scopes
note: Read from published OAuth discovery metadata (HTTP 200); the docs publish no scopes reference page.
overview: 'Convika publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Convika API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Convika
provider_slug: convika-com
schemes: []
scope_count: 2
scope_names:
- mcp:connect
- offline_access
scopes:
- description: Scope advertised in scopes_supported of the authorization-server and protected-resource metadata; grants an MCP client access to the Convika MCP tools. No per-tool scope breakdown is documented.
  flows: []
  scope: mcp:connect
- description: Advertised in scopes_supported; enables refresh tokens (refresh_token grant is supported).
  flows: []
  scope: offline_access
slug: convika-com-scopes
source_filename: convika-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.convika.com/.well-known/oauth-authorization-server\ndocs: https://convika.com/docs/\nscopes:\n- name: mcp:connect\n  description: Scope advertised in scopes_supported of the authorization-server and protected-resource metadata; grants an MCP client access to the Convika MCP tools. No per-tool scope breakdown is documented.\n- name: offline_access\n  description: Advertised in scopes_supported; enables refresh tokens (refresh_token grant is supported).\nnote: Read from published OAuth discovery metadata (HTTP 200); the docs publish no scopes reference page.\n"
source_yaml_url: https://artifacts.apis.io/convika-com/scopes/convika-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Web Hosting
- HTML Publishing
- Landing Pages
- MCP
- Artificial Intelligence
- Forms
- Analytics
token_bound: false
token_urls: []
---
