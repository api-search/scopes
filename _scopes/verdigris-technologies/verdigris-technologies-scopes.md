---
api_specs:
- filename: verdigris-technologies-data-v4-openapi.json
  format: json
  label: Verdigris Data API
  slug: verdigris-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-data-v4-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Verdigris Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Verdigris Technologies uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.verdigris.co/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Verdigris Technologies
provider_slug: verdigris-technologies
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.verdigris.co/oauth/token
  name: oauth2
  source: openapi/verdigris-technologies-data-v4-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: verdigris-technologies-scopes
source_filename: verdigris-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/verdigris-technologies-data-v4-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/verdigris-technologies-data-v4-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.verdigris.co/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/scopes/verdigris-technologies-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Energy
- Energy Management
- Building Automation
- Smart Buildings
- IoT
- Sustainability
- Power Monitoring
- Time Series
- Analytics
- Electricity
token_urls:
- https://auth.verdigris.co/oauth/token
---
