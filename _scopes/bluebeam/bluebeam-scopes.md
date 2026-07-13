---
api_specs:
- filename: bluebeam-studio-openapi.yml
  format: yaml
  label: Bluebeam Studio API
  slug: bluebeam-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/openapi/bluebeam-studio-openapi.yml
authorization_urls:
- https://authserver.bluebeam.com/auth/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bluebeam Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'bluebeam publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the bluebeam API on a user''s behalf.


  Tokens are issued from https://authserver.bluebeam.com/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: bluebeam
provider_slug: bluebeam
schemes:
- flows:
  - authorizationUrl: https://authserver.bluebeam.com/auth/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://authserver.bluebeam.com/auth/oauth/token
  name: oauth2
  source: openapi/bluebeam-studio-openapi.yml
scope_count: 3
scope_names:
- full
- jobs.create
- jobs.read
scopes:
- description: Full access to Bluebeam Studio API
  flows:
  - authorizationCode
  scope: full
- description: Create and manage sessions
  flows:
  - authorizationCode
  scope: jobs.create
- description: Read session data
  flows:
  - authorizationCode
  scope: jobs.read
slug: bluebeam-scopes
source_filename: bluebeam-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bluebeam-studio-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bluebeam-studio-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authserver.bluebeam.com/auth/oauth/authorize\n    tokenUrl: https://authserver.bluebeam.com/auth/oauth/token\nscopes:\n- scope: full\n  description: Full access to Bluebeam Studio API\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bluebeam-studio-openapi.yml\n- scope: jobs.create\n  description: Create and manage sessions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bluebeam-studio-openapi.yml\n- scope: jobs.read\n  description: Read session data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bluebeam-studio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluebeam/refs/heads/main/scopes/bluebeam-scopes.yml
summary_line: 3 scopes · authorizationCode
tags: []
token_urls:
- https://authserver.bluebeam.com/auth/oauth/token
---
