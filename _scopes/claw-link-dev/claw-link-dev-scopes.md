---
api_specs:
- filename: claw-link-dev-discovery-api-openapi.yml
  format: yaml
  label: ClawLink Discovery API
  slug: claw-link-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-discovery-api-openapi.yml
- filename: claw-link-dev-execution-api-openapi.yml
  format: yaml
  label: ClawLink Execution API
  slug: claw-link-dev-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-execution-api-openapi.yml
- filename: claw-link-dev-mcp-api-openapi.yml
  format: yaml
  label: ClawLink MCP API
  slug: claw-link-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-mcp-api-openapi.yml
- filename: claw-link-dev-registration-api-openapi.yml
  format: yaml
  label: ClawLink Registration API
  slug: claw-link-dev-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/claw-link-dev/openapi/claw-link-dev-registration-api-openapi.yml
authorization_urls:
- https://clerk.claw-link.dev/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Claw Link Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ClawLink publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClawLink API on a user''s behalf.


  Tokens are issued from https://clerk.claw-link.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClawLink
provider_slug: claw-link-dev
schemes:
- description: For remote MCP clients calling /api/mcp. Discovery starts at https://claw-link.dev/.well-known/oauth-protected-resource; client registration follows the authorization server metadata.
  flows:
  - authorizationUrl: https://clerk.claw-link.dev/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.claw-link.dev/oauth/token
  name: OAuth2
  source: openapi/claw-link-dev-openapi.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Read the user's email address
  flows:
  - authorizationCode
  scope: email
- description: Identify the authorizing user
  flows:
  - authorizationCode
  scope: openid
- description: Read basic profile information
  flows:
  - authorizationCode
  scope: profile
slug: claw-link-dev-scopes
source_filename: claw-link-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/claw-link-dev-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/claw-link-dev-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.claw-link.dev/oauth/authorize\n    tokenUrl: https://clerk.claw-link.dev/oauth/token\n  description: For remote MCP clients calling /api/mcp. Discovery starts at https://claw-link.dev/.well-known/oauth-protected-resource;\n    client registration follows the authorization server metadata.\nscopes:\n- scope: email\n  description: Read the user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/claw-link-dev-openapi.json\n- scope: openid\n  description: Identify the authorizing user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/claw-link-dev-openapi.json\n- scope: profile\n  description: Read basic profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/claw-link-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/claw-link-dev/scopes/claw-link-dev-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Artificial Intelligence
- Integration
- Automation
- Productivity
- Developer Tools
token_bound: false
token_urls:
- https://clerk.claw-link.dev/oauth/token
---
