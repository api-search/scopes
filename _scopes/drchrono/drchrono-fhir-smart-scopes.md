---
api_specs:
- filename: drchrono-administrative-api-openapi.yml
  format: yaml
  label: drchrono Administrative API
  slug: drchrono-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-administrative-api-openapi.yml
- filename: drchrono-audit-api-openapi.yml
  format: yaml
  label: drchrono Audit API
  slug: drchrono-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-audit-api-openapi.yml
- filename: drchrono-availability-api-openapi.yml
  format: yaml
  label: drchrono Availability API
  slug: drchrono-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-availability-api-openapi.yml
- filename: drchrono-billing-api-openapi.yml
  format: yaml
  label: drchrono Billing API
  slug: drchrono-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-billing-api-openapi.yml
- filename: drchrono-clinical-api-openapi.yml
  format: yaml
  label: drchrono Clinical API
  slug: drchrono-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-clinical-api-openapi.yml
- filename: drchrono-practice-management-api-openapi.yml
  format: yaml
  label: drchrono Practice Management API
  slug: drchrono-practice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-practice-management-api-openapi.yml
authorization_urls: []
description: SMART App Launch scopes advertised by the DrChrono SMART on FHIR R4 authorization server, read verbatim from the scopes_supported array of the server's own smart-configuration discovery document on 2026-08-14. These are a SEPARATE vocabulary from the DrChrono REST v4 OAuth scopes in scopes/drchrono-scopes.yml — a token from one authorization server is not valid against the other.
docs: https://drchrono-fhirpresentation.everhealthsoftware.com/drchrono/498711/r4/Home/ApiDocumentation
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Drchrono Fhir Smart Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'drchrono publishes 233 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the drchrono API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: drchrono
provider_slug: drchrono
schemes: []
scope_count: 233
scope_names:
- openid
- profile
- IdentityScope
- fhirUser
- FHIRApi
- user/AllergyIntolerance.read
- patient/AllergyIntolerance.read
- system/AllergyIntolerance.read
- user/Binary.read
- patient/Binary.read
- system/Binary.read
- user/CapabilityStatement.read
- patient/CapabilityStatement.read
- system/CapabilityStatement.read
- user/CarePlan.read
- patient/CarePlan.read
- system/CarePlan.read
- user/CareTeam.read
- patient/CareTeam.read
- system/CareTeam.read
- user/ClinicalImpression.read
- patient/ClinicalImpression.read
- system/ClinicalImpression.read
- user/Composition.read
- patient/Composition.read
- system/Composition.read
- user/Condition.read
- patient/Condition.read
- system/Condition.read
- user/Coverage.read
- patient/Coverage.read
- system/Coverage.read
- user/Device.read
- patient/Device.read
- system/Device.read
- user/DiagnosticReport.read
- patient/DiagnosticReport.read
- system/DiagnosticReport.read
- user/DocumentReference.read
- patient/DocumentReference.read
- system/DocumentReference.read
- user/Encounter.read
- patient/Encounter.read
- system/Encounter.read
- user/Goal.read
- patient/Goal.read
- system/Goal.read
- user/Immunization.read
- patient/Immunization.read
- system/Immunization.read
- user/Location.read
- patient/Location.read
- system/Location.read
- user/Media.read
- patient/Media.read
- system/Media.read
- user/Medication.read
- patient/Medication.read
- system/Medication.read
- user/MedicationDispense.read
- patient/MedicationDispense.read
- system/MedicationDispense.read
- user/MedicationRequest.read
- patient/MedicationRequest.read
- system/MedicationRequest.read
- user/MedicationStatement.read
- patient/MedicationStatement.read
- system/MedicationStatement.read
- user/Observation.read
- patient/Observation.read
- system/Observation.read
- user/Organization.read
- patient/Organization.read
- system/Organization.read
- user/Parameters.read
- patient/Parameters.read
- system/Parameters.read
- user/Patient.read
- patient/Patient.read
- system/Patient.read
- user/Person.read
- patient/Person.read
- system/Person.read
- user/Practitioner.read
- patient/Practitioner.read
- system/Practitioner.read
- user/PractitionerRole.read
- patient/PractitionerRole.read
- system/PractitionerRole.read
- user/Procedure.read
- patient/Procedure.read
- system/Procedure.read
- user/Provenance.read
- patient/Provenance.read
- system/Provenance.read
- user/RelatedPerson.read
- patient/RelatedPerson.read
- system/RelatedPerson.read
- user/ServiceRequest.read
- patient/ServiceRequest.read
- system/ServiceRequest.read
- user/Specimen.read
- patient/Specimen.read
- system/Specimen.read
- launch
- launch/patient
- user/AllergyIntolerance.rs
- patient/AllergyIntolerance.rs
- system/AllergyIntolerance.rs
- user/Binary.rs
- patient/Binary.rs
- system/Binary.rs
- user/CapabilityStatement.rs
- patient/CapabilityStatement.rs
- system/CapabilityStatement.rs
- user/CarePlan.rs
- patient/CarePlan.rs
- system/CarePlan.rs
- user/CareTeam.rs
- patient/CareTeam.rs
- system/CareTeam.rs
- user/ClinicalImpression.rs
- patient/ClinicalImpression.rs
- system/ClinicalImpression.rs
- user/Composition.rs
- patient/Composition.rs
- system/Composition.rs
- user/Condition.rs
- patient/Condition.rs
- system/Condition.rs
- user/Coverage.rs
- patient/Coverage.rs
- system/Coverage.rs
- user/Device.rs
- patient/Device.rs
- system/Device.rs
- user/DiagnosticReport.rs
- patient/DiagnosticReport.rs
- system/DiagnosticReport.rs
- user/DocumentReference.rs
- patient/DocumentReference.rs
- system/DocumentReference.rs
- user/Encounter.rs
- patient/Encounter.rs
- system/Encounter.rs
- user/Goal.rs
- patient/Goal.rs
- system/Goal.rs
- user/Immunization.rs
- patient/Immunization.rs
- system/Immunization.rs
- user/Location.rs
- patient/Location.rs
- system/Location.rs
- user/Media.rs
- patient/Media.rs
- system/Media.rs
- user/Medication.rs
- patient/Medication.rs
- system/Medication.rs
- user/MedicationDispense.rs
- patient/MedicationDispense.rs
- system/MedicationDispense.rs
- user/MedicationRequest.rs
- patient/MedicationRequest.rs
- system/MedicationRequest.rs
- user/MedicationStatement.rs
- patient/MedicationStatement.rs
- system/MedicationStatement.rs
- user/Observation.rs
- patient/Observation.rs
- system/Observation.rs
- user/Organization.rs
- patient/Organization.rs
- system/Organization.rs
- user/Parameters.rs
- patient/Parameters.rs
- system/Parameters.rs
- user/Patient.rs
- patient/Patient.rs
- system/Patient.rs
- user/Person.rs
- patient/Person.rs
- system/Person.rs
- user/Practitioner.rs
- patient/Practitioner.rs
- system/Practitioner.rs
- user/PractitionerRole.rs
- patient/PractitionerRole.rs
- system/PractitionerRole.rs
- user/Procedure.rs
- patient/Procedure.rs
- system/Procedure.rs
- user/Provenance.rs
- patient/Provenance.rs
- system/Provenance.rs
- user/RelatedPerson.rs
- patient/RelatedPerson.rs
- system/RelatedPerson.rs
- user/ServiceRequest.rs
- patient/ServiceRequest.rs
- system/ServiceRequest.rs
- user/Specimen.rs
- patient/Specimen.rs
- system/Specimen.rs
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- offline_access
scopes:
- description: ''
  flows: []
  scope: openid
