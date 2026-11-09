---
api_specs:
- filename: drivings-com-discovery-api-openapi.yml
  format: yaml
  label: Drivings Discovery API
  slug: drivings-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-discovery-api-openapi.yml
- filename: drivings-com-planning-api-openapi.yml
  format: yaml
  label: Drivings Planning API
  slug: drivings-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-planning-api-openapi.yml
authorization_urls:
- https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Drivings Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Drivings publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Drivings API on a user''s behalf.


  Tokens are issued from https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Drivings
provider_slug: drivings-com
schemes:
- description: Not required by any operation in this document. It gates one MCP tool, the learner's own progress, and is listed so an agent can see the whole permission surface in one place.
  flows:
  - authorizationUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/authorize
    flow: authorizationCode
    tokenUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token
  name: drivingsOAuth
  source: openapi/drivings-com-openapi.json
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Read the learner's email address.
  flows:
  - authorizationCode
  scope: email
- description: Identify the signed-in learner.
  flows:
  - authorizationCode
  scope: openid
- description: Read the learner's study target and recent activity.
  flows:
  - authorizationCode
  scope: profile
slug: drivings-com-scopes
source_filename: drivings-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/drivings-com-openapi.json\nschemes:\n- name: drivingsOAuth\n  source: openapi/drivings-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/authorize\n    tokenUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token\n  description: Not required by any operation in this document. It gates one MCP tool, the learner's\n    own progress, and is listed so an agent can see the whole permission surface in one place.\nscopes:\n- scope: email\n  description: Read the learner's email address.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drivings-com-openapi.json\n- scope: openid\n  description: Identify the signed-in learner.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/drivings-com-openapi.json\n- scope: profile\n  description: Read the learner's study target and recent activity.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/drivings-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drivings-com/scopes/drivings-com-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Driving
- Education
- United Kingdom
- US
token_bound: false
token_urls:
- https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token
---
