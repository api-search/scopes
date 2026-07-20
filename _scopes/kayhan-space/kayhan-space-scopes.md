---
api_specs:
- filename: kayhan-space-satcat-openapi-original.json
  format: json
  label: Satcat Service API
  slug: satcat-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/openapi/kayhan-space-satcat-openapi-original.json
authorization_urls: []
description: ''
docs: ''
flows:
- password
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Kayhan Space Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Kayhan Space publishes 1 OAuth 2.0 scope via the password and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Kayhan Space API on a user''s behalf.


  Tokens are issued from login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Kayhan Space
provider_slug: kayhan-space
schemes:
- flows:
  - flow: password
    tokenUrl: login
  - flow: clientCredentials
    tokenUrl: oauth/token
  name: Oauth2Scheme
  source: openapi/kayhan-space-satcat-openapi-original.json
scope_count: 1
scope_names:
- internal
scopes:
- description: Access from an internal API.
  flows:
  - clientCredentials
  - password
  scope: internal
slug: kayhan-space-scopes
source_filename: kayhan-space-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/kayhan-space-satcat-openapi-original.json\nschemes:\n- name: Oauth2Scheme\n  source: openapi/kayhan-space-satcat-openapi-original.json\n  flows:\n  - flow: password\n    tokenUrl: login\n  - flow: clientCredentials\n    tokenUrl: oauth/token\nscopes:\n- scope: internal\n  description: Access from an internal API.\n  flows:\n  - clientCredentials\n  - password\n  sources:\n  - openapi/kayhan-space-satcat-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayhan-space/refs/heads/main/scopes/kayhan-space-scopes.yml
summary_line: 1 scope · password/clientCredentials
tags:
- Company
- Frontier Tech
- Space
- Satellite
- Space Situational Awareness
- Collision Avoidance
- Space Traffic Management
- Aerospace
- Astrodynamics
token_urls:
- login
- oauth/token
---