- description: ''
  flows: []
  scope: profile
- description: ''
  flows: []
  scope: IdentityScope
- description: ''
  flows: []
  scope: fhirUser
- description: ''
  flows: []
  scope: FHIRApi
- description: ''
  flows: []
  scope: user/AllergyIntolerance.read
- description: ''
  flows: []
  scope: patient/AllergyIntolerance.read
- description: ''
  flows: []
  scope: system/AllergyIntolerance.read
- description: ''
  flows: []
  scope: user/Binary.read
- description: ''
  flows: []
  scope: patient/Binary.read
- description: ''
  flows: []
  scope: system/Binary.read
- description: ''
  flows: []
  scope: user/CapabilityStatement.read
- description: ''
  flows: []
  scope: patient/CapabilityStatement.read
- description: ''
  flows: []
  scope: system/CapabilityStatement.read
- description: ''
  flows: []
  scope: user/CarePlan.read
- description: ''
  flows: []
  scope: patient/CarePlan.read
- description: ''
  flows: []
  scope: system/CarePlan.read
- description: ''
  flows: []
  scope: user/CareTeam.read
- description: ''
  flows: []
  scope: patient/CareTeam.read
- description: ''
  flows: []
  scope: system/CareTeam.read
- description: ''
  flows: []
  scope: user/ClinicalImpression.read
- description: ''
  flows: []
  scope: patient/ClinicalImpression.read
- description: ''
  flows: []
  scope: system/ClinicalImpression.read
