---
api_specs:
- filename: arcnautical-com-account-api-openapi.yml
  format: yaml
  label: ArcNautical Account API
  slug: arcnautical-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-account-api-openapi.yml
- filename: arcnautical-com-cargo-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Cargo screening API
  slug: arcnautical-com-cargo-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-cargo-screening-api-openapi.yml
- filename: arcnautical-com-corridor-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Corridor monitors API
  slug: arcnautical-com-corridor-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-corridor-monitors-api-openapi.yml
- filename: arcnautical-com-crew-placement-api-openapi.yml
  format: yaml
  label: ArcNautical Crew placement API
  slug: arcnautical-com-crew-placement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-crew-placement-api-openapi.yml
- filename: arcnautical-com-exports-api-openapi.yml
  format: yaml
  label: ArcNautical Exports API
  slug: arcnautical-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-exports-api-openapi.yml
- filename: arcnautical-com-fleets-api-openapi.yml
  format: yaml
  label: ArcNautical Fleets API
  slug: arcnautical-com-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-fleets-api-openapi.yml
- filename: arcnautical-com-port-lookup-api-openapi.yml
  format: yaml
  label: ArcNautical Port lookup API
  slug: arcnautical-com-port-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-port-lookup-api-openapi.yml
- filename: arcnautical-com-public-vessel-check-api-openapi.yml
  format: yaml
  label: ArcNautical Public vessel check API
  slug: arcnautical-com-public-vessel-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-public-vessel-check-api-openapi.yml
- filename: arcnautical-com-vessel-monitors-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel monitors API
  slug: arcnautical-com-vessel-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-monitors-api-openapi.yml
- filename: arcnautical-com-vessel-screening-api-openapi.yml
  format: yaml
  label: ArcNautical Vessel screening API
  slug: arcnautical-com-vessel-screening-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-vessel-screening-api-openapi.yml
- filename: arcnautical-com-voyage-assessments-api-openapi.yml
  format: yaml
  label: ArcNautical Voyage assessments API
  slug: arcnautical-com-voyage-assessments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-voyage-assessments-api-openapi.yml
- filename: arcnautical-com-webhooks-api-openapi.yml
  format: yaml
  label: ArcNautical Webhooks API
  slug: arcnautical-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnautical-com/openapi/arcnautical-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Arcnautical Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ArcNautical publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ArcNautical API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ArcNautical
provider_slug: arcnautical-com
schemes: []
scope_count: 8
scope_names:
- vessel:screen
- vessel:monitor
- cargo:screen
- voyage:score
- voyage:monitor
- webhooks:manage
- usage:read
- logs:read
scopes:
- description: Hull screenings, screening batches and fleets, plus exports of screening records.
  flows: []
  scope: vessel:screen
- description: 'Vessel monitors: a standing re-screen per hull, with its history and change events.'
  flows: []
  scope: vessel:monitor
- description: Cargo screenings, plus exports of them.
  flows: []
  scope: cargo:screen
- description: Synchronous and batch assessments, plus retained-result retrieval.
  flows: []
  scope: voyage:score
- description: Live corridor monitors and monitor history.
  flows: []
  scope: voyage:monitor
- description: Webhook endpoint lifecycle, signed test delivery, the delivery log and redelivery.
  flows: []
  scope: webhooks:manage
- description: Entitlement limits and current consumption.
  flows: []
  scope: usage:read
- description: Your account's API access log for the key's environment, plus exports of it.
  flows: []
  scope: logs:read
slug: arcnautical-com-scopes
source_filename: arcnautical-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://arcnautical.com/developers/reference/#authentication\nscopes:\n  - name: vessel:screen\n    description: \"Hull screenings, screening batches and fleets, plus exports of screening records.\"\n  - name: vessel:monitor\n    description: \"Vessel monitors: a standing re-screen per hull, with its history and change events.\"\n  - name: cargo:screen\n    description: \"Cargo screenings, plus exports of them.\"\n  - name: voyage:score\n    description: \"Synchronous and batch assessments, plus retained-result retrieval.\"\n  - name: voyage:monitor\n    description: \"Live corridor monitors and monitor history.\"\n  - name: webhooks:manage\n    description: \"Webhook endpoint lifecycle, signed test delivery, the delivery log and redelivery.\"\n  - name: usage:read\n    description: \"Entitlement limits and current consumption.\"\n  - name: logs:read\n    description: \"Your account's API access log for the key's environment,\
  \ plus exports of it.\"\n"
source_yaml_url: https://artifacts.apis.io/arcnautical-com/scopes/arcnautical-com-scopes.yml
summary_line: 8 scopes
tags:
- Company
- Maritime
- Compliance
- Data
- Screening
token_bound: false
token_urls: []
---
