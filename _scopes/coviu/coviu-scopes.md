---
api_specs:
- filename: coviu-auth-api-openapi.yml
  format: yaml
  label: Coviu Auth API
  slug: coviu-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-auth-api-openapi.yml
- filename: coviu-collections-api-openapi.yml
  format: yaml
  label: Coviu Collections API
  slug: coviu-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-collections-api-openapi.yml
- filename: coviu-participants-api-openapi.yml
  format: yaml
  label: Coviu Participants API
  slug: coviu-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-participants-api-openapi.yml
- filename: coviu-sessions-api-openapi.yml
  format: yaml
  label: Coviu Sessions API
  slug: coviu-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-sessions-api-openapi.yml
- filename: coviu-waiting-area-api-openapi.yml
  format: yaml
  label: Coviu Waiting Area API
  slug: coviu-waiting-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-waiting-area-api-openapi.yml
- filename: coviu-webhook-requests-api-openapi.yml
  format: yaml
  label: Coviu Webhook Requests API
  slug: coviu-webhook-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/openapi/coviu-webhook-requests-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Coviu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coviu uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /v1/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coviu
provider_slug: coviu
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /v1/auth/token
  name: ClientCredentials
  source: openapi/coviu-rest-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: coviu-scopes
source_filename: coviu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: derived\nsource: openapi/coviu-rest-api-openapi.json\nschemes:\n- name: ClientCredentials\n  source: openapi/coviu-rest-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/auth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coviu/refs/heads/main/scopes/coviu-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare
- Telehealth
- Australia
- Virtual Care
- Video
- WebRTC
- Appointments
- Remote Monitoring
- REST
token_urls:
- /v1/auth/token
---
