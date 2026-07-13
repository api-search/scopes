---
api_specs:
- filename: varian-aria-fhir-openapi.yml
  format: yaml
  label: ARIA FHIR API
  slug: aria-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/openapi/varian-aria-fhir-openapi.yml
authorization_urls:
- https://varian-smart.dynamicfhir.com/core/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Varian Medical Systems Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Varian Medical Systems publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Varian Medical Systems API on a user''s behalf.


  Tokens are issued from https://varian-smart.dynamicfhir.com/core/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Varian Medical Systems
provider_slug: varian-medical-systems
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize
    flow: authorizationCode
    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token
  name: OAuthSMARTonFHIR
  source: openapi/varian-aria-fhir-openapi.yml
scope_count: 11
scope_names:
- launch/patient
- patient/AllergyIntolerance.read
- patient/CarePlan.read
- patient/Condition.read
- patient/DiagnosticReport.read
- patient/DocumentReference.read
- patient/Goal.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
- patient/Procedure.read
scopes:
- description: Patient context launch
  flows:
  - authorizationCode
  scope: launch/patient
- description: Read allergy records
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: Read care plans
  flows:
  - authorizationCode
  scope: patient/CarePlan.read
- description: Read patient conditions/diagnoses
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read diagnostic reports
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.read
- description: Read document references
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: Read treatment goals
  flows:
  - authorizationCode
  scope: patient/Goal.read
- description: Read medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read patient observations/labs
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient demographics
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: Read patient procedures
  flows:
  - authorizationCode
  scope: patient/Procedure.read
slug: varian-medical-systems-scopes
source_filename: varian-medical-systems-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/varian-aria-fhir-openapi.yml\nschemes:\n- name: OAuthSMARTonFHIR\n  source: openapi/varian-aria-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://varian-smart.dynamicfhir.com/core/connect/authorize\n    tokenUrl: https://varian-smart.dynamicfhir.com/core/connect/token\n  description: SMART on FHIR OAuth 2.0 authorization\nscopes:\n- scope: launch/patient\n  description: Patient context launch\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/AllergyIntolerance.read\n  description: Read allergy records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/CarePlan.read\n  description: Read care plans\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/Condition.read\n  description: Read patient conditions/diagnoses\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/DiagnosticReport.read\n  description: Read diagnostic reports\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/DocumentReference.read\n  description: Read document references\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/Goal.read\n  description: Read treatment goals\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/Observation.read\n  description: Read patient observations/labs\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient demographics\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n- scope: patient/Procedure.read\n  description: Read patient procedures\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/varian-aria-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/varian-medical-systems/refs/heads/main/scopes/varian-medical-systems-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- Healthcare
- Oncology
- Medical Devices
- FHIR
- Radiation Therapy
- Health IT
- Fortune 1000
token_urls:
- https://varian-smart.dynamicfhir.com/core/connect/token
---
