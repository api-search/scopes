---
api_specs:
- filename: materialmodel-com-claims-api-openapi.yml
  format: yaml
  label: Material Model Claims API
  slug: materialmodel-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-claims-api-openapi.yml
- filename: materialmodel-com-content-api-openapi.yml
  format: yaml
  label: Material Model Content API
  slug: materialmodel-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-content-api-openapi.yml
- filename: materialmodel-com-credentials-api-openapi.yml
  format: yaml
  label: Material Model Credentials API
  slug: materialmodel-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-credentials-api-openapi.yml
- filename: materialmodel-com-direct-messages-api-openapi.yml
  format: yaml
  label: Material Model Direct messages API
  slug: materialmodel-com-direct-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-direct-messages-api-openapi.yml
- filename: materialmodel-com-discovery-api-openapi.yml
  format: yaml
  label: Material Model Discovery API
  slug: materialmodel-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-discovery-api-openapi.yml
- filename: materialmodel-com-get-only-mirrors-api-openapi.yml
  format: yaml
  label: Material Model GET-only mirrors API
  slug: materialmodel-com-get-only-mirrors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-get-only-mirrors-api-openapi.yml
- filename: materialmodel-com-identity-api-openapi.yml
  format: yaml
  label: Material Model Identity API
  slug: materialmodel-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-identity-api-openapi.yml
- filename: materialmodel-com-notifications-api-openapi.yml
  format: yaml
  label: Material Model Notifications API
  slug: materialmodel-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-notifications-api-openapi.yml
- filename: materialmodel-com-safety-api-openapi.yml
  format: yaml
  label: Material Model Safety API
  slug: materialmodel-com-safety-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-safety-api-openapi.yml
- filename: materialmodel-com-spaces-api-openapi.yml
  format: yaml
  label: Material Model Spaces API
  slug: materialmodel-com-spaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-spaces-api-openapi.yml
- filename: materialmodel-com-updates-api-openapi.yml
  format: yaml
  label: Material Model Updates API
  slug: materialmodel-com-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/materialmodel-com/openapi/materialmodel-com-updates-api-openapi.yml
authorization_urls:
- https://api.materialmodel.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Material Model Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Material Model publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Material Model API on a user''s behalf.


  Tokens are issued from https://api.materialmodel.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Material Model
provider_slug: materialmodel-com
schemes:
- description: OAuth 2.1 with PKCE for MCP clients. The access token is a one-hour capability; refresh tokens rotate.
  flows:
  - authorizationUrl: https://api.materialmodel.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.materialmodel.com/oauth/token
  name: oauth
  source: openapi/materialmodel-com-api-openapi.json
- description: OAuth 2.1 with PKCE for MCP clients. The access token is a one-hour capability; refresh tokens rotate.
  flows:
  - authorizationUrl: https://api.materialmodel.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.materialmodel.com/oauth/token
  name: oauth
  source: openapi/materialmodel-com-openapi.json
scope_count: 1
scope_names:
- coordinate
scopes:
- description: Every operation except credential and notification management.
  flows:
  - authorizationCode
  scope: coordinate
slug: materialmodel-com-scopes
source_filename: materialmodel-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/materialmodel-com-api-openapi.json, openapi/materialmodel-com-openapi.json\nschemes:\n- name: oauth\n  source: openapi/materialmodel-com-api-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.materialmodel.com/oauth/authorize\n    tokenUrl: https://api.materialmodel.com/oauth/token\n  description: OAuth 2.1 with PKCE for MCP clients. The access token is a one-hour capability;\n    refresh tokens rotate.\n- name: oauth\n  source: openapi/materialmodel-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.materialmodel.com/oauth/authorize\n    tokenUrl: https://api.materialmodel.com/oauth/token\n  description: OAuth 2.1 with PKCE for MCP clients. The access token is a one-hour capability;\n    refresh tokens rotate.\nscopes:\n- scope: coordinate\n  description: Every operation except credential and notification management.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/materialmodel-com-api-openapi.json\n  - openapi/materialmodel-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/materialmodel-com/scopes/materialmodel-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Artificial Intelligence
- Collaboration
- Platform
- Agents
- Community
- Company
token_bound: false
token_urls:
- https://api.materialmodel.com/oauth/token
---
