---
api_specs:
- filename: auphonic-info-api-openapi.yml
  format: yaml
  label: Auphonic Info API
  slug: auphonic-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-info-api-openapi.yml
- filename: auphonic-presets-api-openapi.yml
  format: yaml
  label: Auphonic Presets API
  slug: auphonic-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-presets-api-openapi.yml
- filename: auphonic-productions-api-openapi.yml
  format: yaml
  label: Auphonic Productions API
  slug: auphonic-productions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-productions-api-openapi.yml
- filename: auphonic-services-api-openapi.yml
  format: yaml
  label: Auphonic Services API
  slug: auphonic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-services-api-openapi.yml
- filename: auphonic-simple-api-api-openapi.yml
  format: yaml
  label: Auphonic Simple API
  slug: auphonic-simple-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-simple-api-api-openapi.yml
- filename: auphonic-user-api-openapi.yml
  format: yaml
  label: Auphonic User API
  slug: auphonic-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/openapi/auphonic-user-api-openapi.yml
authorization_urls:
- https://auphonic.com/oauth2/authorize/
description: ''
docs: ''
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: derived
name: Auphonic Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Auphonic uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auphonic.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Auphonic
provider_slug: auphonic
schemes:
- description: OAuth 2.0 authentication for third-party applications.
  flows:
  - authorizationUrl: https://auphonic.com/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://auphonic.com/oauth2/token/
  - flow: password
    tokenUrl: https://auphonic.com/oauth2/token/
  name: oauth2
  source: openapi/auphonic-openapi.yaml
scope_count: 0
scope_names: []
scopes: []
slug: auphonic-scopes
source_filename: auphonic-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/auphonic-openapi.yaml\nschemes:\n- name: oauth2\n  source: openapi/auphonic-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auphonic.com/oauth2/authorize/\n    tokenUrl: https://auphonic.com/oauth2/token/\n  - flow: password\n    tokenUrl: https://auphonic.com/oauth2/token/\n  description: OAuth 2.0 authentication for third-party applications.\n\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auphonic/refs/heads/main/scopes/auphonic-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Audio
- Podcasting
- AI
- Automation
- Media
token_bound: false
token_urls:
- https://auphonic.com/oauth2/token/
---
