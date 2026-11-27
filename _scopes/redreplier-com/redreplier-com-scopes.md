---
api_specs:
- filename: redreplier-com-alerts-api-openapi.yml
  format: yaml
  label: RedReplier Alerts API
  slug: redreplier-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-alerts-api-openapi.yml
- filename: redreplier-com-keywords-api-openapi.yml
  format: yaml
  label: RedReplier Keywords API
  slug: redreplier-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-keywords-api-openapi.yml
- filename: redreplier-com-mentions-api-openapi.yml
  format: yaml
  label: RedReplier Mentions API
  slug: redreplier-com-mentions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-mentions-api-openapi.yml
- filename: redreplier-com-websites-api-openapi.yml
  format: yaml
  label: RedReplier Websites API
  slug: redreplier-com-websites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-websites-api-openapi.yml
- filename: redreplier-com-workspaces-api-openapi.yml
  format: yaml
  label: RedReplier Workspaces API
  slug: redreplier-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redreplier-com/openapi/redreplier-com-workspaces-api-openapi.yml
authorization_urls:
- https://cultured-oxygen-23.authkit.app/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: RedReplier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'RedReplier publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the RedReplier API on a user''s behalf.


  Tokens are issued from https://cultured-oxygen-23.authkit.app/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: RedReplier
provider_slug: redreplier-com
schemes:
- description: 'Authorization code flow with PKCE or a client secret. Send the access token as `Authorization: Bearer <token>`. It reaches every workspace its member belongs to: list them with `GET /workspaces` and pick one per call with the `X-Workspace-Id` header. Ask for `offline_access` to receive a refresh token'
  flows:
  - authorizationUrl: https://cultured-oxygen-23.authkit.app/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://cultured-oxygen-23.authkit.app/oauth2/token
  name: oauth2
  source: openapi/redreplier-com-openapi.json
scope_count: 4
scope_names:
- email
- offline_access
- openid
- profile
scopes:
- description: Read the member's email address
  flows:
  - authorizationCode
  scope: email
- description: Receive a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Identify the signed-in member
  flows:
  - authorizationCode
  scope: openid
- description: Read the member's name
  flows:
  - authorizationCode
  scope: profile
slug: redreplier-com-scopes
source_filename: redreplier-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/redreplier-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/redreplier-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://cultured-oxygen-23.authkit.app/oauth2/authorize\n    tokenUrl: https://cultured-oxygen-23.authkit.app/oauth2/token\n  description: 'Authorization code flow with PKCE or a client secret. Send the access token\n    as `Authorization: Bearer <token>`. It reaches every workspace its member belongs to: list\n    them with `GET /workspaces` and pick one per call with the `X-Workspace-Id` header. Ask\n    for `offline_access` to receive a refresh token'\nscopes:\n- scope: email\n  description: Read the member's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/redreplier-com-openapi.json\n- scope: offline_access\n  description: Receive a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/redreplier-com-openapi.json\n\
  - scope: openid\n  description: Identify the signed-in member\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/redreplier-com-openapi.json\n- scope: profile\n  description: Read the member's name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/redreplier-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/redreplier-com/scopes/redreplier-com-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Reddit
- Lead-Generation
- AI
- Marketing
- Sales
token_bound: false
token_urls:
- https://cultured-oxygen-23.authkit.app/oauth2/token
---
