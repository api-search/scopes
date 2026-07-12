---
authorization_urls:
- https://api.chs.net/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Community Health Systems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Community Health Systems publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Community Health Systems API on a user''s behalf.


  Tokens are issued from https://api.chs.net/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Community Health Systems
provider_slug: community-health-systems
schemes:
- flows:
  - authorizationUrl: https://api.chs.net/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.chs.net/oauth2/token
  name: oauth2
  source: openapi/chs-patient-access-api-openapi.yml
scope_count: 2
scope_names:
- launch/patient
- patient/*.read
scopes:
- description: Patient launch context
  flows:
  - authorizationCode
  scope: launch/patient
- description: Read access to patient data
  flows:
  - authorizationCode
  scope: patient/*.read
slug: community-health-systems-scopes
source_filename: community-health-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chs-patient-access-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/chs-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.chs.net/oauth2/authorize\n    tokenUrl: https://api.chs.net/oauth2/token\nscopes:\n- scope: launch/patient\n  description: Patient launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chs-patient-access-api-openapi.yml\n- scope: patient/*.read\n  description: Read access to patient data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chs-patient-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community-health-systems/refs/heads/main/scopes/community-health-systems-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- CMS-9115-F
- FHIR
- Healthcare
- Hospitals
- Interoperability
- Patient Access
- Provider Directory
- SMART-on-FHIR
- Fortune 500
token_urls:
- https://api.chs.net/oauth2/token
---
