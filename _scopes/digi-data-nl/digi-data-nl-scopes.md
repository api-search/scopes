---
authorization_urls: []
description: ''
docs: https://www.digi-data.nl/en/mcp/chatgpt
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Digi Data Nl Scopes
name_suffix: OAuth Scopes
note: Scopes are taken from scopes_supported in the published OAuth metadata documents (HTTP 200). The docs do not publish a scopes reference that maps each scope; descriptions below quote only what the provider pages say about read versus manage access, and the mapping of mcp:manage to that option is our reading, not a provider statement.
overview: 'DigiData publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the DigiData API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DigiData
provider_slug: digi-data-nl
schemes: []
scope_count: 3
scope_names:
- mcp:read
- mcp:manage
- offline_access
scopes:
- description: Read access to the customer data released to the MCP connection (sources always stay read-only per /en/mcp/security).
  flows: []
  scope: mcp:read
- description: Not documented by name. The ChatGPT setup page describes an optional administrator setting letting the assistant create and modify DigiData dashboards and agent calculations, with confirmation before each change; likely the scope behind it (unconfirmed).
  flows: []
  scope: mcp:manage
- description: Standard OIDC/OAuth scope for refresh tokens (refresh_token grant is advertised).
  flows: []
  scope: offline_access
slug: digi-data-nl-scopes
source_filename: digi-data-nl-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource:\n- https://mcp.digi-data.nl/.well-known/oauth-protected-resource\n- https://mcp.digi-data.nl/.well-known/oauth-authorization-server\ndocs: https://www.digi-data.nl/en/mcp/chatgpt\nnote: Scopes are taken from scopes_supported in the published OAuth metadata documents (HTTP 200). The docs do not publish\n  a scopes reference that maps each scope; descriptions below quote only what the provider pages say about read versus manage\n  access, and the mapping of mcp:manage to that option is our reading, not a provider statement.\nscopes:\n- name: mcp:read\n  description: Read access to the customer data released to the MCP connection (sources always stay read-only per /en/mcp/security).\n- name: mcp:manage\n  description: Not documented by name. The ChatGPT setup page describes an optional administrator setting letting the assistant\n    create and modify DigiData dashboards and agent calculations, with confirmation before each change;\
  \ likely the scope behind\n    it (unconfirmed).\n- name: offline_access\n  description: Standard OIDC/OAuth scope for refresh tokens (refresh_token grant is advertised).\n"
source_yaml_url: https://artifacts.apis.io/digi-data-nl/scopes/digi-data-nl-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Business Intelligence
- Dashboards
- AI Agents
- MCP
- OData
- Power BI
- Data Integration
- Accounting
- Netherlands
token_bound: false
token_urls: []
---
