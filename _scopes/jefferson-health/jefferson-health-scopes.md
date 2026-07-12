---
authorization_urls:
- https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Jefferson Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jefferson Health publishes 13 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jefferson Health API on a user''s behalf.


  Tokens are issued from https://fhir.jefferson.edu/FHIRProxy/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jefferson Health
provider_slug: jefferson-health
schemes:
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token
  name: smartOnFhir
  source: openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml
scope_count: 13
scope_names:
- fhirUser
- launch
- offline_access
- openid
- patient/AllergyIntolerance.read
- patient/Condition.read
- patient/DocumentReference.read
- patient/Encounter.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
- system/Patient.read
- user/Patient.read
scopes:
- description: Identity of the user launching the app
  flows:
  - authorizationCode
  scope: fhirUser
- description: EHR launch context for provider-launched apps
  flows:
  - authorizationCode
  scope: launch
- description: Refresh token for long-lived access
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Read the launching patient's allergies
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: Read the launching patient's conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read the launching patient's documents
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: Read the launching patient's encounters
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read the launching patient's medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read the launching patient's observations
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read the launching patient's demographics
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: System-level Patient read (Bulk Data)
  flows:
  - authorizationCode
  scope: system/Patient.read
- description: Read Patient as the launching user
  flows:
  - authorizationCode
  scope: user/Patient.read
slug: jefferson-health-scopes
source_filename: jefferson-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize\n    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app\n    launches.\nscopes:\n- scope: fhirUser\n  description: Identity of the user launching the app\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: launch\n  description: EHR launch context for provider-launched apps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: offline_access\n  description: Refresh token for long-lived access\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: openid\n  description: OpenID Connect authentication\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/AllergyIntolerance.read\n  description: Read the launching patient's allergies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/Condition.read\n  description: Read the launching patient's conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/DocumentReference.read\n  description: Read the launching patient's documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/Encounter.read\n  description: Read the launching patient's encounters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n\
  - scope: patient/MedicationRequest.read\n  description: Read the launching patient's medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/Observation.read\n  description: Read the launching patient's observations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: patient/Patient.read\n  description: Read the launching patient's demographics\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: system/Patient.read\n  description: System-level Patient read (Bulk Data)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n- scope: user/Patient.read\n  description: Read Patient as the launching user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/scopes/jefferson-health-scopes.yml
summary_line: 13 scopes · authorizationCode
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
token_urls:
- https://fhir.jefferson.edu/FHIRProxy/oauth2/token
---
