---
api_specs:
- filename: penneo-case-file-creation-api-openapi.yml
  format: yaml
  label: Penneo Case File Creation API
  slug: penneo-case-file-creation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-case-file-creation-api-openapi.yml
- filename: penneo-oauth-api-openapi.yml
  format: yaml
  label: Penneo OAuth API
  slug: penneo-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-oauth-api-openapi.yml
- filename: penneo-penneo-collect-api-api-openapi.yml
  format: yaml
  label: Penneo Penneo Collect API
  slug: penneo-penneo-collect-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-penneo-collect-api-api-openapi.yml
- filename: penneo-queue-status-check-api-openapi.yml
  format: yaml
  label: Penneo Queue Status Check API
  slug: penneo-queue-status-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-queue-status-check-api-openapi.yml
- filename: penneo-version-api-openapi.yml
  format: yaml
  label: Penneo Version API
  slug: penneo-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/penneo/openapi/penneo-version-api-openapi.yml
authorization_urls:
- https://dev.oauth.penneo.cloud/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Penneo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Penneo publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Penneo API on a user''s behalf.


  Tokens are issued from https://app.penneo.com/collect/api/swagger/oauth/forward.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Penneo
provider_slug: penneo
schemes:
- description: 'Oauth2 with Authorization Code and PKCE (Proof Key for Code Exchange) flow.

    Used in Swagger only. Please use API Grants for production integrations.'
  flows:
  - authorizationUrl: https://dev.oauth.penneo.cloud/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.penneo.com/collect/api/swagger/oauth/forward
  name: Pluto
  source: openapi/penneo-collect-api-openapi.yml
scope_count: 1
scope_names:
- full_access
scopes:
- description: Access your Penneo account
  flows:
  - authorizationCode
  scope: full_access
slug: penneo-scopes
source_filename: penneo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/penneo-collect-api-openapi.yml\nschemes:\n- name: Pluto\n  source: openapi/penneo-collect-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dev.oauth.penneo.cloud/oauth/authorize\n    tokenUrl: https://app.penneo.com/collect/api/swagger/oauth/forward\n  description: |-\n    Oauth2 with Authorization Code and PKCE (Proof Key for Code Exchange) flow.\n    Used in Swagger only. Please use API Grants for production integrations.\nscopes:\n- scope: full_access\n  description: Access your Penneo account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/penneo-collect-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/penneo/scopes/penneo-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Digital Signing
- eIDAS
- API
- Compliance
token_bound: false
token_urls:
- https://app.penneo.com/collect/api/swagger/oauth/forward
---
