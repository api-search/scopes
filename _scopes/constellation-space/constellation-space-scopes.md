---
api_specs:
- filename: constellation-space-openapi.yml
  format: yaml
  label: ConstellationOS API
  slug: constellationos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/openapi/constellation-space-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.constellation.space/connect/api-tokens
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Constellation Space Scopes
name_suffix: OAuth Scopes
note: ConstellationOS uses scoped static bearer tokens (not an OAuth2 authorization flow). Scopes are selected when a token is created in the console and gate the API operations below.
overview: 'Constellation Space publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Constellation Space API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Constellation Space
provider_slug: constellation-space
schemes:
- name: bearerAuth
  source: openapi/constellation-space-openapi.yml
  type: token-scopes
scope_count: 3
scope_names:
- topology:read
- telemetry:write
- predictions:run
scopes:
- description: Read the fleet topology graph. Enables GET /api/v1/topology/.
  flows: []
  scope: topology:read
- description: Ingest telemetry metrics. Enables POST /api/v1/telemetry/ingest.
  flows: []
  scope: telemetry:write
- description: Run ML predictions. Enables POST /api/v1/predictions/.
  flows: []
  scope: predictions:run
slug: constellation-space-scopes
source_filename: constellation-space-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.constellation.space/connect/api-tokens\ndocs: https://docs.constellation.space/connect/api-tokens\nnote: >-\n  ConstellationOS uses scoped static bearer tokens (not an OAuth2 authorization\n  flow). Scopes are selected when a token is created in the console and gate the\n  API operations below.\nschemes:\n- name: bearerAuth\n  type: token-scopes\n  source: openapi/constellation-space-openapi.yml\nscopes:\n- scope: topology:read\n  description: Read the fleet topology graph. Enables GET /api/v1/topology/.\n  operations:\n  - getTopology\n  sources:\n  - openapi/constellation-space-openapi.yml\n- scope: telemetry:write\n  description: Ingest telemetry metrics. Enables POST /api/v1/telemetry/ingest.\n  operations:\n  - ingestTelemetry\n  sources:\n  - openapi/constellation-space-openapi.yml\n- scope: predictions:run\n  description: Run ML predictions. Enables POST /api/v1/predictions/.\n  operations:\n  - runPredictions\n\
  \  sources:\n  - openapi/constellation-space-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constellation-space/refs/heads/main/scopes/constellation-space-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Satellites
- Space
- Telemetry
- Machine Learning
- Fleet Operations
- Ground Segment
- Predictions
token_urls: []
---
