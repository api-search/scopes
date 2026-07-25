---
api_specs:
- filename: vectranetworks-accounts-api-openapi.yml
  format: yaml
  label: Vectra AI Accounts API
  slug: vectranetworks-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-accounts-api-openapi.yml
- filename: vectranetworks-assignment-outcomes-api-openapi.yml
  format: yaml
  label: Vectra AI Assignment Outcomes API
  slug: vectranetworks-assignment-outcomes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignment-outcomes-api-openapi.yml
- filename: vectranetworks-assignments-api-openapi.yml
  format: yaml
  label: Vectra AI Assignments API
  slug: vectranetworks-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-assignments-api-openapi.yml
- filename: vectranetworks-detections-api-openapi.yml
  format: yaml
  label: Vectra AI Detections API
  slug: vectranetworks-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detections-api-openapi.yml
- filename: vectranetworks-entities-api-openapi.yml
  format: yaml
  label: Vectra AI Entities API
  slug: vectranetworks-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-entities-api-openapi.yml
- filename: vectranetworks-events-api-openapi.yml
  format: yaml
  label: Vectra AI Events API
  slug: vectranetworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-events-api-openapi.yml
- filename: vectranetworks-groups-api-openapi.yml
  format: yaml
  label: Vectra AI Groups API
  slug: vectranetworks-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-groups-api-openapi.yml
- filename: vectranetworks-health-api-openapi.yml
  format: yaml
  label: Vectra AI Health API
  slug: vectranetworks-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-health-api-openapi.yml
- filename: vectranetworks-hosts-api-openapi.yml
  format: yaml
  label: Vectra AI Hosts API
  slug: vectranetworks-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-hosts-api-openapi.yml
- filename: vectranetworks-lockdown-api-openapi.yml
  format: yaml
  label: Vectra AI Lockdown API
  slug: vectranetworks-lockdown-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-lockdown-api-openapi.yml
- filename: vectranetworks-match-api-openapi.yml
  format: yaml
  label: Vectra AI Match API
  slug: vectranetworks-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-match-api-openapi.yml
- filename: vectranetworks-notes-api-openapi.yml
  format: yaml
  label: Vectra AI Notes API
  slug: vectranetworks-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-notes-api-openapi.yml
- filename: vectranetworks-proxies-api-openapi.yml
  format: yaml
  label: Vectra AI Proxies API
  slug: vectranetworks-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-proxies-api-openapi.yml
- filename: vectranetworks-search-api-openapi.yml
  format: yaml
  label: Vectra AI Search API
  slug: vectranetworks-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-search-api-openapi.yml
- filename: vectranetworks-tagging-api-openapi.yml
  format: yaml
  label: Vectra AI Tagging API
  slug: vectranetworks-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-tagging-api-openapi.yml
- filename: vectranetworks-threat-feeds-api-openapi.yml
  format: yaml
  label: Vectra AI Threat Feeds API
  slug: vectranetworks-threat-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-threat-feeds-api-openapi.yml
- filename: vectranetworks-users-api-openapi.yml
  format: yaml
  label: Vectra AI Users API
  slug: vectranetworks-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-users-api-openapi.yml
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
