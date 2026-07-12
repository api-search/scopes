---
authorization_urls:
- https://api.climate.com/api/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Climate Fieldview Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Climate FieldView publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Climate FieldView API on a user''s behalf.


  Tokens are issued from https://api.climate.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Climate FieldView
provider_slug: climate-fieldview
schemes:
- description: OAuth 2.0 authorization for Climate FieldView API
  flows:
  - authorizationUrl: https://api.climate.com/api/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.climate.com/api/oauth/token
  name: oauth2
  source: openapi/climate-fieldview-platform-openapi.yml
scope_count: 5
scope_names:
- fields:read
- imagery:read
- layers:read
- layers:write
- soilsampling:read
scopes:
- description: Read field boundaries and metadata
  flows:
  - authorizationCode
  scope: fields:read
- description: Read satellite imagery layers
  flows:
  - authorizationCode
  scope: imagery:read
- description: Read activity layer data
  flows:
  - authorizationCode
  scope: layers:read
- description: Upload activity layer data
  flows:
  - authorizationCode
  scope: layers:write
- description: Read soil sampling results
  flows:
  - authorizationCode
  scope: soilsampling:read
slug: climate-fieldview-scopes
source_filename: climate-fieldview-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/climate-fieldview-platform-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/climate-fieldview-platform-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.climate.com/api/oauth/authorize\n    tokenUrl: https://api.climate.com/api/oauth/token\n  description: OAuth 2.0 authorization for Climate FieldView API\nscopes:\n- scope: fields:read\n  description: Read field boundaries and metadata\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n- scope: imagery:read\n  description: Read satellite imagery layers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n- scope: layers:read\n  description: Read activity layer data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n- scope: layers:write\n  description: Upload activity layer data\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n- scope: soilsampling:read\n  description: Read soil sampling results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/climate-fieldview-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-fieldview/refs/heads/main/scopes/climate-fieldview-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Agriculture
- Bayer
- Crop Data
- Field Boundaries
- Harvest
- OAuth2
- Planting
- Precision Ag
token_urls:
- https://api.climate.com/api/oauth/token
---
