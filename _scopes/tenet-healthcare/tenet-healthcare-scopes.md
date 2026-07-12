---
authorization_urls:
- https://auth.tenethealth.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Tenet Healthcare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tenet Healthcare publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tenet Healthcare API on a user''s behalf.


  Tokens are issued from https://auth.tenethealth.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tenet Healthcare
provider_slug: tenet-healthcare
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://auth.tenethealth.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tenethealth.com/oauth2/token
  name: smartOnFhir
  source: openapi/tenet-healthcare-fhir-openapi.yml
scope_count: 6
scope_names:
- patient/Appointment.read
- patient/Condition.read
- patient/DocumentReference.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
scopes:
- description: Read patient appointments
  flows:
  - authorizationCode
  scope: patient/Appointment.read
- description: Read patient conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read document references
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: Read medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read clinical observations
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient demographic data
  flows:
  - authorizationCode
  scope: patient/Patient.read
slug: tenet-healthcare-scopes
source_filename: tenet-healthcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tenet-healthcare-fhir-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/tenet-healthcare-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tenethealth.com/oauth2/authorize\n    tokenUrl: https://auth.tenethealth.com/oauth2/token\n  description: SMART on FHIR OAuth 2.0 authorization\nscopes:\n- scope: patient/Appointment.read\n  description: Read patient appointments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n- scope: patient/Condition.read\n  description: Read patient conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n- scope: patient/DocumentReference.read\n  description: Read document references\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read medication requests\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n- scope: patient/Observation.read\n  description: Read clinical observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient demographic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/tenet-healthcare-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenet-healthcare/refs/heads/main/scopes/tenet-healthcare-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Healthcare
- Hospitals
- Ambulatory Surgery Centers
- Revenue Cycle Management
- Fortune 500
token_urls:
- https://auth.tenethealth.com/oauth2/token
---
