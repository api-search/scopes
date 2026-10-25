---
api_specs:
- filename: blacksky-budgets-api-openapi.yml
  format: yaml
  label: BlackSky Budgets API
  slug: blacksky-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-budgets-api-openapi.yml
- filename: blacksky-catalog-api-openapi.yml
  format: yaml
  label: BlackSky Catalog API
  slug: blacksky-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-catalog-api-openapi.yml
- filename: blacksky-data-management-api-openapi.yml
  format: yaml
  label: BlackSky Data management API
  slug: blacksky-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-data-management-api-openapi.yml
- filename: blacksky-eulas-api-openapi.yml
  format: yaml
  label: BlackSky EULAs API
  slug: blacksky-eulas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-eulas-api-openapi.yml
- filename: blacksky-geometries-api-openapi.yml
  format: yaml
  label: BlackSky Geometries API
  slug: blacksky-geometries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-geometries-api-openapi.yml
- filename: blacksky-glossary-api-openapi.yml
  format: yaml
  label: BlackSky Glossary API
  slug: blacksky-glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-glossary-api-openapi.yml
- filename: blacksky-orders-api-openapi.yml
  format: yaml
  label: BlackSky Orders API
  slug: blacksky-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-orders-api-openapi.yml
- filename: blacksky-processing-api-openapi.yml
  format: yaml
  label: BlackSky Processing API
  slug: blacksky-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-processing-api-openapi.yml
- filename: blacksky-tasking-api-openapi.yml
  format: yaml
  label: BlackSky Tasking API
  slug: blacksky-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/openapi/blacksky-tasking-api-openapi.yml
authorization_urls:
- https://auth.up42.com/realms/public/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Blacksky Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BlackSky publishes 3 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the BlackSky API on a user''s behalf.


  Tokens are issued from https://auth.up42.com/realms/public/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BlackSky
provider_slug: blacksky
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token
  - authorizationUrl: https://auth.up42.com/realms/public/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token
  name: oauth2Profiles
  source: openapi/blacksky-up42-api-openapi.yml
scope_count: 3
scope_names:
- account
- budget.r
- eula.w
scopes:
- description: Access to resources of the authenticated user's account
  flows:
  - authorizationCode
  - clientCredentials
  scope: account
- description: ''
  flows: []
  scope: budget.r
- description: Create/Update/Delete a EULA document
  flows:
  - authorizationCode
  - clientCredentials
  scope: eula.w
slug: blacksky-scopes
source_filename: blacksky-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: derived\nsource: openapi/blacksky-up42-api-openapi.yml\nschemes:\n- name: oauth2Profiles\n  source: openapi/blacksky-up42-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token\n  - flow: authorizationCode\n    authorizationUrl: https://auth.up42.com/realms/public/protocol/openid-connect/auth\n    tokenUrl: https://auth.up42.com/realms/public/protocol/openid-connect/token\nscopes:\n- scope: account\n  description: Access to resources of the authenticated user's account\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blacksky-up42-api-openapi.yml\n- scope: budget.r\n  sources:\n  - openapi/blacksky-up42-api-openapi.yml\n- scope: eula.w\n  description: Create/Update/Delete a EULA document\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/blacksky-up42-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksky/refs/heads/main/scopes/blacksky-scopes.yml
summary_line: 3 scopes · clientCredentials/authorizationCode
tags:
- Earth Observation
- Satellite Imagery
- Remote Sensing
- Geospatial Intelligence
- Space
- ISR
- Intelligence Surveillance Reconnaissance
- Tasking
- AI Analytics
- Object Detection
- Defense
- Monitoring
- Spectra
- Gen-3
- NYSE BKSY
token_bound: false
token_urls:
- https://auth.up42.com/realms/public/protocol/openid-connect/token
---
