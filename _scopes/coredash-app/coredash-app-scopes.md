---
authorization_urls: []
description: ''
docs: https://www.coredash.app/core-web-vitals-mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CoreDash Scopes
name_suffix: OAuth Scopes
note: Only scope advertised in scopes_supported of both the protected-resource (HTTP 200) and authorization-server (HTTP 200) metadata. API keys (cdk_, cdk_master_) are not scope-based.
overview: 'CoreDash publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoreDash API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreDash
provider_slug: coredash-app
schemes: []
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read access to the CoreDash MCP server (RUM tools, list_projects, uptime read tools) for an OAuth connection such as Claude; OAuth tokens cannot create, change or delete monitors (403).
  flows: []
  scope: mcp:read
slug: coredash-app-scopes
source_filename: coredash-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: CoreDash OAuth scopes\ngenerated: '2026-11-04'\nmethod: probed\nsource: https://app.coredash.app/.well-known/oauth-protected-resource\ndocs: https://www.coredash.app/core-web-vitals-mcp-server\nscopes:\n- name: mcp:read\n  description: Read access to the CoreDash MCP server (RUM tools, list_projects, uptime read tools) for an OAuth connection such as Claude; OAuth tokens cannot create, change or delete monitors (403).\n  resource: https://app.coredash.app/api/mcp\nnote: Only scope advertised in scopes_supported of both the protected-resource (HTTP 200) and authorization-server (HTTP 200) metadata. API keys (cdk_, cdk_master_) are not scope-based.\n"
source_yaml_url: https://artifacts.apis.io/coredash-app/scopes/coredash-app-scopes.yml
summary_line: 1 scope
tags:
- Company
- Core Web Vitals
- Real User Monitoring
- Web Performance
- Observability
- MCP
- JSON-RPC
- AI Agents
token_bound: false
token_urls: []
---
