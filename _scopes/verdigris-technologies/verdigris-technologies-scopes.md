---
api_specs:
- filename: verdigris-technologies-control-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Control API
  slug: verdigris-technologies-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-control-api-openapi.yml
- filename: verdigris-technologies-current-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Current API
  slug: verdigris-technologies-current-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-current-api-openapi.yml
- filename: verdigris-technologies-energy-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Energy API
  slug: verdigris-technologies-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-energy-api-openapi.yml
- filename: verdigris-technologies-events-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Events API
  slug: verdigris-technologies-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-events-api-openapi.yml
- filename: verdigris-technologies-forecast-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Forecast API
  slug: verdigris-technologies-forecast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-forecast-api-openapi.yml
- filename: verdigris-technologies-power-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Power API
  slug: verdigris-technologies-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-power-api-openapi.yml
- filename: verdigris-technologies-power-factor-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Power Factor API
  slug: verdigris-technologies-power-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-power-factor-api-openapi.yml
- filename: verdigris-technologies-total-harmonic-distortion-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Total Harmonic Distortion API
  slug: verdigris-technologies-total-harmonic-distortion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-total-harmonic-distortion-api-openapi.yml
- filename: verdigris-technologies-voltage-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Voltage API
  slug: verdigris-technologies-voltage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-voltage-api-openapi.yml
- filename: verdigris-technologies-weather-api-openapi.yml
  format: yaml
  label: Verdigris Technologies Weather API
  slug: verdigris-technologies-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-weather-api-openapi.yml
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
