---
api_specs:
- filename: camara-openapi.yml
  format: yaml
  label: CAMARA Quality On Demand API
  slug: quality-on-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/openapi/camara-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Camara Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CAMARA publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CAMARA API on a user''s behalf.


  Tokens are issued from https://api.example.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CAMARA
provider_slug: camara
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.example.com/oauth2/token
  name: oAuth2ClientCredentials
  source: openapi/camara-openapi.yml
scope_count: 1
scope_names:
- qod
scopes:
- description: Quality On Demand session management
  flows:
  - clientCredentials
  scope: qod
slug: camara-scopes
source_filename: camara-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/camara-openapi.yml\nschemes:\n- name: oAuth2ClientCredentials\n  source: openapi/camara-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.example.com/oauth2/token\nscopes:\n- scope: qod\n  description: Quality On Demand session management\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/camara-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camara/refs/heads/main/scopes/camara-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Telecom
- Network APIs
- Standards
- Linux Foundation
- Open Gateway
- GSMA
- Connectivity
- 5G
token_urls:
- https://api.example.com/oauth2/token
---
