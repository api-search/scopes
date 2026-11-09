---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Entyrix Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'entyrix-com publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the entyrix-com API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: entyrix-com
provider_slug: entyrix-com
schemes: []
scope_count: 3
scope_names:
- mcp:read
- fo:read
- api:read
scopes:
- description: company data via MCP
  flows: []
  scope: mcp:read
- description: natural-person data, needs a key with a signed FO addendum
  flows: []
  scope: fo:read
- description: direct REST
  flows: []
  scope: api:read
slug: entyrix-com-scopes
source_filename: entyrix-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://entyrix.com/llms.txt\nscopes:\n  - name: \"mcp:read\"\n    description: \"company data via MCP\"\n  - name: \"fo:read\"\n    description: \"natural-person data, needs a key with a signed FO addendum\"\n  - name: \"api:read\"\n    description: \"direct REST\"\n"
source_yaml_url: https://artifacts.apis.io/entyrix-com/scopes/entyrix-com-scopes.yml
summary_line: 3 scopes
tags:
- Business Data
- Compliance
- KYC
- European
token_bound: false
token_urls: []
---
