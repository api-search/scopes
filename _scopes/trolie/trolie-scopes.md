---
api_specs:
- filename: trolie-forecasting-api-openapi.yml
  format: yaml
  label: TROLIE Forecasting API
  slug: trolie-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-forecasting-api-openapi.yml
- filename: trolie-monitoring-sets-api-openapi.yml
  format: yaml
  label: TROLIE Monitoring Sets API
  slug: trolie-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-monitoring-sets-api-openapi.yml
- filename: trolie-seasonal-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal API
  slug: trolie-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-api-openapi.yml
- filename: trolie-seasonal-overrides-api-openapi.yml
  format: yaml
  label: TROLIE Seasonal Overrides API
  slug: trolie-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-seasonal-overrides-api-openapi.yml
- filename: trolie-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: TROLIE Temporary AAR Exceptions API
  slug: trolie-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-temporary-aar-exceptions-api-openapi.yml
- filename: trolie-realtime-api-openapi.yml
  format: yaml
  label: TROLIE Realtime API
  slug: trolie-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/openapi/trolie-realtime-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Trolie Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'TROLIE publishes 15 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the TROLIE API on a user''s behalf.


  Tokens are issued from https://no-server/oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TROLIE
provider_slug: trolie
schemes:
- description: Support RFC8725 JWT tokens.
  flows:
  - flow: clientCredentials
    tokenUrl: https://no-server/oauth2
  name: oauth2-primary-flow
  source: openapi/trolie-openapi.yml
scope_count: 15
scope_names:
- read:forecast-proposals
- read:monitoring-sets
- read:operating-snapshot
- read:realtime-proposals
- read:regional-operating-snapshot
- read:seasonal-overrides
- read:seasonal-proposals
- read:temporary-aar-exceptions
- write:forecast-proposals
- write:monitoring-sets
- write:realtime-proposals
- write:regional-operating-snapshot
- write:seasonal-overrides
- write:seasonal-proposals
- write:temporary-aar-exceptions
scopes:
- description: Read Forecast rating proposals
  flows:
  - clientCredentials
  scope: read:forecast-proposals
- description: Read monitoring sets
  flows:
  - clientCredentials
  scope: read:monitoring-sets
- description: Read the ratings and limits snapshots in-use by the transmission provider
  flows:
  - clientCredentials
  scope: read:operating-snapshot
- description: Read real-time rating proposals
  flows:
  - clientCredentials
  scope: read:realtime-proposals
- description: Read a Regional Operating Snapshot
  flows:
  - clientCredentials
  scope: read:regional-operating-snapshot
- description: Read seasonal overrides
  flows:
  - clientCredentials
  scope: read:seasonal-overrides
- description: Read seasonal rating proposals
  flows:
  - clientCredentials
  scope: read:seasonal-proposals
- description: Read temporary AAR exceptions
  flows:
  - clientCredentials
  scope: read:temporary-aar-exceptions
- description: Submit forecasted ratings
  flows:
  - clientCredentials
  scope: write:forecast-proposals
- description: Write monitoring sets
  flows:
  - clientCredentials
  scope: write:monitoring-sets
- description: Submit realtime ratings
  flows:
  - clientCredentials
  scope: write:realtime-proposals
- description: Write a Regional Operating Snapshot
  flows:
  - clientCredentials
  scope: write:regional-operating-snapshot
- description: Write seasonal overrides
  flows:
  - clientCredentials
  scope: write:seasonal-overrides
- description: Submit seasonal ratings
  flows:
  - clientCredentials
  scope: write:seasonal-proposals
- description: Write temporary AAR exceptions
  flows:
  - clientCredentials
  scope: write:temporary-aar-exceptions
slug: trolie-scopes
source_filename: trolie-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/trolie-openapi.yml\nschemes:\n- name: oauth2-primary-flow\n  source: openapi/trolie-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://no-server/oauth2\n  description: Support RFC8725 JWT tokens.\nscopes:\n- scope: read:forecast-proposals\n  description: Read Forecast rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:monitoring-sets\n  description: Read monitoring sets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:operating-snapshot\n  description: Read the ratings and limits snapshots in-use by the transmission provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:realtime-proposals\n  description: Read real-time rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:regional-operating-snapshot\n\
  \  description: Read a Regional Operating Snapshot\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:seasonal-overrides\n  description: Read seasonal overrides\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:seasonal-proposals\n  description: Read seasonal rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: read:temporary-aar-exceptions\n  description: Read temporary AAR exceptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:forecast-proposals\n  description: Submit forecasted ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:monitoring-sets\n  description: Write monitoring sets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:realtime-proposals\n  description: Submit realtime ratings\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:regional-operating-snapshot\n  description: Write a Regional Operating Snapshot\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:seasonal-overrides\n  description: Write seasonal overrides\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:seasonal-proposals\n  description: Submit seasonal ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n- scope: write:temporary-aar-exceptions\n  description: Write temporary AAR exceptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trolie/refs/heads/main/scopes/trolie-scopes.yml
summary_line: 15 scopes · clientCredentials
tags:
- Company
- Energy
- Electric Grid
- Transmission
- Open Standards
- OpenAPI
- LF Energy
- Open Source
token_bound: false
token_urls:
- https://no-server/oauth2
---
