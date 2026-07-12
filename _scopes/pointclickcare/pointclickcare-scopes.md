---
authorization_urls:
- https://login.pointclickcare.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Pointclickcare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PointClickCare publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PointClickCare API on a user''s behalf.


  Tokens are issued from https://login.pointclickcare.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PointClickCare
provider_slug: pointclickcare
schemes:
- description: OAuth2 authorization code flow via PointClickCare identity server
  flows:
  - authorizationUrl: https://login.pointclickcare.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://login.pointclickcare.com/oauth2/token
  name: oauth2
  source: openapi/pointclickcare-ehr-openapi.yml
scope_count: 3
scope_names:
- clinical.read
- facility.read
- patient.read
scopes:
- description: Read clinical data (vitals, medications, assessments)
  flows:
  - authorizationCode
  scope: clinical.read
- description: Read facility information
  flows:
  - authorizationCode
  scope: facility.read
- description: Read patient demographics
  flows:
  - authorizationCode
  scope: patient.read
slug: pointclickcare-scopes
source_filename: pointclickcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pointclickcare-ehr-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/pointclickcare-ehr-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.pointclickcare.com/oauth2/authorize\n    tokenUrl: https://login.pointclickcare.com/oauth2/token\n  description: OAuth2 authorization code flow via PointClickCare identity server\nscopes:\n- scope: clinical.read\n  description: Read clinical data (vitals, medications, assessments)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pointclickcare-ehr-openapi.yml\n- scope: facility.read\n  description: Read facility information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pointclickcare-ehr-openapi.yml\n- scope: patient.read\n  description: Read patient demographics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pointclickcare-ehr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pointclickcare/refs/heads/main/scopes/pointclickcare-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Healthcare
- Long-Term Care
- Post-Acute Care
- EHR
- FHIR
- Senior Care
- Interoperability
token_urls:
- https://login.pointclickcare.com/oauth2/token
---
