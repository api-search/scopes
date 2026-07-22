---
api_specs:
- filename: the-climate-corporation-platform-openapi-original.yml
  format: yaml
  label: Climate FieldView Platform API
  slug: climate-fieldview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/openapi/the-climate-corporation-platform-openapi-original.yml
authorization_urls:
- https://climate.com/static/app-login/
description: ''
docs: https://dev.fieldview.com/api-details/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: The Climate Corporation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'The Climate Corporation publishes 24 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Climate Corporation API on a user''s behalf.


  Tokens are issued from https://api.climate.com/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Climate Corporation
provider_slug: the-climate-corporation
schemes:
- description: 'Log in with FieldView OAuth2 provider (Authorization Code Grant). Used to authorize the client (partner) and

    user. The *access_token* is required to be provided in the `Authorization` header on all calls to the FieldView

    APIs with the following format `Bearer $access_token`.'
  flows:
  - authorizationUrl: https://climate.com/static/app-login/
    flow: authorizationCode
    tokenUrl: https://api.climate.com/api/oauth/token
  name: oauth2_authorization_code
  source: openapi/the-climate-corporation-platform-openapi-original.yml
scope_count: 24
scope_names:
- asApplied:read
- asApplied:write
- asHarvested:read
- asHarvested:write
- asPlanted:read
- asPlanted:write
- avroAgronomicData:read
- boundaries:write
- customerInsights:read
- diagnostics:read
- exports:read
- farmOrganizations:read
- fields:read
- fields:write
- imagery:write
- operations:read
- plantingActivitySummary:read
- platform
- resourceOwners:read
- rx:write
- scouting:read
- soil:write
- standCount:write
- weedCount:write
scopes:
- description: Required for retrieving as applied data
  flows:
  - authorizationCode
  scope: asApplied:read
- description: Required for uploading application data
  flows:
  - authorizationCode
  scope: asApplied:write
- description: Required for retrieving harvest data
  flows:
  - authorizationCode
  scope: asHarvested:read
- description: Required for uploading harvest data
  flows:
  - authorizationCode
  scope: asHarvested:write
- description: Required for retrieving planting data
  flows:
  - authorizationCode
  scope: asPlanted:read
- description: Required for uploading planting data
  flows:
  - authorizationCode
  scope: asPlanted:write
- description: Required for retrieving agronomic data
  flows:
  - authorizationCode
  scope: avroAgronomicData:read
- description: ''
  flows: []
  scope: boundaries:write
- description: Required for retrieving customer insights metrics data
  flows:
  - authorizationCode
  scope: customerInsights:read
- description: Required for retrieving CNH machine diagnostic data
  flows:
  - authorizationCode
  scope: diagnostics:read
- description: Required for requesting or retrieving exports
  flows:
  - authorizationCode
  scope: exports:read
- description: Required for retrieving farm organization information
  flows:
  - authorizationCode
  scope: farmOrganizations:read
- description: Required for retrieving field and boundary information
  flows:
  - authorizationCode
  scope: fields:read
- description: Required for uploading field boundaries
  flows:
  - authorizationCode
  scope: fields:write
- description: Required for uploading imagery
  flows:
  - authorizationCode
  scope: imagery:write
- description: Required for retrieving operation information
  flows:
  - authorizationCode
  scope: operations:read
- description: Required for retrieving planting activity summary data
  flows:
  - authorizationCode
  scope: plantingActivitySummary:read
- description: (DEPRECATED) Legacy scope used for some Platform APIs
  flows:
  - authorizationCode
  scope: platform
- description: Required for retrieving resource owner information
  flows:
  - authorizationCode
  scope: resourceOwners:read
- description: Required for uploading prescriptions
  flows:
  - authorizationCode
  scope: rx:write
- description: Required for retrieving user\'s scouting information
  flows:
  - authorizationCode
  scope: scouting:read
- description: Required for uploading soil sample results
  flows:
  - authorizationCode
  scope: soil:write
- description: ''
  flows: []
  scope: standCount:write
- description: ''
  flows: []
  scope: weedCount:write
slug: the-climate-corporation-scopes
source_filename: the-climate-corporation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/the-climate-corporation-platform-openapi-original.yml (v4.0.11)\ndocs: https://dev.fieldview.com/api-details/\nnotes: >-\n  Scopes are resource:action pairs (e.g. fields:read imagery:write), passed\n  space-delimited and URL-encoded on the authorization request. The user is\n  prompted to grant each requested scope. The legacy \"platform\" scope is\n  deprecated in favor of resource-specific scopes.\nschemes:\n- name: oauth2_authorization_code\n  source: openapi/the-climate-corporation-platform-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://climate.com/static/app-login/\n    tokenUrl: https://api.climate.com/api/oauth/token\n  description: |-\n    Log in with FieldView OAuth2 provider (Authorization Code Grant). Used to authorize the client (partner) and\n    user. The *access_token* is required to be provided in the `Authorization` header on all calls to the FieldView\n \
  \   APIs with the following format `Bearer $access_token`.\nscopes:\n- scope: asApplied:read\n  description: Required for retrieving as applied data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: asApplied:write\n  description: Required for uploading application data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: asHarvested:read\n  description: Required for retrieving harvest data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: asHarvested:write\n  description: Required for uploading harvest data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: asPlanted:read\n  description: Required for retrieving planting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n\
  - scope: asPlanted:write\n  description: Required for uploading planting data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: avroAgronomicData:read\n  description: Required for retrieving agronomic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: boundaries:write\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: customerInsights:read\n  description: Required for retrieving customer insights metrics data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: diagnostics:read\n  description: Required for retrieving CNH machine diagnostic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: exports:read\n  description: Required for requesting or retrieving exports\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: farmOrganizations:read\n  description: Required for retrieving farm organization information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: fields:read\n  description: Required for retrieving field and boundary information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: fields:write\n  description: Required for uploading field boundaries\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: imagery:write\n  description: Required for uploading imagery\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: operations:read\n  description: Required for retrieving operation information\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: plantingActivitySummary:read\n  description: Required for retrieving planting activity summary data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: platform\n  description: (DEPRECATED) Legacy scope used for some Platform APIs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: resourceOwners:read\n  description: Required for retrieving resource owner information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: rx:write\n  description: Required for uploading prescriptions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: scouting:read\n  description: Required for retrieving user\\'s scouting\
  \ information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: soil:write\n  description: Required for uploading soil sample results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: standCount:write\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n- scope: weedCount:write\n  sources:\n  - openapi/the-climate-corporation-platform-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-climate-corporation/refs/heads/main/scopes/the-climate-corporation-scopes.yml
summary_line: 24 scopes · authorizationCode
tags:
- Company
- Climate
- Agriculture
- AgTech
- Digital Agriculture
- Farm Management
- Geospatial
- APIs
token_urls:
- https://api.climate.com/api/oauth/token
---
