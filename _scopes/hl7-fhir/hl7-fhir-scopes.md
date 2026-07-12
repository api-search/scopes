---
authorization_urls:
- https://auth.example.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hl7 Fhir Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HL7 FHIR publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HL7 FHIR API on a user''s behalf.


  Tokens are issued from https://auth.example.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HL7 FHIR
provider_slug: hl7-fhir
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://auth.example.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.example.com/token
  name: SMARTonFHIR
  source: openapi/hl7-fhir-r4-openapi.yml
scope_count: 7
scope_names:
- launch/patient
- openid
- patient/Condition.read
- patient/Encounter.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
scopes:
- description: Patient context launch
  flows:
  - authorizationCode
  scope: launch/patient
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
- description: Read conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read encounters
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read observations
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient data
  flows:
  - authorizationCode
  scope: patient/Patient.read
slug: hl7-fhir-scopes
source_filename: hl7-fhir-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hl7-fhir-r4-openapi.yml\nschemes:\n- name: SMARTonFHIR\n  source: openapi/hl7-fhir-r4-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.example.com/authorize\n    tokenUrl: https://auth.example.com/token\n  description: SMART on FHIR OAuth 2.0 authorization\nscopes:\n- scope: launch/patient\n  description: Patient context launch\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: patient/Condition.read\n  description: Read conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: patient/Encounter.read\n  description: Read encounters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: patient/MedicationRequest.read\n  description:\
  \ Read medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: patient/Observation.read\n  description: Read observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hl7-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hl7-fhir/refs/heads/main/scopes/hl7-fhir-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Clinical
- FHIR
- Healthcare
- HL7
- Interoperability
token_urls:
- https://auth.example.com/token
---
