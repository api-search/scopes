---
api_specs:
- filename: bitfinder-awair-openapi.yml
  format: yaml
  label: Awair Home & OAuth Developer API
  slug: awair-home-oauth-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitfinder/refs/heads/main/openapi/bitfinder-awair-openapi.yml
authorization_urls:
- https://oauth2.awair.is/v2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bitfinder Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Bitfinder uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://oauth2.awair.is/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bitfinder
provider_slug: bitfinder
schemes:
- description: OAuth 2.0 authorization-code flow for third-party access to Awair user data.
  flows:
  - authorizationUrl: https://oauth2.awair.is/v2/authorize
    flow: authorizationCode
    tokenUrl: https://oauth2.awair.is/v2/token
  name: oauth2
  source: openapi/bitfinder-awair-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: bitfinder-scopes
source_filename: bitfinder-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/bitfinder-awair-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/bitfinder-awair-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.awair.is/v2/authorize\n    tokenUrl: https://oauth2.awair.is/v2/token\n  description: OAuth 2.0 authorization-code flow for third-party access to Awair user data.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfinder/refs/heads/main/scopes/bitfinder-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Air Quality
- Internet of Things
- IoT
- Environmental Monitoring
- Smart Home
- Sensors
- Health
- Developer API
token_urls:
- https://oauth2.awair.is/v2/token
---
