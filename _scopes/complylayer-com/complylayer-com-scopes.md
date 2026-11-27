---
authorization_urls: []
description: ''
docs: https://complylayer.com/features/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: ComplyLayer Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ComplyLayer publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the ComplyLayer API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ComplyLayer
provider_slug: complylayer-com
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Single scope for the MCP server resource https://app.complylayer.com/api/mcp/. The docs state a connection "acts as the person who allowed it, only inside their organization". Read-only tools plus propose_use_case / propose_ai_tool, which create proposals a person must accept.
  flows: []
  scope: mcp
slug: complylayer-com-scopes
source_filename: complylayer-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource:\n- https://app.complylayer.com/.well-known/oauth-protected-resource\n- https://app.complylayer.com/.well-known/oauth-authorization-server\ndocs: https://complylayer.com/features/mcp-server\nscopes:\n- name: mcp\n  description: Single scope for the MCP server resource https://app.complylayer.com/api/mcp/. The docs state a connection \"acts as the person who allowed it, only inside their organization\". Read-only tools plus propose_use_case / propose_ai_tool, which create proposals a person must accept.\n  source: scopes_supported in both discovery documents (HTTP 200)\n"
source_yaml_url: https://artifacts.apis.io/complylayer-com/scopes/complylayer-com-scopes.yml
summary_line: 1 scope
tags:
- Company
- AI Governance
- Compliance
- EU AI Act
- Risk Management
- GDPR
- MCP
- Privacy
token_bound: false
token_urls: []
---
