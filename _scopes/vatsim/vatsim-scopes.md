---
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Vatsim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'VATSIM publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the VATSIM API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: VATSIM
provider_slug: vatsim
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: connect
  source: openapi/connect.yaml
scope_count: 4
scope_names:
- country
- email
- full_name
- vatsim_details
scopes:
- description: Read the user's country of residence
  flows:
  - authorizationCode
  scope: country
- description: Read the user's email address
  flows:
  - authorizationCode
  scope: email
- description: Read the user's full name
  flows:
  - authorizationCode
  scope: full_name
- description: Read the user's VATSIM ratings and divisions
  flows:
  - authorizationCode
  scope: vatsim_details
slug: vatsim-scopes
source_filename: vatsim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/connect.yaml\nschemes:\n- name: connect\n  source: openapi/connect.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\nscopes:\n- scope: country\n  description: Read the user's country of residence\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: email\n  description: Read the user's email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: full_name\n  description: Read the user's full name\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n- scope: vatsim_details\n  description: Read the user's VATSIM ratings and divisions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/connect.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatsim/refs/heads/main/scopes/vatsim-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Aviation
- Flight Simulation
- Air Traffic Control
- Real-Time Data
- Community
token_urls:
- /oauth/token
---
