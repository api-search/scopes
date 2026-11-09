---
api_specs:
- filename: carryo-io-health-api-openapi.yml
  format: yaml
  label: Carryo Health API
  slug: carryo-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-health-api-openapi.yml
- filename: carryo-io-mcp-api-openapi.yml
  format: yaml
  label: Carryo MCP API
  slug: carryo-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-mcp-api-openapi.yml
- filename: carryo-io-well-known-api-openapi.yml
  format: yaml
  label: Carryo .well Known API
  slug: carryo-io-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/carryo-io/openapi/carryo-io-well-known-api-openapi.yml
authorization_urls:
- https://mcp.carryo.io/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Carryo Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Carryo publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Carryo API on a user''s behalf.


  Tokens are issued from https://mcp.carryo.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Carryo
provider_slug: carryo-io
schemes:
- description: OAuth 2.1 authorization code flow with PKCE and least-privilege website permissions.
  flows:
  - authorizationUrl: https://mcp.carryo.io/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.carryo.io/token
  name: carryoOAuth
  source: openapi/carryo-io-openapi.json
scope_count: 3
scope_names:
- artifact.read
- artifact.revoke
- artifact.write
scopes:
- description: Read publishing availability, websites, drafts, version history, and authorized form responses.
  flows:
  - authorizationCode
  scope: artifact.read
- description: Take a published website offline.
  flows:
  - authorizationCode
  scope: artifact.revoke
- description: Save drafts, publish websites, edit websites, and manage images.
  flows:
  - authorizationCode
  scope: artifact.write
slug: carryo-io-scopes
source_filename: carryo-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/carryo-io-openapi.json\nschemes:\n- name: carryoOAuth\n  source: openapi/carryo-io-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.carryo.io/authorize\n    tokenUrl: https://mcp.carryo.io/token\n  description: OAuth 2.1 authorization code flow with PKCE and least-privilege website permissions.\nscopes:\n- scope: artifact.read\n  description: Read publishing availability, websites, drafts, version history, and authorized\n    form responses.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/carryo-io-openapi.json\n- scope: artifact.revoke\n  description: Take a published website offline.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/carryo-io-openapi.json\n- scope: artifact.write\n  description: Save drafts, publish websites, edit websites, and manage images.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/carryo-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/carryo-io/scopes/carryo-io-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Artificial Intelligence
- Website Publishing
- Content Generation
- Software-as-a-Service
- Low-Code
token_bound: false
token_urls:
- https://mcp.carryo.io/token
---
