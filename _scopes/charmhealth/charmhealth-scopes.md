---
api_specs:
- filename: charmhealth-fhir-api-openapi.yml
  format: yaml
  label: CharmHealth FHIR API
  slug: fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/openapi/charmhealth-fhir-api-openapi.yml
authorization_urls:
- https://ehr2.charmtracker.com/oauth/v2/auth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Charmhealth Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CharmHealth publishes 7 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the CharmHealth API on a user''s behalf.


  Tokens are issued from https://ehr2.charmtracker.com/oauth/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CharmHealth
provider_slug: charmhealth
schemes:
- description: SMART on FHIR authorization with patient/, user/, and system/ scopes.
  flows:
  - authorizationUrl: https://ehr2.charmtracker.com/oauth/v2/auth
    flow: authorizationCode
    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token
  - flow: clientCredentials
    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token
  name: smartOnFhir
  source: openapi/charmhealth-fhir-api-openapi.yml
scope_count: 7
scope_names:
- launch/patient
- patient/Condition.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
- system/*.read
- user/*.read
scopes:
- description: Patient context launch
  flows:
  - authorizationCode
  scope: launch/patient
- description: Read conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read medication orders
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read observations
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient demographic data
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: Backend services read access
  flows:
  - clientCredentials
  scope: system/*.read
- description: Read all user-accessible resources
  flows:
  - authorizationCode
  scope: user/*.read
slug: charmhealth-scopes
source_filename: charmhealth-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/charmhealth-fhir-api-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/charmhealth-fhir-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ehr2.charmtracker.com/oauth/v2/auth\n    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token\n  - flow: clientCredentials\n    tokenUrl: https://ehr2.charmtracker.com/oauth/v2/token\n  description: SMART on FHIR authorization with patient/, user/, and system/ scopes.\nscopes:\n- scope: launch/patient\n  description: Patient context launch\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n- scope: patient/Condition.read\n  description: Read conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read medication orders\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n\
  - scope: patient/Observation.read\n  description: Read observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient demographic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n- scope: system/*.read\n  description: Backend services read access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n- scope: user/*.read\n  description: Read all user-accessible resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/charmhealth-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charmhealth/refs/heads/main/scopes/charmhealth-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials
tags:
- EHR
- EMR
- FHIR
- Healthcare
- HL7
- Patient Engagement
- Patients
- SMART on FHIR
- US Core
token_urls:
- https://ehr2.charmtracker.com/oauth/v2/token
---