- description: ''
  flows: []
  scope: user/Composition.read
- description: ''
  flows: []
  scope: patient/Composition.read
- description: ''
  flows: []
  scope: system/Composition.read
- description: ''
  flows: []
  scope: user/Condition.read
- description: ''
  flows: []
  scope: patient/Condition.read
- description: ''
  flows: []
  scope: system/Condition.read
- description: ''
  flows: []
  scope: user/Coverage.read
- description: ''
  flows: []
  scope: patient/Coverage.read
- description: ''
  flows: []
  scope: system/Coverage.read
- description: ''
  flows: []
  scope: user/Device.read
- description: ''
  flows: []
  scope: patient/Device.read
- description: ''
  flows: []
  scope: system/Device.read
- description: ''
  flows: []
  scope: user/DiagnosticReport.read
- description: ''
  flows: []
  scope: patient/DiagnosticReport.read
- description: ''
  flows: []
  scope: system/DiagnosticReport.read
- description: ''
  flows: []
  scope: user/DocumentReference.read
- description: ''
  flows: []
  scope: patient/DocumentReference.read
- description: ''
  flows: []
  scope: system/DocumentReference.read
- description: ''
  flows: []
  scope: user/Encounter.read
- description: ''
  flows: []
  scope: patient/Encounter.read
- description: ''
  flows: []
  scope: system/Encounter.read
- description: ''
  flows: []
  scope: user/Goal.read
- description: ''
  flows: []
  scope: patient/Goal.read
- description: ''
  flows: []
  scope: system/Goal.read
- description: ''
  flows: []
  scope: user/Immunization.read
- description: ''
  flows: []
  scope: patient/Immunization.read
- description: ''
  flows: []
  scope: system/Immunization.read
- description: ''
  flows: []
  scope: user/Location.read
- description: ''
  flows: []
  scope: patient/Location.read
- description: ''
  flows: []
  scope: system/Location.read
- description: ''
  flows: []
  scope: user/Media.read
- description: ''
  flows: []
  scope: patient/Media.read
- description: ''
  flows: []
  scope: system/Media.read
- description: ''
  flows: []
  scope: user/Medication.read
- description: ''
  flows: []
  scope: patient/Medication.read
- description: ''
  flows: []
  scope: system/Medication.read
- description: ''
  flows: []
  scope: user/MedicationDispense.read
- description: ''
  flows: []
  scope: patient/MedicationDispense.read
- description: ''
  flows: []
  scope: system/MedicationDispense.read
- description: ''
  flows: []
  scope: user/MedicationRequest.read
- description: ''
  flows: []
  scope: patient/MedicationRequest.read
- description: ''
  flows: []
  scope: system/MedicationRequest.read
- description: ''
  flows: []
  scope: user/MedicationStatement.read
- description: ''
  flows: []
  scope: patient/MedicationStatement.read
- description: ''
  flows: []
  scope: system/MedicationStatement.read
- description: ''
  flows: []
  scope: user/Observation.read
- description: ''
  flows: []
  scope: patient/Observation.read
- description: ''
  flows: []
  scope: system/Observation.read
- description: ''
  flows: []
  scope: user/Organization.read
- description: ''
  flows: []
  scope: patient/Organization.read
- description: ''
  flows: []
  scope: system/Organization.read
- description: ''
  flows: []
  scope: user/Parameters.read
- description: ''
  flows: []
  scope: patient/Parameters.read
- description: ''
  flows: []
  scope: system/Parameters.read
- description: ''
  flows: []
  scope: user/Patient.read
- description: ''
  flows: []
  scope: patient/Patient.read
- description: ''
  flows: []
  scope: system/Patient.read
- description: ''
  flows: []
  scope: user/Person.read
- description: ''
  flows: []
  scope: patient/Person.read
- description: ''
  flows: []
  scope: system/Person.read
- description: ''
  flows: []
  scope: user/Practitioner.read
- description: ''
  flows: []
  scope: patient/Practitioner.read
- description: ''
  flows: []
  scope: system/Practitioner.read
- description: ''
  flows: []
  scope: user/PractitionerRole.read
- description: ''
  flows: []
  scope: patient/PractitionerRole.read
- description: ''
  flows: []
  scope: system/PractitionerRole.read
- description: ''
  flows: []
  scope: user/Procedure.read
- description: ''
  flows: []
  scope: patient/Procedure.read
- description: ''
  flows: []
  scope: system/Procedure.read
- description: ''
  flows: []
  scope: user/Provenance.read
- description: ''
  flows: []
  scope: patient/Provenance.read
- description: ''
  flows: []
  scope: system/Provenance.read
