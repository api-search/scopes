---
api_specs:
- filename: openapi.json
  format: json
  label: Fillfolio public API
  slug: fillfolio-public-api
  spec_type: OpenAPI
  url: https://fillfolio.com/openapi.json
authorization_urls: []
description: ''
docs: https://fillfolio.com/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fillfolio Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fillfolio publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fillfolio API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fillfolio
provider_slug: fillfolio-com
schemes: []
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Request this single OAuth scope for MCP access. Fillfolio assigns internal tool scopes from the approved client grant; Spending & Budgets reads require a separate per-client permission enabled by the user in Fillfolio Settings.
  flows: []
  scope: mcp:read
slug: fillfolio-com-scopes
source_filename: fillfolio-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://fillfolio.com/.well-known/oauth-protected-resource/api/mcp\ndocs: https://fillfolio.com/auth.md\nscopes:\n- name: mcp:read\n  description: >-\n    Request this single OAuth scope for MCP access. Fillfolio assigns internal\n    tool scopes from the approved client grant; Spending & Budgets reads require\n    a separate per-client permission enabled by the user in Fillfolio Settings.\n"
source_yaml_url: https://artifacts.apis.io/fillfolio-com/scopes/fillfolio-com-scopes.yml
summary_line: 1 scope
tags:
- Portfolio Tracking
- Net Worth
- Personal Finance
- Investment Tracking
- Bank Aggregation
- Crypto Wallet Tracking
- MCP
- Google Sheets Add-on
token_bound: false
token_urls: []
---
