---
authorization_urls: []
description: ''
docs: https://structura.tools/docs
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Structura Tools Scopes
name_suffix: OAuth Scopes
note: The docs publish no scopes reference page. The scope names were read from live discovery metadata.
overview: 'Structura publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Structura API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Structura
provider_slug: structura-tools
schemes: []
scope_count: 2
scope_names:
- mcp:tools
- mcp:assistant
scopes:
- description: Listed in scopes_supported in both the protected-resource and the authorization-server metadata. The docs do not describe it; it presumably grants access to the MCP tools.
  flows: []
  scope: mcp:tools
- description: Listed only in the protected-resource metadata scopes_supported. Not described in the docs.
  flows: []
  scope: mcp:assistant
slug: structura-tools-scopes
source_filename: structura-tools-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: https://mcp.structura.tools/.well-known/oauth-protected-resource\ndocs: https://structura.tools/docs\nscopes:\n- name: mcp:tools\n  description: Listed in scopes_supported in both the protected-resource and the authorization-server metadata. The docs do not describe it; it presumably grants access to the MCP tools.\n  source: https://mcp.structura.tools/.well-known/oauth-authorization-server\n- name: mcp:assistant\n  description: Listed only in the protected-resource metadata scopes_supported. Not described in the docs.\n  source: https://mcp.structura.tools/.well-known/oauth-protected-resource\nnote: The docs publish no scopes reference page. The scope names were read from live discovery metadata.\n"
source_yaml_url: https://artifacts.apis.io/structura-tools/scopes/structura-tools-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Code Generation
- Domain Modeling
- UML
- Software Architecture
- Low-Code
- Compliance
- MCP
token_bound: false
token_urls: []
---
