---
api_specs:
- filename: chaoss-collectoss-openapi.yml
  format: yaml
  label: CollectOSS REST API
  slug: collectoss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/openapi/chaoss-collectoss-openapi.yml
authorization_urls: []
description: CollectOSS runs OAuth 2.0 authorization code but publishes NO scope vocabulary. This is a recorded absence, not an unfinished probe.
docs: https://docs.collectoss.org/en/latest/login.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Chaoss Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CHAOSS uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CHAOSS
provider_slug: chaoss
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: chaoss-scopes
source_filename: chaoss-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: CHAOSS\nproviderId: chaoss\napi: CollectOSS REST API\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.collectoss.org/en/latest/login.html and the published contract\n  openapi/chaoss-collectoss-openapi.yml, both read 2026-09-05.\ndocs: https://docs.collectoss.org/en/latest/login.html\ndescription: >-\n  CollectOSS runs OAuth 2.0 authorization code but publishes NO scope vocabulary. This is a recorded\n  absence, not an unfinished probe.\nscope_count: 0\nscopes: []\nfindings:\n  - >-\n    The OpenAPI declares no components.securitySchemes, so there is no `scopes` map to derive from.\n    derive-oauth-scopes.py returned \"with oauth2: 0\" against this repo for exactly that reason.\n  - >-\n    The authorization page is documented as showing the user \"what information will be shared\", but\n    no scope names, no permission reference page, and no per-operation\
  \ scope requirements are\n    published anywhere in the CollectOSS documentation.\n  - >-\n    Consequence for an integrator: authorization is all-or-nothing per Client Application. An agent\n    cannot request least privilege because there is no privilege vocabulary to request from.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoss/refs/heads/main/scopes/chaoss-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Community Health
- DEI
- Linux Foundation
- Metrics
- Observability
- Open-Source
- Risk
- Sustainability
token_urls: []
---
