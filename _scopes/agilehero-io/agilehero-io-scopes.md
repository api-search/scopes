---
api_specs:
- filename: agilehero-io-account-api-openapi.yml
  format: yaml
  label: AgileHero Account API
  slug: agilehero-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-account-api-openapi.yml
- filename: agilehero-io-cards-api-openapi.yml
  format: yaml
  label: AgileHero Cards API
  slug: agilehero-io-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-cards-api-openapi.yml
- filename: agilehero-io-discovery-api-openapi.yml
  format: yaml
  label: AgileHero Discovery API
  slug: agilehero-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-discovery-api-openapi.yml
- filename: agilehero-io-projects-api-openapi.yml
  format: yaml
  label: AgileHero Projects API
  slug: agilehero-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-projects-api-openapi.yml
- filename: agilehero-io-webhooks-api-openapi.yml
  format: yaml
  label: AgileHero Webhooks API
  slug: agilehero-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agilehero-io/openapi/agilehero-io-webhooks-api-openapi.yml
authorization_urls:
- https://mcp.agilehero.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Agilehero Io Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AgileHero publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AgileHero API on a user''s behalf.


  Tokens are issued from https://mcp.agilehero.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AgileHero
provider_slug: agilehero-io
schemes:
- description: Authorization code with PKCE (S256). Send `resource=https://api.agilehero.io/v0` on the authorization and token requests.
  flows:
  - authorizationUrl: https://mcp.agilehero.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.agilehero.io/oauth/token
  name: oauth2
  source: openapi/agilehero-io-openapi.yml
scope_count: 2
scope_names:
- api:read
- api:write
scopes:
- description: Read the workspaces, projects and cards the user can access.
  flows:
  - authorizationCode
  scope: api:read
- description: Change the projects and cards the user can change, and manage webhook endpoints.
  flows:
  - authorizationCode
  scope: api:write
slug: agilehero-io-scopes
source_filename: agilehero-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/agilehero-io-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/agilehero-io-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.agilehero.io/oauth/authorize\n    tokenUrl: https://mcp.agilehero.io/oauth/token\n  description: Authorization code with PKCE (S256). Send `resource=https://api.agilehero.io/v0`\n    on the authorization and token requests.\nscopes:\n- scope: api:read\n  description: Read the workspaces, projects and cards the user can access.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/agilehero-io-openapi.yml\n- scope: api:write\n  description: Change the projects and cards the user can change, and manage webhook endpoints.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/agilehero-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/agilehero-io/scopes/agilehero-io-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Project Management
- Agile
- AI Integration
- Collaboration
token_bound: false
token_urls:
- https://mcp.agilehero.io/oauth/token
---
