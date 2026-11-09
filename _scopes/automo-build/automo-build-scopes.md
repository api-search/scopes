---
api_specs:
- filename: automo-build-agent-api-openapi.yml
  format: yaml
  label: Automo Agent API
  slug: automo-build-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-agent-api-openapi.yml
- filename: automo-build-mcp-api-openapi.yml
  format: yaml
  label: Automo MCP API
  slug: automo-build-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-mcp-api-openapi.yml
- filename: automo-build-oauth-api-openapi.yml
  format: yaml
  label: Automo OAuth API
  slug: automo-build-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-oauth-api-openapi.yml
- filename: automo-build-openapi-json-api-openapi.yml
  format: yaml
  label: Automo Openapi.json API
  slug: automo-build-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-openapi-json-api-openapi.yml
- filename: automo-build-well-known-api-openapi.yml
  format: yaml
  label: Automo .well Known API
  slug: automo-build-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/automo-build/openapi/automo-build-well-known-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Automo Build Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Automo uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Automo
provider_slug: automo-build
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: automo-build-scopes
source_filename: automo-build-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://automo.build/auth.md\nscopes:\n  - workspaces:read\n  - projects:read\n  - projects:write\n  - prompts:write\n  - sessions:read\n  - sessions:write\n  - reviews:read\n  - reviews:write\n  - playbooks:read\n  - playbooks:run\n  - playbooks:write\n  - deployments:read\n  - deployments:write\n  - chat:read\n  - billing:write\n"
source_yaml_url: https://artifacts.apis.io/automo-build/scopes/automo-build-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Platform
- Low-Code
- Automation
- Software Development
token_bound: false
token_urls: []
---
