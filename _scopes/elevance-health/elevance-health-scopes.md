---
authorization_urls:
- https://patient360c.anthem.com/P360Member/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Elevance Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elevance Health publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elevance Health API on a user''s behalf.


  Tokens are issued from https://patient360c.anthem.com/P360Member/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elevance Health
provider_slug: elevance-health
schemes:
- flows:
  - authorizationUrl: https://patient360c.anthem.com/P360Member/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://patient360c.anthem.com/P360Member/oauth2/token
  name: oauth2
  source: openapi/elevance-health-openapi.yml
scope_count: 3
scope_names:
- launch/patient
- offline_access
- patient/*.read
scopes:
- description: SMART on FHIR patient launch context
  flows:
  - authorizationCode
  scope: launch/patient
- description: Refresh token access
  flows:
  - authorizationCode
  scope: offline_access
- description: Read patient-scoped resources
  flows:
  - authorizationCode
  scope: patient/*.read
slug: elevance-health-scopes
source_filename: elevance-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/elevance-health-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/elevance-health-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient360c.anthem.com/P360Member/oauth2/authorize\n    tokenUrl: https://patient360c.anthem.com/P360Member/oauth2/token\nscopes:\n- scope: launch/patient\n  description: SMART on FHIR patient launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/elevance-health-openapi.yml\n- scope: offline_access\n  description: Refresh token access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/elevance-health-openapi.yml\n- scope: patient/*.read\n  description: Read patient-scoped resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/elevance-health-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/scopes/elevance-health-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Fortune 500
- Healthcare
- Health Insurance
- FHIR
- Interoperability
token_urls:
- https://patient360c.anthem.com/P360Member/oauth2/token
---
