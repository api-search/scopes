---
api_specs:
- filename: hootsuite-openapi.yml
  format: yaml
  label: Hootsuite REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/openapi/hootsuite-openapi.yml
authorization_urls:
- https://platform.hootsuite.com/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hootsuite Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Hootsuite publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Hootsuite API on a user''s behalf.


  Tokens are issued from https://platform.hootsuite.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Hootsuite
provider_slug: hootsuite
schemes:
- flows:
  - authorizationUrl: https://platform.hootsuite.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://platform.hootsuite.com/oauth2/token
  name: OAuth2
  source: openapi/hootsuite-openapi.yml
scope_count: 1
scope_names:
- offline
scopes:
- description: Issue a refresh token alongside the access token
  flows:
  - authorizationCode
  scope: offline
slug: hootsuite-scopes
source_filename: hootsuite-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hootsuite-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/hootsuite-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.hootsuite.com/oauth2/auth\n    tokenUrl: https://platform.hootsuite.com/oauth2/token\nscopes:\n- scope: offline\n  description: Issue a refresh token alongside the access token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hootsuite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hootsuite/refs/heads/main/scopes/hootsuite-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Social Media
- Social Media Management
- Marketing
- Content Scheduling
- Analytics
- Engagement
token_urls:
- https://platform.hootsuite.com/oauth2/token
---