- description: ''
  flows: []
  scope: user/RelatedPerson.read
- description: ''
  flows: []
  scope: patient/RelatedPerson.read
- description: ''
  flows: []
  scope: system/RelatedPerson.read
- description: ''
  flows: []
  scope: user/ServiceRequest.read
- description: ''
  flows: []
  scope: patient/ServiceRequest.read
- description: ''
  flows: []
  scope: system/ServiceRequest.read
- description: ''
  flows: []
  scope: user/Specimen.read
- description: ''
  flows: []
  scope: patient/Specimen.read
- description: ''
  flows: []
  scope: system/Specimen.read
- description: ''
  flows: []
  scope: launch
- description: ''
  flows: []
  scope: launch/patient
- description: ''
  flows: []
  scope: user/AllergyIntolerance.rs
- description: ''
  flows: []
  scope: patient/AllergyIntolerance.rs
- description: ''
  flows: []
  scope: system/AllergyIntolerance.rs
- description: ''
  flows: []
  scope: user/Binary.rs
- description: ''
  flows: []
  scope: patient/Binary.rs
- description: ''
  flows: []
  scope: system/Binary.rs
- description: ''
  flows: []
  scope: user/CapabilityStatement.rs
- description: ''
  flows: []
  scope: patient/CapabilityStatement.rs
- description: ''
  flows: []
  scope: system/CapabilityStatement.rs
- description: ''
  flows: []
  scope: user/CarePlan.rs
- description: ''
  flows: []
  scope: patient/CarePlan.rs
- description: ''
  flows: []
  scope: system/CarePlan.rs
- description: ''
  flows: []
  scope: user/CareTeam.rs
- description: ''
  flows: []
  scope: patient/CareTeam.rs
- description: ''
  flows: []
  scope: system/CareTeam.rs
- description: ''
  flows: []
  scope: user/ClinicalImpression.rs
- description: ''
  flows: []
  scope: patient/ClinicalImpression.rs
- description: ''
  flows: []
  scope: system/ClinicalImpression.rs
- description: ''
  flows: []
  scope: user/Composition.rs
- description: ''
  flows: []
  scope: patient/Composition.rs
- description: ''
  flows: []
  scope: system/Composition.rs
- description: ''
  flows: []
  scope: user/Condition.rs
- description: ''
  flows: []
  scope: patient/Condition.rs
- description: ''
  flows: []
  scope: system/Condition.rs
- description: ''
  flows: []
  scope: user/Coverage.rs
- description: ''
  flows: []
  scope: patient/Coverage.rs
- description: ''
  flows: []
  scope: system/Coverage.rs
- description: ''
  flows: []
  scope: user/Device.rs
- description: ''
  flows: []
  scope: patient/Device.rs
- description: ''
  flows: []
  scope: system/Device.rs
- description: ''
  flows: []
  scope: user/DiagnosticReport.rs
- description: ''
  flows: []
  scope: patient/DiagnosticReport.rs
- description: ''
  flows: []
  scope: system/DiagnosticReport.rs
- description: ''
  flows: []
  scope: user/DocumentReference.rs
- description: ''
  flows: []
  scope: patient/DocumentReference.rs
- description: ''
  flows: []
  scope: system/DocumentReference.rs
- description: ''
  flows: []
  scope: user/Encounter.rs
- description: ''
  flows: []
  scope: patient/Encounter.rs
- description: ''
  flows: []
  scope: system/Encounter.rs
- description: ''
  flows: []
  scope: user/Goal.rs
- description: ''
  flows: []
  scope: patient/Goal.rs
- description: ''
  flows: []
  scope: system/Goal.rs
- description: ''
  flows: []
  scope: user/Immunization.rs
- description: ''
  flows: []
  scope: patient/Immunization.rs
- description: ''
  flows: []
  scope: system/Immunization.rs
- description: ''
  flows: []
  scope: user/Location.rs
- description: ''
  flows: []
  scope: patient/Location.rs
- description: ''
  flows: []
  scope: system/Location.rs
- description: ''
  flows: []
  scope: user/Media.rs
- description: ''
  flows: []
  scope: patient/Media.rs
- description: ''
  flows: []
  scope: system/Media.rs
- description: ''
  flows: []
  scope: user/Medication.rs
- description: ''
  flows: []
  scope: patient/Medication.rs
- description: ''
  flows: []
  scope: system/Medication.rs
- description: ''
  flows: []
  scope: user/MedicationDispense.rs
- description: ''
  flows: []
  scope: patient/MedicationDispense.rs
- description: ''
  flows: []
  scope: system/MedicationDispense.rs
