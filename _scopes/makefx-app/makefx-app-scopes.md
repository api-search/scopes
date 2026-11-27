---
api_specs:
- filename: makefx-app-asset-api-openapi.yml
  format: yaml
  label: makefx Asset API
  slug: makefx-app-asset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-asset-api-openapi.yml
- filename: makefx-app-auth-api-openapi.yml
  format: yaml
  label: makefx Auth API
  slug: makefx-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-auth-api-openapi.yml
- filename: makefx-app-link-api-openapi.yml
  format: yaml
  label: makefx Link API
  slug: makefx-app-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-link-api-openapi.yml
- filename: makefx-app-models-api-openapi.yml
  format: yaml
  label: makefx Models API
  slug: makefx-app-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-models-api-openapi.yml
- filename: makefx-app-oauth-api-openapi.yml
  format: yaml
  label: makefx OAuth API
  slug: makefx-app-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-oauth-api-openapi.yml
- filename: makefx-app-p-api-openapi.yml
  format: yaml
  label: makefx P API
  slug: makefx-app-p-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-p-api-openapi.yml
- filename: makefx-app-service-api-openapi.yml
  format: yaml
  label: makefx Service API
  slug: makefx-app-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-service-api-openapi.yml
- filename: makefx-app-space-api-openapi.yml
  format: yaml
  label: makefx Space API
  slug: makefx-app-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-space-api-openapi.yml
- filename: makefx-app-user-api-openapi.yml
  format: yaml
  label: makefx User API
  slug: makefx-app-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makefx-app/openapi/makefx-app-user-api-openapi.yml
authorization_urls:
- https://makefx.app/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: makefx Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'makefx publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the makefx API on a user''s behalf.


  Tokens are issued from https://makefx.app/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: makefx
provider_slug: makefx-app
schemes:
- description: 'OAuth 2.1 authorization code with PKCE (S256), issued by this deployment. Register a client at the registration endpoint or present a Client ID Metadata Document, then send the person to authorize. Metadata: /.well-known/oauth-authorization-server.'
  flows:
  - authorizationUrl: https://makefx.app/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://makefx.app/api/oauth/token
  name: oauth2
  source: openapi/makefx-app-openapi.json
scope_count: 5
scope_names:
- email
- openid
- profile
- read
- write
scopes:
- description: See your email address
  flows:
  - authorizationCode
  scope: email
- description: Confirm who you are
  flows:
  - authorizationCode
  scope: openid
- description: See your name
  flows:
  - authorizationCode
  scope: profile
- description: Read your data
  flows:
  - authorizationCode
  scope: read
- description: Change your data on your behalf
  flows:
  - authorizationCode
  scope: write
slug: makefx-app-scopes
source_filename: makefx-app-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/makefx-app-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/makefx-app-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://makefx.app/api/oauth/authorize\n    tokenUrl: https://makefx.app/api/oauth/token\n  description: 'OAuth 2.1 authorization code with PKCE (S256), issued by this deployment. Register\n    a client at the registration endpoint or present a Client ID Metadata Document, then send\n    the person to authorize. Metadata: /.well-known/oauth-authorization-server.'\nscopes:\n- scope: email\n  description: See your email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/makefx-app-openapi.json\n- scope: openid\n  description: Confirm who you are\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/makefx-app-openapi.json\n- scope: profile\n  description: See your name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/makefx-app-openapi.json\n\
  - scope: read\n  description: Read your data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/makefx-app-openapi.json\n- scope: write\n  description: Change your data on your behalf\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/makefx-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/makefx-app/scopes/makefx-app-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Artificial Intelligence
- Media
- Platform
- Creators
- Payments
token_bound: false
token_urls:
- https://makefx.app/api/oauth/token
---
