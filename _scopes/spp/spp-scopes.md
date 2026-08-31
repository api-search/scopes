---
api_specs:
- filename: spp-forecasting-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Forecasting API
  slug: spp-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-forecasting-api-openapi.yml
- filename: spp-monitoring-sets-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Monitoring Sets API
  slug: spp-monitoring-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-monitoring-sets-api-openapi.yml
- filename: spp-real-time-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Real Time API
  slug: spp-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-real-time-api-openapi.yml
- filename: spp-seasonal-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Seasonal API
  slug: spp-seasonal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-seasonal-api-openapi.yml
- filename: spp-seasonal-overrides-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Seasonal Overrides API
  slug: spp-seasonal-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-seasonal-overrides-api-openapi.yml
- filename: spp-temporary-aar-exceptions-api-openapi.yml
  format: yaml
  label: Southwest Power Pool Temporary AAR Exceptions API
  slug: spp-temporary-aar-exceptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/spp-temporary-aar-exceptions-api-openapi.yml
authorization_urls: []
description: ''
docs: https://trolie.energy/spec
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Spp Scopes
name_suffix: OAuth Scopes
note: These scopes are declared by the LF Energy TROLIE community specification — the contract SPP's own "SPP LEP/TROLIE API Data Exchange Guide" (v1.0, 2024-11-08) directs implementers to — not by an SPP-published authorization server. SPP publishes no OAuth authorization server, no token URL and no scope reference of its own; its LEP ratings API authenticates with an OATI webCARES x.509 certificate plus an SPP UAA role (see authentication/spp-authentication.yml). Treat this as the scope vocabulary an SPP LEP integration is built against, not as an observed SPP OAuth surface.
overview: 'Southwest Power Pool publishes 15 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Southwest Power Pool API on a user''s behalf.


  Tokens are issued from relative /oauth2 against the spec placeholder server (no SPP host published).


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Southwest Power Pool
provider_slug: spp
schemes:
- description: Support RFC8725 JWT tokens.
  flows:
  - flow: clientCredentials
    tokenUrl: relative /oauth2 against the spec placeholder server (no SPP host published)
  name: oauth2-primary-flow
  source: openapi/trolie-standard-openapi.yml
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
slug: spp-scopes
source_filename: spp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/trolie-standard-openapi.yml\ndocs: https://trolie.energy/spec\nstandard: LF Energy TROLIE 1.1.0\nnote: >-\n  These scopes are declared by the LF Energy TROLIE community specification —\n  the contract SPP's own \"SPP LEP/TROLIE API Data Exchange Guide\" (v1.0,\n  2024-11-08) directs implementers to — not by an SPP-published authorization\n  server. SPP publishes no OAuth authorization server, no token URL and no scope\n  reference of its own; its LEP ratings API authenticates with an OATI webCARES\n  x.509 certificate plus an SPP UAA role (see\n  authentication/spp-authentication.yml). Treat this as the scope vocabulary an\n  SPP LEP integration is built against, not as an observed SPP OAuth surface.\nschemes:\n- name: oauth2-primary-flow\n  source: openapi/trolie-standard-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: relative /oauth2 against the spec placeholder server (no SPP host published)\n \
  \ description: Support RFC8725 JWT tokens.\nscopes:\n- scope: read:forecast-proposals\n  description: Read Forecast rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:monitoring-sets\n  description: Read monitoring sets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:operating-snapshot\n  description: Read the ratings and limits snapshots in-use by the transmission provider\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:realtime-proposals\n  description: Read real-time rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:regional-operating-snapshot\n  description: Read a Regional Operating Snapshot\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:seasonal-overrides\n  description: Read seasonal overrides\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:seasonal-proposals\n  description: Read seasonal rating proposals\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: read:temporary-aar-exceptions\n  description: Read temporary AAR exceptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:forecast-proposals\n  description: Submit forecasted ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:monitoring-sets\n  description: Write monitoring sets\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:realtime-proposals\n  description: Submit realtime ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:regional-operating-snapshot\n  description: Write a Regional Operating Snapshot\n\
  \  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:seasonal-overrides\n  description: Write seasonal overrides\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:seasonal-proposals\n  description: Submit seasonal ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n- scope: write:temporary-aar-exceptions\n  description: Write temporary AAR exceptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/trolie-standard-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/scopes/spp-scopes.yml
summary_line: 15 scopes · clientCredentials
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- Utilities
- Renewables
- Market Data
- Transmission
- System Operator
token_urls:
- relative /oauth2 against the spec placeholder server (no SPP host published)
---
