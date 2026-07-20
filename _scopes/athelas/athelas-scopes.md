---
api_specs:
- filename: athelas-enterprise-openapi.yml
  format: yaml
  label: Athelas Enterprise API
  slug: athelas-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/openapi/athelas-enterprise-openapi.yml
authorization_urls:
- https://onc.api.staging-ehr.athelas.com/authorize
description: ''
docs: https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Athelas Scopes
name_suffix: OAuth Scopes
note: SMART on FHIR v2 granular scopes. All resource scopes use the .rs (read-search) action. Advertised in the server's /.well-known/smart-configuration document.
overview: 'Athelas publishes 31 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Athelas API on a user''s behalf.


  Tokens are issued from https://onc.api.staging-ehr.athelas.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Athelas
provider_slug: athelas
schemes:
- flows:
  - authorizationUrl: https://onc.api.staging-ehr.athelas.com/authorize
    flow: authorizationCode
    tokenUrl: https://onc.api.staging-ehr.athelas.com/token
  - flow: clientCredentials
    tokenUrl: https://onc.api.staging-ehr.athelas.com/token
  name: smartOnFhir
  source: docs.athelas.com FHIR API reference
scope_count: 31
scope_names:
- openid
- profile
- fhirUser
- offline_access
- launch
- launch/patient
- patient/AllergyIntolerance.rs
- patient/CarePlan.rs
- patient/CareTeam.rs
- patient/Condition.rs
- patient/Coverage.rs
- patient/Device.rs
- patient/DiagnosticReport.rs
- patient/DocumentReference.rs
- patient/Encounter.rs
- patient/Goal.rs
- patient/Immunization.rs
- patient/Location.rs
- patient/MedicationDispense.rs
- patient/MedicationRequest.rs
- patient/Observation.rs
- patient/Organization.rs
- patient/Patient.rs
- patient/Practitioner.rs
- patient/PractitionerRole.rs
- patient/Procedure.rs
- patient/Provenance.rs
- patient/RelatedPerson.rs
- patient/ServiceRequest.rs
- patient/Specimen.rs
- system/*.rs
scopes:
- description: OpenID Connect
  flows: []
  scope: openid
- description: User profile
  flows: []
  scope: profile
- description: Resolves the current user as a FHIR resource
  flows: []
  scope: fhirUser
- description: Issue a refresh token
  flows: []
  scope: offline_access
- description: EHR launch context
  flows: []
  scope: launch
- description: Standalone patient launch context
  flows: []
  scope: launch/patient
- description: Allergy and intolerance records
  flows: []
  scope: patient/AllergyIntolerance.rs
- description: Care plans
  flows: []
  scope: patient/CarePlan.rs
- description: Care team members
  flows: []
  scope: patient/CareTeam.rs
- description: All conditions (problems, diagnoses, health concerns)
  flows: []
  scope: patient/Condition.rs
- description: Insurance coverage
  flows: []
  scope: patient/Coverage.rs
- description: Implantable devices
  flows: []
  scope: patient/Device.rs
- description: Diagnostic reports (lab, notes)
  flows: []
  scope: patient/DiagnosticReport.rs
- description: Clinical documents and chart notes
  flows: []
  scope: patient/DocumentReference.rs
- description: Encounters and visits
  flows: []
  scope: patient/Encounter.rs
- description: Health goals
  flows: []
  scope: patient/Goal.rs
- description: Immunization records
  flows: []
  scope: patient/Immunization.rs
- description: Practice locations
  flows: []
  scope: patient/Location.rs
- description: Medication dispense records
  flows: []
  scope: patient/MedicationDispense.rs
- description: Medication requests and prescriptions
  flows: []
  scope: patient/MedicationRequest.rs
- description: All observations (vitals, labs, surveys, SDOH)
  flows: []
  scope: patient/Observation.rs
- description: Organizations
  flows: []
  scope: patient/Organization.rs
- description: Patient demographics
  flows: []
  scope: patient/Patient.rs
- description: Practitioners
  flows: []
  scope: patient/Practitioner.rs
- description: Practitioner roles
  flows: []
  scope: patient/PractitionerRole.rs
- description: Procedures
  flows: []
  scope: patient/Procedure.rs
- description: Provenance (data source/attribution) records
  flows: []
  scope: patient/Provenance.rs
- description: Related persons
  flows: []
  scope: patient/RelatedPerson.rs
- description: Service requests
  flows: []
  scope: patient/ServiceRequest.rs
- description: Specimens
  flows: []
  scope: patient/Specimen.rs
- description: System-level read-search across all resources (Backend Services / bulk data)
  flows: []
  scope: system/*.rs
slug: athelas-scopes
source_filename: athelas-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api\ndocs: https://docs.athelas.com/air_developer/fhir_api/commure_ehr_fhir_api\napi: Commure EHR FHIR API\nnote: >-\n  SMART on FHIR v2 granular scopes. All resource scopes use the .rs (read-search)\n  action. Advertised in the server's /.well-known/smart-configuration document.\nschemes:\n- name: smartOnFhir\n  source: docs.athelas.com FHIR API reference\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://onc.api.staging-ehr.athelas.com/authorize\n    tokenUrl: https://onc.api.staging-ehr.athelas.com/token\n  - flow: clientCredentials\n    tokenUrl: https://onc.api.staging-ehr.athelas.com/token\nscopes:\n- scope: openid\n  description: OpenID Connect\n  group: context\n- scope: profile\n  description: User profile\n  group: context\n- scope: fhirUser\n  description: Resolves the current user as a FHIR resource\n  group: context\n- scope: offline_access\n\
  \  description: Issue a refresh token\n  group: context\n- scope: launch\n  description: EHR launch context\n  group: context\n- scope: launch/patient\n  description: Standalone patient launch context\n  group: context\n- scope: patient/AllergyIntolerance.rs\n  description: Allergy and intolerance records\n  group: patient\n- scope: patient/CarePlan.rs\n  description: Care plans\n  group: patient\n- scope: patient/CareTeam.rs\n  description: Care team members\n  group: patient\n- scope: patient/Condition.rs\n  description: All conditions (problems, diagnoses, health concerns)\n  group: patient\n- scope: patient/Coverage.rs\n  description: Insurance coverage\n  group: patient\n- scope: patient/Device.rs\n  description: Implantable devices\n  group: patient\n- scope: patient/DiagnosticReport.rs\n  description: Diagnostic reports (lab, notes)\n  group: patient\n- scope: patient/DocumentReference.rs\n  description: Clinical documents and chart notes\n  group: patient\n- scope: patient/Encounter.rs\n\
  \  description: Encounters and visits\n  group: patient\n- scope: patient/Goal.rs\n  description: Health goals\n  group: patient\n- scope: patient/Immunization.rs\n  description: Immunization records\n  group: patient\n- scope: patient/Location.rs\n  description: Practice locations\n  group: patient\n- scope: patient/MedicationDispense.rs\n  description: Medication dispense records\n  group: patient\n- scope: patient/MedicationRequest.rs\n  description: Medication requests and prescriptions\n  group: patient\n- scope: patient/Observation.rs\n  description: All observations (vitals, labs, surveys, SDOH)\n  group: patient\n- scope: patient/Organization.rs\n  description: Organizations\n  group: patient\n- scope: patient/Patient.rs\n  description: Patient demographics\n  group: patient\n- scope: patient/Practitioner.rs\n  description: Practitioners\n  group: patient\n- scope: patient/PractitionerRole.rs\n  description: Practitioner roles\n  group: patient\n- scope: patient/Procedure.rs\n\
  \  description: Procedures\n  group: patient\n- scope: patient/Provenance.rs\n  description: Provenance (data source/attribution) records\n  group: patient\n- scope: patient/RelatedPerson.rs\n  description: Related persons\n  group: patient\n- scope: patient/ServiceRequest.rs\n  description: Service requests\n  group: patient\n- scope: patient/Specimen.rs\n  description: Specimens\n  group: patient\n- scope: system/*.rs\n  description: System-level read-search across all resources (Backend Services / bulk data)\n  group: system\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/scopes/athelas-scopes.yml
summary_line: 31 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Electronic Health Records
- FHIR
- Revenue Cycle Management
- Medical Devices
- SMART on FHIR
- Interoperability
- AI
token_urls:
- https://onc.api.staging-ehr.athelas.com/token
---
