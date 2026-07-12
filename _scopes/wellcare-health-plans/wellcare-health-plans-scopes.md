---
authorization_urls:
- https://partners.centene.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wellcare Health Plans Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'wellcare-health-plans publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the wellcare-health-plans API on a user''s behalf.


  Tokens are issued from https://partners.centene.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: wellcare-health-plans
provider_slug: wellcare-health-plans
schemes:
- description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.
  flows:
  - authorizationUrl: https://partners.centene.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://partners.centene.com/oauth2/token
  name: smartOnFhir
  source: openapi/wellcare-fhir-patient-access-api-openapi.yml
scope_count: 8
scope_names:
- patient/Condition.read
- patient/Coverage.read
- patient/Encounter.read
- patient/ExplanationOfBenefit.read
- patient/Immunization.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
scopes:
- description: Read diagnosed conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read coverage and enrollment data
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: Read care encounters
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read claims and EOB data
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: Read immunization records
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: Read medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read observations and lab results
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient demographic data
  flows:
  - authorizationCode
  scope: patient/Patient.read
slug: wellcare-health-plans-scopes
source_filename: wellcare-health-plans-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellcare-fhir-patient-access-api-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/wellcare-fhir-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://partners.centene.com/oauth2/authorize\n    tokenUrl: https://partners.centene.com/oauth2/token\n  description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.\nscopes:\n- scope: patient/Condition.read\n  description: Read diagnosed conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Coverage.read\n  description: Read coverage and enrollment data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Encounter.read\n  description: Read care encounters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n\
  - scope: patient/ExplanationOfBenefit.read\n  description: Read claims and EOB data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Immunization.read\n  description: Read immunization records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Observation.read\n  description: Read observations and lab results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient demographic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/scopes/wellcare-health-plans-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Fortune 500
token_urls:
- https://partners.centene.com/oauth2/token
---