- description: ''
  flows: []
  scope: user/MedicationRequest.rs
- description: ''
  flows: []
  scope: patient/MedicationRequest.rs
- description: ''
  flows: []
  scope: system/MedicationRequest.rs
- description: ''
  flows: []
  scope: user/MedicationStatement.rs
- description: ''
  flows: []
  scope: patient/MedicationStatement.rs
- description: ''
  flows: []
  scope: system/MedicationStatement.rs
- description: ''
  flows: []
  scope: user/Observation.rs
- description: ''
  flows: []
  scope: patient/Observation.rs
- description: ''
  flows: []
  scope: system/Observation.rs
- description: ''
  flows: []
  scope: user/Organization.rs
- description: ''
  flows: []
  scope: patient/Organization.rs
- description: ''
  flows: []
  scope: system/Organization.rs
- description: ''
  flows: []
  scope: user/Parameters.rs
- description: ''
  flows: []
  scope: patient/Parameters.rs
- description: ''
  flows: []
  scope: system/Parameters.rs
- description: ''
  flows: []
  scope: user/Patient.rs
- description: ''
  flows: []
  scope: patient/Patient.rs
- description: ''
  flows: []
  scope: system/Patient.rs
- description: ''
  flows: []
  scope: user/Person.rs
- description: ''
  flows: []
  scope: patient/Person.rs
- description: ''
  flows: []
  scope: system/Person.rs
- description: ''
  flows: []
  scope: user/Practitioner.rs
- description: ''
  flows: []
  scope: patient/Practitioner.rs
- description: ''
  flows: []
  scope: system/Practitioner.rs
- description: ''
  flows: []
  scope: user/PractitionerRole.rs
- description: ''
  flows: []
  scope: patient/PractitionerRole.rs
- description: ''
  flows: []
  scope: system/PractitionerRole.rs
- description: ''
  flows: []
  scope: user/Procedure.rs
- description: ''
  flows: []
  scope: patient/Procedure.rs
- description: ''
  flows: []
  scope: system/Procedure.rs
- description: ''
  flows: []
  scope: user/Provenance.rs
- description: ''
  flows: []
  scope: patient/Provenance.rs
- description: ''
  flows: []
  scope: system/Provenance.rs
- description: ''
  flows: []
  scope: user/RelatedPerson.rs
- description: ''
  flows: []
  scope: patient/RelatedPerson.rs
- description: ''
  flows: []
  scope: system/RelatedPerson.rs
- description: ''
  flows: []
  scope: user/ServiceRequest.rs
- description: ''
  flows: []
  scope: patient/ServiceRequest.rs
- description: ''
  flows: []
  scope: system/ServiceRequest.rs
- description: ''
  flows: []
  scope: user/Specimen.rs
- description: ''
  flows: []
  scope: patient/Specimen.rs
- description: ''
  flows: []
  scope: system/Specimen.rs
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure
- description: ''
  flows: []
  scope: offline_access
