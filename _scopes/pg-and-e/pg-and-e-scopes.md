---
authorization_urls:
- https://api.pge.com/datacustodian/oauth/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pg And E Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'pg-and-e publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the pg-and-e API on a user''s behalf.


  Tokens are issued from https://api.pge.com/datacustodian/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: pg-and-e
provider_slug: pg-and-e
schemes:
- flows:
  - authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/authorize
    flow: authorizationCode
    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token
  name: oauth2
  source: openapi/pg-and-e-share-my-data-api-openapi.yml
scope_count: 1
scope_names:
- usage:read
scopes:
- description: Read energy usage data
  flows:
  - authorizationCode
  scope: usage:read
slug: pg-and-e-scopes
source_filename: pg-and-e-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pg-and-e-share-my-data-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pg-and-e-share-my-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.pge.com/datacustodian/oauth/v2/authorize\n    tokenUrl: https://api.pge.com/datacustodian/oauth/v2/token\nscopes:\n- scope: usage:read\n  description: Read energy usage data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pg-and-e-share-my-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pg-and-e/refs/heads/main/scopes/pg-and-e-scopes.yml
summary_line: 1 scope · authorizationCode
tags: []
token_urls:
- https://api.pge.com/datacustodian/oauth/v2/token
---
