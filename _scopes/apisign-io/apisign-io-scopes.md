---
api_specs:
- filename: apisign-io-api-keys-api-openapi.yml
  format: yaml
  label: APISign API Keys API
  slug: apisign-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-api-keys-api-openapi.yml
- filename: apisign-io-contracts-api-openapi.yml
  format: yaml
  label: APISign Contracts API
  slug: apisign-io-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-contracts-api-openapi.yml
- filename: apisign-io-health-api-openapi.yml
  format: yaml
  label: APISign Health API
  slug: apisign-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-health-api-openapi.yml
- filename: apisign-io-organization-api-openapi.yml
  format: yaml
  label: APISign Organization API
  slug: apisign-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-organization-api-openapi.yml
- filename: apisign-io-templates-api-openapi.yml
  format: yaml
  label: APISign Templates API
  slug: apisign-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-templates-api-openapi.yml
- filename: apisign-io-webhooks-api-openapi.yml
  format: yaml
  label: APISign Webhooks API
  slug: apisign-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apisign-io/openapi/apisign-io-webhooks-api-openapi.yml
authorization_urls:
- https://apisign.io/api/auth/oauth2/authorize
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: APISign Scopes
name_suffix: OAuth Scopes
note: These scopes govern the hosted MCP server. The REST API authenticates with an x-api-key header and declares no oauth2 securityScheme, so the REST contract carries no scope model.
overview: 'APISign publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the APISign API on a user''s behalf.


  Tokens are issued from https://apisign.io/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: APISign
provider_slug: apisign-io
schemes: []
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Lookup tools only (the four read tools).
  flows: []
  scope: read
- description: Create and send contracts and manage templates (all 12 tools).
  flows: []
  scope: write
slug: apisign-io-scopes
source_filename: apisign-io-scopes.yml
source_heading: OAuth Scopes
source_url: https://apisign.io/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-10'\nmethod: searched\nsource: https://apisign.io/.well-known/oauth-protected-resource/mcp\nsources:\n- https://apisign.io/.well-known/oauth-protected-resource/mcp\n- https://apisign.io/.well-known/oauth-authorization-server\n- https://apisign.io/docs/api/mcp\nnote: >-\n  These scopes govern the hosted MCP server. The REST API authenticates with an x-api-key header\n  and declares no oauth2 securityScheme, so the REST contract carries no scope model.\nissuer: https://apisign.io/api/auth\nauthorization_endpoint: https://apisign.io/api/auth/oauth2/authorize\ntoken_endpoint: https://apisign.io/api/auth/oauth2/token\nregistration_endpoint: https://apisign.io/api/auth/oauth2/register\nrevocation_endpoint: https://apisign.io/api/auth/oauth2/revoke\nscopes:\n  - name: read\n    description: Lookup tools only (the four read tools).\n  - name: write\n    description: Create and send contracts and manage templates (all 12 tools).\n"
source_yaml_url: https://artifacts.apis.io/apisign-io/scopes/apisign-io-scopes.yml
summary_line: 2 scopes
tags:
- E-Signature
- Artificial Intelligence
- MCP
- Contracts
- Developer Platform
token_bound: false
token_urls:
- https://apisign.io/api/auth/oauth2/token
---
