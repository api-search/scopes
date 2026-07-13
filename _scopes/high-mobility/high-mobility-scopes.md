---
api_specs:
- filename: high-mobility-openapi.yml
  format: yaml
  label: High Mobility Vehicle API
  slug: high-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/openapi/high-mobility-openapi.yml
authorization_urls:
- https://owner-panel.high-mobility.com/oauth/new
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: High Mobility Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'High Mobility publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the High Mobility API on a user''s behalf.


  Tokens are issued from https://api.high-mobility.com/v1/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: High Mobility
provider_slug: high-mobility
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.high-mobility.com/v1/access_token
  - authorizationUrl: https://owner-panel.high-mobility.com/oauth/new
    flow: authorizationCode
    tokenUrl: https://api.high-mobility.com/v1/access_token
  name: oauth2
  source: openapi/high-mobility-openapi.yml
scope_count: 1
scope_names:
- vehicle:data
scopes:
- description: Read connected vehicle data
  flows:
  - authorizationCode
  - clientCredentials
  scope: vehicle:data
slug: high-mobility-scopes
source_filename: high-mobility-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/high-mobility-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/high-mobility-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.high-mobility.com/v1/access_token\n  - flow: authorizationCode\n    authorizationUrl: https://owner-panel.high-mobility.com/oauth/new\n    tokenUrl: https://api.high-mobility.com/v1/access_token\nscopes:\n- scope: vehicle:data\n  description: Read connected vehicle data\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/high-mobility-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/high-mobility/refs/heads/main/scopes/high-mobility-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Automotive
- Connected Cars
- IoT
- Vehicle Data
token_urls:
- https://api.high-mobility.com/v1/access_token
---
