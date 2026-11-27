---
api_specs:
- filename: register-gy-openapi.json
  format: json
  label: Register.gy API
  slug: registergy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/register-gy/openapi/register-gy-openapi.json
authorization_urls:
- https://register.gy/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Register.gy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Register.gy publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Register.gy API on a user''s behalf.


  Tokens are issued from https://register.gy/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Register.gy
provider_slug: register-gy
schemes:
- flows:
  - authorizationUrl: https://register.gy/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://register.gy/oauth/token
  name: oauth2
  source: openapi/register-gy-openapi.json
scope_count: 2
scope_names:
- domains:read
- websites:write
scopes:
- description: See your .gy domains and their DNS records
  flows:
  - authorizationCode
  scope: domains:read
- description: Connect your websites (change website records only, with 7-day undo)
  flows:
  - authorizationCode
  scope: websites:write
slug: register-gy-scopes
source_filename: register-gy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: derived\nsource: openapi/register-gy-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/register-gy-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://register.gy/oauth/authorize\n    tokenUrl: https://register.gy/oauth/token\nscopes:\n- scope: domains:read\n  description: See your .gy domains and their DNS records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/register-gy-openapi.json\n- scope: websites:write\n  description: Connect your websites (change website records only, with 7-day undo)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/register-gy-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/register-gy/scopes/register-gy-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Domain Registration
- DNS
- Customer Support
token_bound: false
token_urls:
- https://register.gy/oauth/token
---
