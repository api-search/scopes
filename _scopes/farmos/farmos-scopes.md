---
api_specs:
- filename: farmos-farmos-api-openapi.yml
  format: yaml
  label: farmOS JSON:API
  slug: farmos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/openapi/farmos-farmos-api-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Farmos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'farmOS publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the farmOS API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: farmOS
provider_slug: farmos
schemes:
- description: 'OAuth2 Authorization Code grant for third-party integrations. Users

    authorize the client application to access their farmOS data.'
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: oauth2AuthorizationCode
  source: openapi/farmos-farmos-api-openapi.yml
- description: 'OAuth2 Client Credentials grant for machine-to-machine authentication.

    Used when no user account is required.'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: oauth2ClientCredentials
  source: openapi/farmos-farmos-api-openapi.yml
scope_count: 3
scope_names:
- farm_manager
- farm_viewer
- farm_worker
scopes:
- description: Full management access to the farm
  flows:
  - authorizationCode
  - clientCredentials
  scope: farm_manager
- description: Read-only access to farm records
  flows:
  - authorizationCode
  - clientCredentials
  scope: farm_viewer
- description: Worker-level access to farm records
  flows:
  - authorizationCode
  - clientCredentials
  scope: farm_worker
slug: farmos-scopes
source_filename: farmos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/farmos-farmos-api-openapi.yml\nschemes:\n- name: oauth2AuthorizationCode\n  source: openapi/farmos-farmos-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  description: |-\n    OAuth2 Authorization Code grant for third-party integrations. Users\n    authorize the client application to access their farmOS data.\n- name: oauth2ClientCredentials\n  source: openapi/farmos-farmos-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: |-\n    OAuth2 Client Credentials grant for machine-to-machine authentication.\n    Used when no user account is required.\nscopes:\n- scope: farm_manager\n  description: Full management access to the farm\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/farmos-farmos-api-openapi.yml\n- scope: farm_viewer\n  description: Read-only access to farm\
  \ records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/farmos-farmos-api-openapi.yml\n- scope: farm_worker\n  description: Worker-level access to farm records\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/farmos-farmos-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farmos/refs/heads/main/scopes/farmos-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Agriculture
- Farm Management
- Open Source
- JSON:API
- Record Keeping
- Self-Hosted
- Drupal
token_urls:
- /oauth/token
---
