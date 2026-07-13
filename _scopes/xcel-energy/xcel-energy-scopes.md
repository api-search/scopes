---
api_specs:
- filename: xcel-energy-green-button-api.yaml
  format: yaml
  label: Xcel Energy Green Button Connect My Data API
  slug: xcel-energy-green-button-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-green-button-api.yaml
- filename: xcel-energy-smart-meter-api.yaml
  format: yaml
  label: Xcel Energy Smart Meter IEEE 2030.5 API
  slug: xcel-energy-smart-meter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-smart-meter-api.yaml
authorization_urls:
- https://api.xcelenergy.com/DataCustodian/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Xcel Energy Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Xcel Energy publishes 2 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Xcel Energy API on a user''s behalf.


  Tokens are issued from https://api.xcelenergy.com/DataCustodian/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Xcel Energy
provider_slug: xcel-energy
schemes:
- description: Customer-scoped access token issued via the OAuth 2.0 authorization-code grant.
  flows:
  - authorizationUrl: https://api.xcelenergy.com/DataCustodian/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token
  name: accessToken
  source: openapi/xcel-energy-green-button-api.yaml
- description: Application-scoped client access token used for management endpoints (Authorization list, Bulk, ServiceStatus).
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token
  name: clientAccessToken
  source: openapi/xcel-energy-green-button-api.yaml
scope_count: 2
scope_names:
- DataCustodian_Admin_Access
- FB=4_5_15;IntervalDuration=900;BlockDuration=monthly;HistoryLength=34128000
scopes:
- description: Administrative scope used for application-level operations.
  flows:
  - clientCredentials
  scope: DataCustodian_Admin_Access
- description: Standard ESPI scope string for 15-minute electric usage data with 13 months of history.
  flows:
  - authorizationCode
  scope: FB=4_5_15;IntervalDuration=900;BlockDuration=monthly;HistoryLength=34128000
slug: xcel-energy-scopes
source_filename: xcel-energy-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xcel-energy-green-button-api.yaml\nschemes:\n- name: accessToken\n  source: openapi/xcel-energy-green-button-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.xcelenergy.com/DataCustodian/oauth/authorize\n    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token\n  description: Customer-scoped access token issued via the OAuth 2.0 authorization-code grant.\n- name: clientAccessToken\n  source: openapi/xcel-energy-green-button-api.yaml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token\n  description: Application-scoped client access token used for management endpoints (Authorization\n    list, Bulk, ServiceStatus).\nscopes:\n- scope: DataCustodian_Admin_Access\n  description: Administrative scope used for application-level operations.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/xcel-energy-green-button-api.yaml\n\
  - scope: FB=4_5_15;IntervalDuration=900;BlockDuration=monthly;HistoryLength=34128000\n  description: Standard ESPI scope string for 15-minute electric usage data with 13 months of\n    history.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/xcel-energy-green-button-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/scopes/xcel-energy-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials
tags:
- Electric Utility
- Energy
- Energy Data
- Green Button
- Natural Gas
- Smart Grid
- Smart Meter
- Utility
- ESPI
- IEEE 2030.5
- Fortune 500
token_urls:
- https://api.xcelenergy.com/DataCustodian/oauth/token
---
