---
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Earth Engine Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Earth Engine REST publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Earth Engine REST API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Earth Engine REST
provider_slug: google-earth-engine
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/earth-engine.yml
scope_count: 3
scope_names:
- https://www.googleapis.com/auth/cloud-platform
- https://www.googleapis.com/auth/earthengine
- https://www.googleapis.com/auth/earthengine.readonly
scopes:
- description: View and manage your data across Google Cloud Platform services
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/cloud-platform
- description: View and manage your Earth Engine data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/earthengine
- description: View your Earth Engine data
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/earthengine.readonly
slug: google-earth-engine-scopes
source_filename: google-earth-engine-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/earth-engine.yml\nschemes:\n- name: oauth2\n  source: openapi/earth-engine.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/cloud-platform\n  description: View and manage your data across Google Cloud Platform services\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/earth-engine.yml\n- scope: https://www.googleapis.com/auth/earthengine\n  description: View and manage your Earth Engine data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/earth-engine.yml\n- scope: https://www.googleapis.com/auth/earthengine.readonly\n  description: View your Earth Engine data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/earth-engine.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-earth-engine/refs/heads/main/scopes/google-earth-engine-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Climate
- Earth Observation
- Environmental
- Geospatial
- GIS
- Google
- Remote Sensing
- Satellite Imagery
token_urls:
- https://oauth2.googleapis.com/token
---
