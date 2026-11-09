---
authorization_urls: []
description: ''
docs: https://dilohost.es/docs/referencia/servidor-mcp
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Dilohost Es Scopes
name_suffix: OAuth Scopes
note: Single scope documented in the MCP server reference and in the documented protected-resource metadata (scopes_supported). Authorization is otherwise role-based (owner vs team member), see https://dilohost.es/docs/cuenta/equipo.
overview: 'Dilohost publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Dilohost API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dilohost
provider_slug: dilohost-es
schemes: []
scope_count: 1
scope_names:
- mcp:use
scopes:
- description: Use the Dilohost MCP server. A token without this scope receives 403 insufficient_scope.
  flows: []
  scope: mcp:use
slug: dilohost-es-scopes
source_filename: dilohost-es-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dilohost.es/docs/referencia/servidor-mcp\ndocs: https://dilohost.es/docs/referencia/servidor-mcp\nname: Dilohost OAuth scopes\nnote: Single scope documented in the MCP server reference and in the documented protected-resource metadata (scopes_supported). Authorization is otherwise role-based (owner vs team member), see https://dilohost.es/docs/cuenta/equipo.\nscopes:\n- name: mcp:use\n  description: Use the Dilohost MCP server. A token without this scope receives 403 insufficient_scope.\n"
source_yaml_url: https://artifacts.apis.io/dilohost-es/scopes/dilohost-es-scopes.yml
summary_line: 1 scope
tags:
- Company
- Hosting
- Web Hosting
- MCP
- AI Agents
- Database
- Domains
- Email
- European Union
token_bound: false
token_urls: []
---
