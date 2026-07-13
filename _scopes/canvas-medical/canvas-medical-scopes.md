---
api_specs:
- filename: canvas-medical-fhir-api-openapi.yml
  format: yaml
  label: Canvas Medical FHIR API
  slug: canvas-medical-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/openapi/canvas-medical-fhir-api-openapi.yml
authorization_urls:
- https://{canvas-instance}.canvasmedical.com/auth/authorize/
description: ''
docs: ''
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Canvas Medical Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Canvas Medical publishes 11 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Canvas Medical API on a user''s behalf.


  Tokens are issued from https://{canvas-instance}.canvasmedical.com/auth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Canvas Medical
provider_slug: canvas-medical
schemes:
- description: Machine-to-machine authentication using client credentials grant. Obtain client_id and client_secret from Canvas admin panel.
  flows:
  - flow: clientCredentials
    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/
  name: OAuth2ClientCredentials
  source: openapi/canvas-medical-fhir-api-openapi.yml
- description: User-delegated access using Authorization Code flow with SMART on FHIR scopes.
  flows:
  - authorizationUrl: https://{canvas-instance}.canvasmedical.com/auth/authorize/
    flow: authorizationCode
    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/
  name: OAuth2AuthCode
  source: openapi/canvas-medical-fhir-api-openapi.yml
scope_count: 11
scope_names:
- patient/*.read
- system/*.read
- system/*.write
- system/Appointment.read
- system/Appointment.write
- system/Observation.read
- system/Observation.write
- system/Patient.read
- system/Patient.write
- user/*.read
- user/*.write
scopes:
- description: Read patient-context FHIR resources
  flows:
  - authorizationCode
  scope: patient/*.read
- description: Read all FHIR resources
  flows:
  - clientCredentials
  scope: system/*.read
- description: Write all FHIR resources
  flows:
  - clientCredentials
  scope: system/*.write
- description: Read Appointment resources
  flows:
  - clientCredentials
  scope: system/Appointment.read
- description: Write Appointment resources
  flows:
  - clientCredentials
  scope: system/Appointment.write
- description: Read Observation resources
  flows:
  - clientCredentials
  scope: system/Observation.read
- description: Write Observation resources
  flows:
  - clientCredentials
  scope: system/Observation.write
- description: Read Patient resources
  flows:
  - clientCredentials
  scope: system/Patient.read
- description: Write Patient resources
  flows:
  - clientCredentials
  scope: system/Patient.write
- description: Read user-context FHIR resources
  flows:
  - authorizationCode
  scope: user/*.read
- description: Write user-context FHIR resources
  flows:
  - authorizationCode
  scope: user/*.write
slug: canvas-medical-scopes
source_filename: canvas-medical-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/canvas-medical-fhir-api-openapi.yml\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/canvas-medical-fhir-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/\n  description: Machine-to-machine authentication using client credentials grant. Obtain client_id\n    and client_secret from Canvas admin panel.\n- name: OAuth2AuthCode\n  source: openapi/canvas-medical-fhir-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{canvas-instance}.canvasmedical.com/auth/authorize/\n    tokenUrl: https://{canvas-instance}.canvasmedical.com/auth/token/\n  description: User-delegated access using Authorization Code flow with SMART on FHIR scopes.\nscopes:\n- scope: patient/*.read\n  description: Read patient-context FHIR resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n\
  - scope: system/*.read\n  description: Read all FHIR resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/*.write\n  description: Write all FHIR resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/Appointment.read\n  description: Read Appointment resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/Appointment.write\n  description: Write Appointment resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/Observation.read\n  description: Read Observation resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/Observation.write\n  description: Write Observation resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n\
  - scope: system/Patient.read\n  description: Read Patient resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: system/Patient.write\n  description: Write Patient resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: user/*.read\n  description: Read user-context FHIR resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n- scope: user/*.write\n  description: Write user-context FHIR resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/canvas-medical-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas-medical/refs/heads/main/scopes/canvas-medical-scopes.yml
summary_line: 11 scopes · clientCredentials/authorizationCode
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Virtual Care
- Clinical Workflows
- Patient Management
- Care Coordination
token_urls:
- https://{canvas-instance}.canvasmedical.com/auth/token/
---
