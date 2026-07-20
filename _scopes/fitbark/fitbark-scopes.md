---
api_specs:
- filename: fitbark-openapi.yml
  format: yaml
  label: FitBark API v2
  slug: fitbark-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fitbark/refs/heads/main/openapi/fitbark-openapi.yml
authorization_urls:
- https://app.fitbark.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Fitbark Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FitBark publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the FitBark API on a user''s behalf.


  Tokens are issued from https://app.fitbark.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FitBark
provider_slug: fitbark
schemes:
- description: FitBark OAuth 2.0
  flows:
  - authorizationUrl: https://app.fitbark.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.fitbark.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://app.fitbark.com/oauth/token
  name: oauth2
  source: openapi/fitbark-openapi.yml
scope_count: 1
scope_names:
- fitbark_open_api
scopes:
- description: Access to the FitBark Public API for the approved application
  flows:
  - authorizationCode
  - clientCredentials
  scope: fitbark_open_api
slug: fitbark-scopes
source_filename: fitbark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/fitbark-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/fitbark-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.fitbark.com/oauth/authorize\n    tokenUrl: https://app.fitbark.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://app.fitbark.com/oauth/token\n  description: FitBark OAuth 2.0\nscopes:\n- scope: fitbark_open_api\n  description: Access to the FitBark Public API for the approved application\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/fitbark-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitbark/refs/heads/main/scopes/fitbark-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Company
- Dogs
- Pets
- Wearables
- Activity Tracking
- Health
- IoT
- Fitness
token_urls:
- https://app.fitbark.com/oauth/token
---