slug: drchrono-fhir-smart-scopes
source_filename: drchrono-fhir-smart-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://drchrono-fhirpresentation.everhealthsoftware.com/fhir/drchrono/498711/r4/.well-known/smart-configuration\ndocs: https://drchrono-fhirpresentation.everhealthsoftware.com/drchrono/498711/r4/Home/ApiDocumentation\nname: drchrono SMART on FHIR OAuth Scopes\ndescription: SMART App Launch scopes advertised by the DrChrono SMART on FHIR R4 authorization server, read verbatim\n  from the scopes_supported array of the server's own smart-configuration discovery document on 2026-08-14. These\n  are a SEPARATE vocabulary from the DrChrono REST v4 OAuth scopes in scopes/drchrono-scopes.yml — a token from\n  one authorization server is not valid against the other.\nauthorization_server: https://drchrono-fhir.everhealthsoftware.com/core\nauthorization_endpoint: https://drchrono-fhir.everhealthsoftware.com/core/connect/authorize\ntoken_endpoint: https://drchrono-fhir.everhealthsoftware.com/core/connect/token\nintrospection_endpoint:\
  \ https://drchrono-fhir.everhealthsoftware.com/core/connect/introspect\nrevocation_endpoint: https://drchrono-fhir.everhealthsoftware.com/core/connect/revocation\ngrant_types:\n- authorization_code\n- client_credentials\n- refresh_token\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\npkce:\n  supported: true\n  methods:\n  - S256\nscope_count: 233\nscope_contexts:\n- context: identity\n  count: 7\n  meaning: OpenID Connect / SMART identity and API-access scopes\n- context: user\n  count: 75\n  meaning: Access limited to what the authorizing user can see\n- context: patient\n  count: 75\n  meaning: Access limited to a single patient context\n- context: system\n  count: 75\n  meaning: Backend-services access, used with client_credentials and Bulk Data Export\n- context: launch\n  count: 1\n  meaning: ''\nscopes:\n- scope: openid\n  access: n/a\n- scope: profile\n  access: n/a\n- scope: IdentityScope\n  access: n/a\n- scope: fhirUser\n  access: n/a\n- scope: FHIRApi\n  access:\
  \ n/a\n- scope: user/AllergyIntolerance.read\n  access: read\n- scope: patient/AllergyIntolerance.read\n  access: read\n- scope: system/AllergyIntolerance.read\n  access: read\n- scope: user/Binary.read\n  access: read\n- scope: patient/Binary.read\n  access: read\n- scope: system/Binary.read\n  access: read\n- scope: user/CapabilityStatement.read\n  access: read\n- scope: patient/CapabilityStatement.read\n  access: read\n- scope: system/CapabilityStatement.read\n  access: read\n- scope: user/CarePlan.read\n  access: read\n- scope: patient/CarePlan.read\n  access: read\n- scope: system/CarePlan.read\n  access: read\n- scope: user/CareTeam.read\n  access: read\n- scope: patient/CareTeam.read\n  access: read\n- scope: system/CareTeam.read\n  access: read\n- scope: user/ClinicalImpression.read\n  access: read\n- scope: patient/ClinicalImpression.read\n  access: read\n- scope: system/ClinicalImpression.read\n  access: read\n- scope: user/Composition.read\n  access: read\n- scope: patient/Composition.read\n\
  \  access: read\n- scope: system/Composition.read\n  access: read\n- scope: user/Condition.read\n  access: read\n- scope: patient/Condition.read\n  access: read\n- scope: system/Condition.read\n  access: read\n- scope: user/Coverage.read\n  access: read\n- scope: patient/Coverage.read\n  access: read\n- scope: system/Coverage.read\n  access: read\n- scope: user/Device.read\n  access: read\n- scope: patient/Device.read\n  access: read\n- scope: system/Device.read\n  access: read\n- scope: user/DiagnosticReport.read\n  access: read\n- scope: patient/DiagnosticReport.read\n  access: read\n- scope: system/DiagnosticReport.read\n  access: read\n- scope: user/DocumentReference.read\n  access: read\n- scope: patient/DocumentReference.read\n  access: read\n- scope: system/DocumentReference.read\n  access: read\n- scope: user/Encounter.read\n  access: read\n- scope: patient/Encounter.read\n  access: read\n- scope: system/Encounter.read\n  access: read\n- scope: user/Goal.read\n  access: read\n\
  - scope: patient/Goal.read\n  access: read\n- scope: system/Goal.read\n  access: read\n- scope: user/Immunization.read\n  access: read\n- scope: patient/Immunization.read\n  access: read\n- scope: system/Immunization.read\n  access: read\n- scope: user/Location.read\n  access: read\n- scope: patient/Location.read\n  access: read\n- scope: system/Location.read\n  access: read\n- scope: user/Media.read\n  access: read\n- scope: patient/Media.read\n  access: read\n- scope: system/Media.read\n  access: read\n- scope: user/Medication.read\n  access: read\n- scope: patient/Medication.read\n  access: read\n- scope: system/Medication.read\n  access: read\n- scope: user/MedicationDispense.read\n  access: read\n- scope: patient/MedicationDispense.read\n  access: read\n- scope: system/MedicationDispense.read\n  access: read\n- scope: user/MedicationRequest.read\n  access: read\n- scope: patient/MedicationRequest.read\n  access: read\n- scope: system/MedicationRequest.read\n  access: read\n- scope:\
  \ user/MedicationStatement.read\n  access: read\n- scope: patient/MedicationStatement.read\n  access: read\n- scope: system/MedicationStatement.read\n  access: read\n- scope: user/Observation.read\n  access: read\n- scope: patient/Observation.read\n  access: read\n- scope: system/Observation.read\n  access: read\n- scope: user/Organization.read\n  access: read\n- scope: patient/Organization.read\n  access: read\n- scope: system/Organization.read\n  access: read\n- scope: user/Parameters.read\n  access: read\n- scope: patient/Parameters.read\n  access: read\n- scope: system/Parameters.read\n  access: read\n- scope: user/Patient.read\n  access: read\n- scope: patient/Patient.read\n  access: read\n- scope: system/Patient.read\n  access: read\n- scope: user/Person.read\n  access: read\n- scope: patient/Person.read\n  access: read\n- scope: system/Person.read\n  access: read\n- scope: user/Practitioner.read\n  access: read\n- scope: patient/Practitioner.read\n  access: read\n- scope: system/Practitioner.read\n\
  \  access: read\n- scope: user/PractitionerRole.read\n  access: read\n- scope: patient/PractitionerRole.read\n  access: read\n- scope: system/PractitionerRole.read\n  access: read\n- scope: user/Procedure.read\n  access: read\n- scope: patient/Procedure.read\n  access: read\n- scope: system/Procedure.read\n  access: read\n- scope: user/Provenance.read\n  access: read\n- scope: patient/Provenance.read\n  access: read\n- scope: system/Provenance.read\n  access: read\n- scope: user/RelatedPerson.read\n  access: read\n- scope: patient/RelatedPerson.read\n  access: read\n- scope: system/RelatedPerson.read\n  access: read\n- scope: user/ServiceRequest.read\n  access: read\n- scope: patient/ServiceRequest.read\n  access: read\n- scope: system/ServiceRequest.read\n  access: read\n- scope: user/Specimen.read\n  access: read\n- scope: patient/Specimen.read\n  access: read\n- scope: system/Specimen.read\n  access: read\n- scope: launch\n  access: n/a\n- scope: launch/patient\n  access: n/a\n- scope:\
  \ user/AllergyIntolerance.rs\n  access: n/a\n- scope: patient/AllergyIntolerance.rs\n  access: n/a\n- scope: system/AllergyIntolerance.rs\n  access: n/a\n- scope: user/Binary.rs\n  access: n/a\n- scope: patient/Binary.rs\n  access: n/a\n- scope: system/Binary.rs\n  access: n/a\n- scope: user/CapabilityStatement.rs\n  access: n/a\n- scope: patient/CapabilityStatement.rs\n  access: n/a\n- scope: system/CapabilityStatement.rs\n  access: n/a\n- scope: user/CarePlan.rs\n  access: n/a\n- scope: patient/CarePlan.rs\n  access: n/a\n- scope: system/CarePlan.rs\n  access: n/a\n- scope: user/CareTeam.rs\n  access: n/a\n- scope: patient/CareTeam.rs\n  access: n/a\n- scope: system/CareTeam.rs\n  access: n/a\n- scope: user/ClinicalImpression.rs\n  access: n/a\n- scope: patient/ClinicalImpression.rs\n  access: n/a\n- scope: system/ClinicalImpression.rs\n  access: n/a\n- scope: user/Composition.rs\n  access: n/a\n- scope: patient/Composition.rs\n  access: n/a\n- scope: system/Composition.rs\n  access:\
  \ n/a\n- scope: user/Condition.rs\n  access: n/a\n- scope: patient/Condition.rs\n  access: n/a\n- scope: system/Condition.rs\n  access: n/a\n- scope: user/Coverage.rs\n  access: n/a\n- scope: patient/Coverage.rs\n  access: n/a\n- scope: system/Coverage.rs\n  access: n/a\n- scope: user/Device.rs\n  access: n/a\n- scope: patient/Device.rs\n  access: n/a\n- scope: system/Device.rs\n  access: n/a\n- scope: user/DiagnosticReport.rs\n  access: n/a\n- scope: patient/DiagnosticReport.rs\n  access: n/a\n- scope: system/DiagnosticReport.rs\n  access: n/a\n- scope: user/DocumentReference.rs\n  access: n/a\n- scope: patient/DocumentReference.rs\n  access: n/a\n- scope: system/DocumentReference.rs\n  access: n/a\n- scope: user/Encounter.rs\n  access: n/a\n- scope: patient/Encounter.rs\n  access: n/a\n- scope: system/Encounter.rs\n  access: n/a\n- scope: user/Goal.rs\n  access: n/a\n- scope: patient/Goal.rs\n  access: n/a\n- scope: system/Goal.rs\n  access: n/a\n- scope: user/Immunization.rs\n  access:\
  \ n/a\n- scope: patient/Immunization.rs\n  access: n/a\n- scope: system/Immunization.rs\n  access: n/a\n- scope: user/Location.rs\n  access: n/a\n- scope: patient/Location.rs\n  access: n/a\n- scope: system/Location.rs\n  access: n/a\n- scope: user/Media.rs\n  access: n/a\n- scope: patient/Media.rs\n  access: n/a\n- scope: system/Media.rs\n  access: n/a\n- scope: user/Medication.rs\n  access: n/a\n- scope: patient/Medication.rs\n  access: n/a\n- scope: system/Medication.rs\n  access: n/a\n- scope: user/MedicationDispense.rs\n  access: n/a\n- scope: patient/MedicationDispense.rs\n  access: n/a\n- scope: system/MedicationDispense.rs\n  access: n/a\n- scope: user/MedicationRequest.rs\n  access: n/a\n- scope: patient/MedicationRequest.rs\n  access: n/a\n- scope: system/MedicationRequest.rs\n  access: n/a\n- scope: user/MedicationStatement.rs\n  access: n/a\n- scope: patient/MedicationStatement.rs\n  access: n/a\n- scope: system/MedicationStatement.rs\n  access: n/a\n- scope: user/Observation.rs\n\
  \  access: n/a\n- scope: patient/Observation.rs\n  access: n/a\n- scope: system/Observation.rs\n  access: n/a\n- scope: user/Organization.rs\n  access: n/a\n- scope: patient/Organization.rs\n  access: n/a\n- scope: system/Organization.rs\n  access: n/a\n- scope: user/Parameters.rs\n  access: n/a\n- scope: patient/Parameters.rs\n  access: n/a\n- scope: system/Parameters.rs\n  access: n/a\n- scope: user/Patient.rs\n  access: n/a\n- scope: patient/Patient.rs\n  access: n/a\n- scope: system/Patient.rs\n  access: n/a\n- scope: user/Person.rs\n  access: n/a\n- scope: patient/Person.rs\n  access: n/a\n- scope: system/Person.rs\n  access: n/a\n- scope: user/Practitioner.rs\n  access: n/a\n- scope: patient/Practitioner.rs\n  access: n/a\n- scope: system/Practitioner.rs\n  access: n/a\n- scope: user/PractitionerRole.rs\n  access: n/a\n- scope: patient/PractitionerRole.rs\n  access: n/a\n- scope: system/PractitionerRole.rs\n  access: n/a\n- scope: user/Procedure.rs\n  access: n/a\n- scope: patient/Procedure.rs\n\
  \  access: n/a\n- scope: system/Procedure.rs\n  access: n/a\n- scope: user/Provenance.rs\n  access: n/a\n- scope: patient/Provenance.rs\n  access: n/a\n- scope: system/Provenance.rs\n  access: n/a\n- scope: user/RelatedPerson.rs\n  access: n/a\n- scope: patient/RelatedPerson.rs\n  access: n/a\n- scope: system/RelatedPerson.rs\n  access: n/a\n- scope: user/ServiceRequest.rs\n  access: n/a\n- scope: patient/ServiceRequest.rs\n  access: n/a\n- scope: system/ServiceRequest.rs\n  access: n/a\n- scope: user/Specimen.rs\n  access: n/a\n- scope: patient/Specimen.rs\n  access: n/a\n- scope: system/Specimen.rs\n  access: n/a\n- scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  access: n/a\n- scope: patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  access: n/a\n- scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n\
  \  access: n/a\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  access: n/a\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  access: n/a\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n  access: n/a\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey\n  access: n/a\n- scope: patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  access: n/a\n- scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  access: n/a\n- scope: user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  access: n/a\n- scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n\
  \  access: n/a\n- scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  access: n/a\n- scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  access: n/a\n- scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n  access: n/a\n- scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey\n  access: n/a\n- scope: user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  access: n/a\n- scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  access: n/a\n- scope: system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  access: n/a\n- scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n\
  \  access: n/a\n- scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  access: n/a\n- scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  access: n/a\n- scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n  access: n/a\n- scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey\n  access: n/a\n- scope: system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  access: n/a\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure\n  access: n/a\n- scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure\n  access: n/a\n- scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure\n  access:\
  \ n/a\n- scope: offline_access\n  access: n/a\nnotes:\n- Every resource scope advertised is .read — consistent with the CapabilityStatement, which declares only read and\n  search-type interactions. The FHIR surface is read-only.\n- permission-v1 and permission-v2 are both advertised as SMART capabilities, so both the v1 (patient/Observation.read)\n  and v2 (patient/Observation.rs) scope syntaxes may be accepted; only the v1 form appears in scopes_supported.\n- Scope grants are provisioned at client registration by an EHR vendor admin, not by dynamic client registration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/scopes/drchrono-fhir-smart-scopes.yml
summary_line: 233 scopes
tags:
- EHR
- Electronic Health Records
- Healthcare
- Medical Records
- Practice Management
- HIPAA
- Appointments
- Billing
- Prescriptions
- Lab Integration
- FHIR
- SMART on FHIR
- USCDI
- Interoperability
- Webhooks
- OAuth 2.0
- ONC Certified
- Telehealth
- Revenue Cycle Management
token_urls: []
---
