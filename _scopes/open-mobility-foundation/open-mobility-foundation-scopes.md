---
api_specs:
- filename: open-mobility-foundation-events-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Events API
  slug: open-mobility-foundation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-events-api-openapi.yml
- filename: open-mobility-foundation-geographies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies API
  slug: open-mobility-foundation-geographies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-api-openapi.yml
- filename: open-mobility-foundation-geographies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Geographies.json API
  slug: open-mobility-foundation-geographies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-geographies-json-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions API
  slug: open-mobility-foundation-jurisdictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-api-openapi.yml
- filename: open-mobility-foundation-jurisdictions-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Jurisdictions.json API
  slug: open-mobility-foundation-jurisdictions-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-jurisdictions-json-api-openapi.yml
- filename: open-mobility-foundation-metrics-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Metrics API
  slug: open-mobility-foundation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-metrics-api-openapi.yml
- filename: open-mobility-foundation-policies-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies API
  slug: open-mobility-foundation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-api-openapi.yml
- filename: open-mobility-foundation-policies-json-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Policies.json API
  slug: open-mobility-foundation-policies-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-policies-json-api-openapi.yml
- filename: open-mobility-foundation-reports-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Reports API
  slug: open-mobility-foundation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-reports-api-openapi.yml
- filename: open-mobility-foundation-requirements-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Requirements API
  slug: open-mobility-foundation-requirements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-requirements-api-openapi.yml
- filename: open-mobility-foundation-stops-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Stops API
  slug: open-mobility-foundation-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-stops-api-openapi.yml
- filename: open-mobility-foundation-telemetry-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Telemetry API
  slug: open-mobility-foundation-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-telemetry-api-openapi.yml
- filename: open-mobility-foundation-trips-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Trips API
  slug: open-mobility-foundation-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-trips-api-openapi.yml
- filename: open-mobility-foundation-value-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Value API
  slug: open-mobility-foundation-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-value-api-openapi.yml
- filename: open-mobility-foundation-vehicles-api-openapi.yml
  format: yaml
  label: Open Mobility Foundation Vehicles API
  slug: open-mobility-foundation-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/openapi/open-mobility-foundation-vehicles-api-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/openmobilityfoundation/mobility-data-specification/blob/main/general-information.md#oauth-20
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Open Mobility Foundation Scopes
name_suffix: OAuth Scopes
note: The specs declare http bearer (not oauth2) securitySchemes. Only the Metrics API names scopes; General Information says OAuth 2.0 client_credentials is RECOMMENDED and producers MAY choose to specify token scopes, so other scopes are implementation-defined.
overview: 'Open Mobility Foundation publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Open Mobility Foundation API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Open Mobility Foundation
provider_slug: open-mobility-foundation
schemes: []
scope_count: 2
scope_names:
- metrics:read
- metrics:read:provider
scopes:
- description: Scope claim expected in the JWT for MDS Metrics endpoints (one of two accepted scopes).
  flows: []
  scope: metrics:read
- description: Alternative scope claim accepted by MDS Metrics endpoints.
  flows: []
  scope: metrics:read:provider
slug: open-mobility-foundation-scopes
source_filename: open-mobility-foundation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: openapi/open-mobility-foundation-mds-metrics-openapi.yml\ndocs: https://github.com/openmobilityfoundation/mobility-data-specification/blob/main/general-information.md#oauth-20\nnote: The specs declare http bearer (not oauth2) securitySchemes. Only the Metrics API names scopes; General Information\n  says OAuth 2.0 client_credentials is RECOMMENDED and producers MAY choose to specify token scopes, so other scopes\n  are implementation-defined.\nscopes:\n- name: metrics:read\n  description: Scope claim expected in the JWT for MDS Metrics endpoints (one of two accepted scopes).\n  api: mds-metrics\n- name: metrics:read:provider\n  description: Alternative scope claim accepted by MDS Metrics endpoints.\n  api: mds-metrics\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-mobility-foundation/refs/heads/main/scopes/open-mobility-foundation-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Mobility
- Open Source
- Open Standards
- Transportation
- Cities
- Micromobility
- Data Specifications
token_bound: false
token_urls: []
---
