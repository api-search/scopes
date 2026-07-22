---
authorization_urls:
- https://auth.gotenzo.com/o/authorize
description: ''
docs: https://support.gotenzo.com/developers/auth-flow/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Tenzo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tenzo publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tenzo API on a user''s behalf.


  Tokens are issued from https://auth.gotenzo.com/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tenzo
provider_slug: tenzo
schemes:
- flows:
  - authorizationUrl: https://auth.gotenzo.com/o/authorize
    flow: authorizationCode
    tokenUrl: https://auth.gotenzo.com/o/token/
  name: OAuth2
  source: https://support.gotenzo.com/developers/auth-flow/
scope_count: 4
scope_names:
- tenzo/sales:read
- tenzo/forecast:read
- tenzo/area:read
- tenzo/location:read
scopes:
- description: Read access to sales data.
  flows:
  - authorizationCode
  scope: tenzo/sales:read
- description: Read access to demand-forecast data.
  flows:
  - authorizationCode
  scope: tenzo/forecast:read
- description: Read access to area (grouping of locations) data.
  flows:
  - authorizationCode
  scope: tenzo/area:read
- description: Read access to location data.
  flows:
  - authorizationCode
  scope: tenzo/location:read
slug: tenzo-scopes
source_filename: tenzo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.gotenzo.com/developers/auth-flow/\ndocs: https://support.gotenzo.com/developers/auth-flow/\nnotes: >-\n  Scopes are granted per partner application by Tenzo at provisioning time and returned in the\n  token response `scope` field (space-delimited). The list below is the set documented in the\n  Authorization Code flow guide; a partner's granted scopes are a subset assigned by Tenzo. All\n  documented scopes are read-only.\nschemes:\n- name: OAuth2\n  source: https://support.gotenzo.com/developers/auth-flow/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.gotenzo.com/o/authorize\n    tokenUrl: https://auth.gotenzo.com/o/token/\nscopes:\n- scope: tenzo/sales:read\n  description: Read access to sales data.\n  flows: [authorizationCode]\n- scope: tenzo/forecast:read\n  description: Read access to demand-forecast data.\n  flows: [authorizationCode]\n- scope: tenzo/area:read\n  description:\
  \ Read access to area (grouping of locations) data.\n  flows: [authorizationCode]\n- scope: tenzo/location:read\n  description: Read access to location data.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenzo/refs/heads/main/scopes/tenzo-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Restaurant
- Analytics
- Business Intelligence
- Reporting
- Forecasting
- Hospitality
- Point of Sale
- Data Aggregation
- MCP
- Artificial Intelligence
token_urls:
- https://auth.gotenzo.com/o/token/
---
