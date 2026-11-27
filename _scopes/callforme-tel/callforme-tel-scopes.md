---
api_specs:
- filename: callforme-tel-account-api-openapi.yml
  format: yaml
  label: CallForMe Account API
  slug: callforme-tel-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-account-api-openapi.yml
- filename: callforme-tel-batches-api-openapi.yml
  format: yaml
  label: CallForMe Batches API
  slug: callforme-tel-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-batches-api-openapi.yml
- filename: callforme-tel-businesses-api-openapi.yml
  format: yaml
  label: CallForMe Businesses API
  slug: callforme-tel-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-businesses-api-openapi.yml
- filename: callforme-tel-calls-api-openapi.yml
  format: yaml
  label: CallForMe Calls API
  slug: callforme-tel-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-calls-api-openapi.yml
- filename: callforme-tel-pricing-api-openapi.yml
  format: yaml
  label: CallForMe Pricing API
  slug: callforme-tel-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-pricing-api-openapi.yml
- filename: callforme-tel-setups-api-openapi.yml
  format: yaml
  label: CallForMe Setups API
  slug: callforme-tel-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callforme-tel/openapi/callforme-tel-setups-api-openapi.yml
authorization_urls: []
description: ''
docs: https://callforme.tel/docs/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: CallForMe Scopes
name_suffix: OAuth Scopes
note: Read from the saved discovery documents (fetched by GET); no OAuth endpoint was called. The MCP docs describe "standard MCP authorization (OAuth)" and publish no scopes reference page.
overview: 'CallForMe publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the CallForMe API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CallForMe
provider_slug: callforme-tel
schemes: []
scope_count: 1
scope_names:
- calls
scopes:
- description: The single scope advertised in scopes_supported by both the protected-resource metadata for https://callforme.tel/mcp and the authorization-server metadata. Its meaning is not described in the docs.
  flows: []
  scope: calls
slug: callforme-tel-scopes
source_filename: callforme-tel-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource:\n- https://callforme.tel/.well-known/oauth-protected-resource\n- https://callforme.tel/.well-known/oauth-authorization-server\ndocs: https://callforme.tel/docs/mcp\nsurface: MCP (https://callforme.tel/mcp); the REST OpenAPI declares only a bearer key scheme, no oauth2 scopes.\nscopes:\n- name: calls\n  description: The single scope advertised in scopes_supported by both the protected-resource metadata for https://callforme.tel/mcp and the authorization-server metadata. Its meaning is not described in the docs.\n  sources:\n  - well-known/callforme-tel-oauth-protected-resource.json\n  - well-known/callforme-tel-oauth-authorization-server.json\nnote: Read from the saved discovery documents (fetched by GET); no OAuth endpoint was called. The MCP docs describe \"standard MCP authorization (OAuth)\" and publish no scopes reference page.\n"
source_yaml_url: https://artifacts.apis.io/callforme-tel/scopes/callforme-tel-scopes.yml
summary_line: 1 scope
tags:
- Company
- AI Agents
- Voice
- Phone Calls
- Telephony
- MCP
- REST API
token_bound: false
token_urls: []
---
