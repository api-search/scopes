---
api_specs:
- filename: lufthansa-openapi.yml
  format: yaml
  label: Lufthansa Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/openapi/lufthansa-openapi.yml
authorization_urls:
- https://api.lufthansa.com/v1/oauth/token
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Lufthansa Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lufthansa publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lufthansa API on a user''s behalf.


  Tokens are issued from https://api.lufthansa.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lufthansa
provider_slug: lufthansa
schemes:
- flows:
  - authorizationUrl: https://api.lufthansa.com/v1/oauth/token
    flow: authorizationCode
    tokenUrl: https://api.lufthansa.com/v1/oauth/token
  name: auth
  source: openapi/lufthansa-openapi.yml
scope_count: 1
scope_names:
- read:LH Open API
scopes:
- description: read access
  flows:
  - authorizationCode
  scope: read:LH Open API
slug: lufthansa-scopes
source_filename: lufthansa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lufthansa-openapi.yml\nschemes:\n- name: auth\n  source: openapi/lufthansa-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.lufthansa.com/v1/oauth/token\n    tokenUrl: https://api.lufthansa.com/v1/oauth/token\nscopes:\n- scope: read:LH Open API\n  description: read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/lufthansa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/scopes/lufthansa-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Airlines
- Travel
- Aviation
- Flights
token_urls:
- https://api.lufthansa.com/v1/oauth/token
---
