---
authorization_urls: []
description: ''
docs: https://www.glaciergrid.com/connector
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Hello Therma Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hello Therma uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hello Therma
provider_slug: hello-therma
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: hello-therma-scopes
source_filename: hello-therma-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://mcp.glaciergrid.com/.well-known/oauth-authorization-server\ndocs: https://www.glaciergrid.com/connector\nsummary: >-\n  GlacierGrid's MCP authorization server advertises exactly two scopes. There is no published\n  scopes/permissions reference page on the marketing site or the help center, so the\n  descriptions below are inferred ONLY from the names plus the access statements GlacierGrid\n  publishes on its connector page; they are marked as such and are not vendor copy.\nauthorization_server: https://mcp.glaciergrid.com/\nprotected_resources:\n- https://mcp.glaciergrid.com/\n- https://mcp.glaciergrid.com/mcp\nscope_count: 2\nscopes:\n- name: customer\n  description_source: not-published\n  inferred_meaning: >-\n    Customer-facing access to the authenticated account's own facility data. GlacierGrid\n    states \"Access is scoped to the locations your account already covers. The connector\n    shows you nothing beyond\
  \ what your GlacierGrid login already grants.\"\n  access: read-only\n  evidence: https://www.glaciergrid.com/connector\n- name: internal\n  description_source: not-published\n  inferred_meaning: >-\n    Not documented publicly. The name suggests a GlacierGrid-internal audience rather than a\n    customer one; no published material describes it.\n  access: unknown\n  evidence: https://mcp.glaciergrid.com/.well-known/oauth-authorization-server\ngaps:\n- >-\n  No scope reference page exists. A customer or an agent developer cannot learn what\n  `internal` grants, nor whether `customer` is required for every tool, without contacting\n  support@glaciergrid.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-therma/refs/heads/main/scopes/hello-therma-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Internet of Things
- Energy
- Sustainability
- Cold Chain
- Temperature Monitoring
- Refrigeration
- HVAC
- Building Automation
- Food Safety
- Facilities Management
- Restaurants
- Retail
- Model Context Protocol
- Agents
token_urls: []
---
