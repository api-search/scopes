---
api_specs:
- filename: invendor-common-openapi-original.json
  format: json
  label: Invendor Common API
  slug: invendor-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-common-openapi-original.json
- filename: invendor-reporting-openapi-original.json
  format: json
  label: Invendor Reporting API
  slug: invendor-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/openapi/invendor-reporting-openapi-original.json
authorization_urls:
- https://identity.scanbro.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Invendor Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Invendor publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Invendor API on a user''s behalf.


  Tokens are issued from https://identity.scanbro.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Invendor
provider_slug: invendor
schemes:
- flows:
  - authorizationUrl: https://identity.scanbro.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.scanbro.com/connect/token
  name: OAuth2
  source: openapi/invendor-common-openapi-original.json
- flows:
  - authorizationUrl: https://identity.scanbro.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://identity.scanbro.com/connect/token
  name: OAuth2
  source: openapi/invendor-reporting-openapi-original.json
scope_count: 2
scope_names:
- io.common
- io.reporting
scopes:
- description: default scope
  flows:
  - authorizationCode
  scope: io.common
- description: default scope
  flows:
  - authorizationCode
  scope: io.reporting
slug: invendor-scopes
source_filename: invendor-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/invendor-common-openapi-original.json, openapi/invendor-reporting-openapi-original.json\nschemes:\n- name: OAuth2\n  source: openapi/invendor-common-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.scanbro.com/connect/authorize\n    tokenUrl: https://identity.scanbro.com/connect/token\n- name: OAuth2\n  source: openapi/invendor-reporting-openapi-original.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.scanbro.com/connect/authorize\n    tokenUrl: https://identity.scanbro.com/connect/token\nscopes:\n- scope: io.common\n  description: default scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/invendor-common-openapi-original.json\n- scope: io.reporting\n  description: default scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/invendor-reporting-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/invendor/refs/heads/main/scopes/invendor-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Inventory Management
- Vendor Managed Inventory
- Industrial Vending
- Supply Chain
- Warehouse Management
- Asset Tracking
token_urls:
- https://identity.scanbro.com/connect/token
---
