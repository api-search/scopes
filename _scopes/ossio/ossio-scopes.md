---
authorization_urls: []
description: The single OAuth scope OSSIO's authorization server advertises. Read from the RFC 8414 metadata document and corroborated by the RFC 9728 protected-resource document, which advertises the same scopes_supported for the MCP endpoint. There is no published scope or permission reference page — this is the complete declared scope surface.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Ossio Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'OSSIO publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the OSSIO API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: OSSIO
provider_slug: ossio
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: Grants an OAuth client access to the OSSIO site MCP server at https://ossio.io/wp-json/mcp/mcp-oauth-server. The provider publishes no further description and no finer-grained scopes; what the scope actually permits could only be established by an authenticated tools/list introspection.
  flows: []
  scope: mcp
slug: ossio-scopes
source_filename: ossio-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://ossio.io/.well-known/oauth-authorization-server\nname: OSSIO OAuth Scopes\ndescription: >-\n  The single OAuth scope OSSIO's authorization server advertises. Read from the RFC 8414\n  metadata document and corroborated by the RFC 9728 protected-resource document, which\n  advertises the same scopes_supported for the MCP endpoint. There is no published scope\n  or permission reference page — this is the complete declared scope surface.\nauthorization_server: https://ossio.io\ndocs: null\nscopes:\n- name: mcp\n  description: >-\n    Grants an OAuth client access to the OSSIO site MCP server at\n    https://ossio.io/wp-json/mcp/mcp-oauth-server. The provider publishes no further\n    description and no finer-grained scopes; what the scope actually permits could only be\n    established by an authenticated tools/list introspection.\n  source: /.well-known/oauth-authorization-server scopes_supported\n  applies_to: https://ossio.io/wp-json/mcp/mcp-oauth-server\n\
  scope_count: 1\nnotes:\n- No sub-scopes, no read/write split, no resource-scoped grants are advertised.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ossio/refs/heads/main/scopes/ossio-scopes.yml
summary_line: 1 scope
tags:
- Company
- Medical Devices
- Health
- Orthopedics
- Life Sciences
- Manufacturing
- MCP
- Agents
token_bound: false
token_urls: []
---
