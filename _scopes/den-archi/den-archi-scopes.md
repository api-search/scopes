---
authorization_urls: []
description: ''
docs: https://den.archi/beta.html
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Den Archi Scopes
name_suffix: OAuth Scopes
note: scopes_supported read from the OAuth authorization-server metadata (HTTP 200). The docs publish no scope reference page.
overview: 'Den publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Den API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Den
provider_slug: den-archi
schemes: []
scope_count: 1
scope_names:
- den.read
scopes:
- description: Only scope advertised by the Den authorization server; grants read access to the Den MCP knowledge tools.
  flows: []
  scope: den.read
slug: den-archi-scopes
source_filename: den-archi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: https://mcp.den.archi/.well-known/oauth-authorization-server\ndocs: https://den.archi/beta.html\nnote: scopes_supported read from the OAuth authorization-server metadata (HTTP 200). The docs publish no scope reference page.\nscopes:\n- name: den.read\n  description: Only scope advertised by the Den authorization server; grants read access to the Den MCP knowledge tools.\n"
source_yaml_url: https://artifacts.apis.io/den-archi/scopes/den-archi-scopes.yml
summary_line: 1 scope
tags:
- Company
- Architecture
- Construction
- AEC
- Building Codes
- Standards
- Knowledge Base
- MCP
- AI Agents
- South Korea
token_bound: false
token_urls: []
---
