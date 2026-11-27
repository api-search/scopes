---
authorization_urls: []
description: ''
docs: https://creadal.com/mcp-server/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Creadal Scopes
name_suffix: OAuth Scopes
note: scopes_supported read from RFC 8414 and RFC 9728 metadata (both HTTP 200). Descriptions paraphrase the MCP page, which states the assistant "cannot delete anything".
overview: 'Creadal publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Creadal API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Creadal
provider_slug: creadal-com
schemes: []
scope_count: 3
scope_names:
- designs:create
- designs:read
- quota:read
scopes:
- description: Make designs in the chosen workspace (the MCP page says access covers "making designs").
  flows: []
  scope: designs:create
- description: See and export your designs ("seeing and exporting your designs").
  flows: []
  scope: designs:read
- description: See your plan and remaining quota ("seeing your plan").
  flows: []
  scope: quota:read
slug: creadal-com-scopes
source_filename: creadal-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://creadal.com/.well-known/oauth-authorization-server\ndocs: https://creadal.com/mcp-server/\nscopes:\n- name: designs:create\n  description: Make designs in the chosen workspace (the MCP page says access covers \"making designs\").\n- name: designs:read\n  description: See and export your designs (\"seeing and exporting your designs\").\n- name: quota:read\n  description: See your plan and remaining quota (\"seeing your plan\").\nnote: scopes_supported read from RFC 8414 and RFC 9728 metadata (both HTTP 200). Descriptions paraphrase the MCP page, which states the assistant \"cannot delete anything\".\n"
source_yaml_url: https://artifacts.apis.io/creadal-com/scopes/creadal-com-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Design
- Templates
- Packaging
- Mockups
- Dielines
- MCP
- Graphic Design
token_bound: false
token_urls: []
---
