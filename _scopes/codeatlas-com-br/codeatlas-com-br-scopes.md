---
api_specs:
- filename: codeatlas-com-br-contact-api-openapi.yml
  format: yaml
  label: CodeAtlas Contact API
  slug: codeatlas-com-br-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-contact-api-openapi.yml
- filename: codeatlas-com-br-discovery-api-openapi.yml
  format: yaml
  label: CodeAtlas Discovery API
  slug: codeatlas-com-br-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-discovery-api-openapi.yml
- filename: codeatlas-com-br-exports-api-openapi.yml
  format: yaml
  label: CodeAtlas Exports API
  slug: codeatlas-com-br-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-exports-api-openapi.yml
- filename: codeatlas-com-br-oauth-api-openapi.yml
  format: yaml
  label: CodeAtlas OAuth API
  slug: codeatlas-com-br-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-oauth-api-openapi.yml
- filename: codeatlas-com-br-system-api-openapi.yml
  format: yaml
  label: CodeAtlas System API
  slug: codeatlas-com-br-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeatlas-com-br/openapi/codeatlas-com-br-system-api-openapi.yml
authorization_urls: []
description: ''
docs: https://codeatlas.com.br/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: CodeAtlas Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CodeAtlas publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CodeAtlas API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CodeAtlas
provider_slug: codeatlas-com-br
schemes: []
scope_count: 1
scope_names:
- api:write
scopes:
- description: Create contact requests and exports. The only scope (scopes_supported in both protected-resource and authorization-server metadata); token requests default to it, any other value returns invalid_scope.
  flows:
  - clientCredentials
  - urn:workos:agent-auth:grant-type:claim
  scope: api:write
slug: codeatlas-com-br-scopes
source_filename: codeatlas-com-br-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://codeatlas.com.br/auth.md\ndocs: https://codeatlas.com.br/auth.md\nscopes:\n- scope: api:write\n  description: Create contact requests and exports. The only scope (scopes_supported in both protected-resource\n    and authorization-server metadata); token requests default to it, any other value returns invalid_scope.\n  flows:\n  - clientCredentials\n  - urn:workos:agent-auth:grant-type:claim\n  sources:\n  - openapi/codeatlas-com-br-openapi.yml\n  - https://codeatlas.com.br/auth.md\n"
source_yaml_url: https://artifacts.apis.io/codeatlas-com-br/scopes/codeatlas-com-br-scopes.yml
summary_line: 1 scope
tags:
- Company
- Software Development
- Developer Tools
- AI Agents
- MCP
- Custom Software
- Brazil
token_bound: false
token_urls: []
---
