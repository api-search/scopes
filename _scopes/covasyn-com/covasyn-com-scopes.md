---
authorization_urls: []
description: ''
docs: https://covasyn.com/en/software/docs/mcp/auth
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CovaSyn Scopes
name_suffix: OAuth Scopes
note: The docs do not publish a scopes reference page; scope names come from the documented RFC 9728 / RFC 8414 discovery documents (HTTP 200).
overview: 'CovaSyn publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the CovaSyn API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CovaSyn
provider_slug: covasyn-com
schemes: []
scope_count: 2
scope_names:
- mcp.tools.list
- mcp.tools.call
scopes:
- description: List the CovaSyn MCP tools (listed in scopes_supported of the protected-resource and authorization-server metadata).
  flows: []
  scope: mcp.tools.list
- description: Call CovaSyn MCP tools (listed in scopes_supported of the protected-resource and authorization-server metadata).
  flows: []
  scope: mcp.tools.call
slug: covasyn-com-scopes
source_filename: covasyn-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://mcp.covasyn.com/.well-known/oauth-protected-resource\ndocs: https://covasyn.com/en/software/docs/mcp/auth\nscopes:\n- name: mcp.tools.list\n  description: List the CovaSyn MCP tools (listed in scopes_supported of the protected-resource and authorization-server metadata).\n- name: mcp.tools.call\n  description: Call CovaSyn MCP tools (listed in scopes_supported of the protected-resource and authorization-server metadata).\nnote: The docs do not publish a scopes reference page; scope names come from the documented RFC 9728 / RFC 8414 discovery documents (HTTP 200).\n"
source_yaml_url: https://artifacts.apis.io/covasyn-com/scopes/covasyn-com-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Chemistry
- Pharma
- Biotechnology
- Cheminformatics
- MCP
- Artificial Intelligence
- Quality and Regulatory
token_bound: false
token_urls: []
---
