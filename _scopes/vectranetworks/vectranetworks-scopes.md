---
api_specs:
- filename: vectranetworks-rux-v3.3-openapi.yml
  format: yaml
  label: Vectra AI Platform API (RUX)
  slug: vectra-ai-platform-api-rux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-rux-v3.3-openapi.yml
- filename: vectranetworks-detect-v2.3-openapi.yml
  format: yaml
  label: Vectra Detect API
  slug: vectra-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detect-v2.3-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Vectranetworks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vectra AI uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://{vectra_portal_url}/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vectra AI
provider_slug: vectranetworks
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://{vectra_portal_url}/oauth2/token
  name: oauth2
  source: openapi/vectranetworks-rux-v3.3-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: vectranetworks-scopes
source_filename: vectranetworks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vectranetworks-rux-v3.3-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/vectranetworks-rux-v3.3-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{vectra_portal_url}/oauth2/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/scopes/vectranetworks-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
token_urls:
- https://{vectra_portal_url}/oauth2/token
---
