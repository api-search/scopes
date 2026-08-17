---
authorization_urls: []
description: ''
docs: https://fhir.eclinicalworks.com/ecwopendev/documentation
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Eclinicalworks Scopes
name_suffix: OAuth Scopes
note: SMART on FHIR scope set read verbatim from the SMART configuration document served by the eClinicalWorks FHIR Facade. The identical 486-scope set is served on the healow patient-facing facade (https://fhir4.healow.com/fhir/r4/{practice_code}/.well-known/smart-configuration). Scope descriptions for the patient/user/system resource scopes are derived mechanically from the SMART v1/v2 scope grammar; the identity and launch-context descriptions are taken from the eClinicalWorks "Scopes Supported by eClinicalWorks" documentation page. Both SMART v1 (.read/.write) and SMART v2 (.rs/.c/.u/.d/.cruds) forms are advertised (capabilities include permission-v1 and permission-v2).
overview: 'eClinicalWorks publishes 486 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the eClinicalWorks API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: eClinicalWorks
provider_slug: eclinicalworks
schemes: []
scope_count: 486
scope_names:
- openid
- profile
- fhirUser
- patient/*.*
- user/*.*
- offline_access
- launch
- launch/patient
- patient/Medication.read
- patient/Medication.rs
- patient/Medication.c
- patient/Medication.u
- patient/AllergyIntolerance.read
- patient/AllergyIntolerance.rs
- patient/AllergyIntolerance.c
- patient/AllergyIntolerance.u
- patient/CarePlan.read
- patient/CarePlan.rs
- patient/CarePlan.c
- patient/CarePlan.u
- patient/CareTeam.read
- patient/CareTeam.rs
- patient/CareTeam.c
- patient/CareTeam.u
- patient/Condition.read
- patient/Condition.rs
- patient/Condition.c
- patient/Condition.u
- patient/Device.read
- patient/Device.rs
- patient/Device.c
- patient/Device.u
- patient/DiagnosticReport.read
- patient/DiagnosticReport.rs
- patient/DiagnosticReport.c
- patient/DiagnosticReport.u
- patient/DocumentReference.read
- patient/DocumentReference.rs
- patient/DocumentReference.c
- patient/DocumentReference.u
- patient/Encounter.read
- patient/Encounter.rs
- patient/Encounter.c
- patient/Encounter.u
- patient/Goal.read
- patient/Goal.rs
- patient/Goal.c
- patient/Goal.u
- patient/Immunization.read
- patient/Immunization.rs
- patient/Immunization.c
- patient/Immunization.u
- patient/Location.read
- patient/Location.rs
- patient/Location.c
- patient/Location.u
- patient/MedicationRequest.read
- patient/MedicationRequest.rs
- patient/MedicationRequest.c
- patient/MedicationRequest.u
- patient/MedicationAdministration.read
- patient/MedicationAdministration.rs
- patient/MedicationAdministration.c
- patient/MedicationAdministration.u
- patient/Observation.read
- patient/Observation.rs
- patient/Observation.c
- patient/Observation.u
- patient/Organization.read
- patient/Organization.rs
- patient/Organization.c
- patient/Organization.u
- patient/Patient.read
- patient/Patient.rs
- patient/Patient.c
- patient/Patient.u
- patient/Practitioner.read
- patient/Practitioner.rs
- patient/Practitioner.c
- patient/Practitioner.u
- patient/PractitionerRole.read
- patient/PractitionerRole.rs
- patient/PractitionerRole.c
- patient/PractitionerRole.u
- patient/Procedure.read
- patient/Procedure.rs
- patient/Procedure.c
- patient/Procedure.u
- patient/Provenance.read
- patient/Provenance.rs
- patient/Provenance.c
- patient/Provenance.u
- user/Medication.read
- user/Medication.rs
- user/Medication.c
- user/Medication.u
- user/AllergyIntolerance.read
- user/AllergyIntolerance.rs
- user/AllergyIntolerance.c
- user/AllergyIntolerance.u
- user/CarePlan.read
- user/CarePlan.rs
- user/CarePlan.c
- user/CarePlan.u
- user/CareTeam.read
- user/CareTeam.rs
- user/CareTeam.c
- user/CareTeam.u
- user/Condition.read
- user/Condition.rs
- user/Condition.c
- user/Condition.u
- user/Device.read
- user/Device.rs
- user/Device.c
- user/Device.u
- user/DiagnosticReport.read
- user/DiagnosticReport.rs
- user/DiagnosticReport.c
- user/DiagnosticReport.u
- user/DocumentReference.read
- user/DocumentReference.rs
- user/DocumentReference.c
- user/DocumentReference.u
- user/Encounter.read
- user/Encounter.rs
- user/Encounter.c
- user/Encounter.u
- user/Goal.read
- user/Goal.rs
- user/Goal.c
- user/Goal.u
- user/Immunization.read
- user/Immunization.rs
- user/Immunization.c
- user/Immunization.u
- user/Location.read
- user/Location.rs
- user/Location.c
- user/Location.u
- user/MedicationRequest.read
- user/MedicationRequest.rs
- user/MedicationRequest.c
- user/MedicationRequest.u
- user/MedicationAdministration.read
- user/MedicationAdministration.rs
- user/MedicationAdministration.c
- user/MedicationAdministration.u
- user/Observation.read
- user/Observation.rs
- user/Observation.c
- user/Observation.u
- user/Organization.read
- user/Organization.rs
- user/Organization.c
- user/Organization.u
- user/Patient.read
- user/Patient.rs
- user/Patient.c
- user/Patient.u
- user/Practitioner.read
- user/Practitioner.rs
- user/Practitioner.c
- user/Practitioner.u
- user/PractitionerRole.read
- user/PractitionerRole.rs
- user/PractitionerRole.c
- user/PractitionerRole.u
- user/Procedure.read
- user/Procedure.rs
- user/Procedure.c
- user/Procedure.u
- user/Provenance.read
- user/Provenance.rs
- user/Provenance.c
- user/Provenance.u
- system/Medication.read
- system/Medication.rs
- system/Medication.c
- system/Medication.u
- system/AllergyIntolerance.read
- system/AllergyIntolerance.rs
- system/AllergyIntolerance.c
- system/AllergyIntolerance.u
- system/CarePlan.read
- system/CarePlan.rs
- system/CarePlan.c
- system/CarePlan.u
- system/CareTeam.read
- system/CareTeam.rs
- system/CareTeam.c
- system/CareTeam.u
- system/Condition.read
- system/Condition.rs
- system/Condition.c
- system/Condition.u
- system/Device.read
- system/Device.rs
- system/Device.c
- system/Device.u
- system/DiagnosticReport.read
- system/DiagnosticReport.rs
- system/DiagnosticReport.c
- system/DiagnosticReport.u
- system/DocumentReference.read
- system/DocumentReference.rs
- system/DocumentReference.c
- system/DocumentReference.u
- system/Encounter.read
- system/Encounter.rs
- system/Encounter.c
- system/Encounter.u
- system/Goal.read
- system/Goal.rs
- system/Goal.c
- system/Goal.u
- system/Immunization.read
- system/Immunization.rs
- system/Immunization.c
- system/Immunization.u
- system/Location.read
- system/Location.rs
- system/Location.c
- system/Location.u
- system/MedicationRequest.read
- system/MedicationRequest.rs
- system/MedicationRequest.c
- system/MedicationRequest.u
- system/MedicationAdministration.read
- system/MedicationAdministration.rs
- system/MedicationAdministration.c
- system/MedicationAdministration.u
- system/Observation.read
- system/Observation.rs
- system/Observation.c
- system/Observation.u
- system/Organization.read
- system/Organization.rs
- system/Organization.c
- system/Organization.u
- system/Patient.read
- system/Patient.rs
- system/Patient.c
- system/Patient.u
- system/Practitioner.read
- system/Practitioner.rs
- system/Practitioner.c
- system/Practitioner.u
- system/PractitionerRole.read
- system/PractitionerRole.rs
- system/PractitionerRole.c
- system/PractitionerRole.u
- system/Procedure.read
- system/Procedure.rs
- system/Procedure.c
- system/Procedure.u
- system/Provenance.read
- system/Provenance.rs
- system/Provenance.c
- system/Provenance.u
- system/Group.read
- system/Group.rs
- system/Group.c
- system/Group.u
- patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- patient/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- user/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- system/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- patient/Patient.r
- user/Patient.r
- system/Patient.r
- patient/AllergyIntolerance.r
- user/AllergyIntolerance.r
- system/AllergyIntolerance.r
- patient/CarePlan.r
- user/CarePlan.r
- system/CarePlan.r
- patient/CareTeam.r
- user/CareTeam.r
- system/CareTeam.r
- patient/Media.r
- user/Media.r
- system/Media.r
- patient/MedicationDispense.r
- user/MedicationDispense.r
- system/MedicationDispense.r
- patient/Specimen.r
- user/Specimen.r
- system/Specimen.r
- patient/Condition.r
- user/Condition.r
- system/Condition.r
- patient/Device.r
- user/Device.r
- system/Device.r
- patient/DiagnosticReport.r
- user/DiagnosticReport.r
- system/DiagnosticReport.r
- patient/DocumentReference.r
- user/DocumentReference.r
- system/DocumentReference.r
- patient/Encounter.r
- user/Encounter.r
- system/Encounter.r
- patient/Goal.r
- user/Goal.r
- system/Goal.r
- patient/Immunization.r
- user/Immunization.r
- system/Immunization.r
- patient/Location.r
- user/Location.r
- system/Location.r
- patient/Medication.r
- user/Medication.r
- system/Medication.r
- patient/MedicationRequest.r
- user/MedicationRequest.r
- system/MedicationRequest.r
- patient/Observation.r
- user/Observation.r
- system/Observation.r
- system/Organization.r
- user/Organization.r
- patient/Organization.r
- patient/Practitioner.r
- user/Practitioner.r
- system/Practitioner.r
- patient/PractitionerRole.r
- user/PractitionerRole.r
- system/PractitionerRole.r
- patient/Procedure.r
- user/Procedure.r
- system/Procedure.r
- patient/Coverage.r
- user/Coverage.r
- system/Coverage.r
- patient/Claim.r
- user/Claim.r
- system/Claim.r
- patient/MedicationAdministration.r
- user/MedicationAdministration.r
- system/MedicationAdministration.r
- patient/Provenance.r
- user/Provenance.r
- system/Provenance.r
- patient/RelatedPerson.r
- user/RelatedPerson.r
- system/RelatedPerson.r
- patient/ServiceRequest.r
- user/ServiceRequest.r
- system/ServiceRequest.r
- patient/Endpoint.r
- user/Endpoint.r
- patient/Binary.r
- user/Binary.r
- system/Binary.r
- system/Group.r
- system/*.r
- user/*.r
- patient/*.r
- patient/QuestionnaireResponse.r
- user/QuestionnaireResponse.r
- system/QuestionnaireResponse.r
- patient/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- user/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- system/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- patient/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- user/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- system/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- patient/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- user/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- system/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- patient/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- user/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- system/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- patient/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- user/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- system/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- patient/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- user/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- system/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- patient/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- user/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- system/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- patient/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- user/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- system/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- patient/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- user/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- system/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- patient/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- user/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- system/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Organization.d
- user/Organization.d
- user/Coverage.d
- system/Coverage.d
- patient/Questionnaire.r
- patient/Questionnaire.read
- system/Questionnaire.c
- system/Questionnaire.u
- system/Questionnaire.r
- user/Questionnaire.r
- system/Questionnaire.read
- user/Questionnaire.read
- patient/Questionnaire.rs
- patient/Basic.read
- system/Basic.read
- user/Basic.read
- patient/Basic.r
- patient/Basic.read
- patient/Basic.rs
- patient/FamilyMemberHistory.r
- patient/FamilyMemberHistory.read
- patient/FamilyMemberHistory.rs
- system/FamilyMemberHistory.u
- system/FamilyMemberHistory.c
- patient/ChargeItem.rs
- system/ChargeItem.rs
- patient/ChargeItem.read
- system/ChargeItem.read
- system/ChargeItem.create
- user/ChargeItem.create
- system/ChargeItem.c
- user/ChargeItem.c
- user/ChargeItem.u
- system/ChargeItem.u
- user/ChargeItem.update
- system/ChargeItem.update
scopes:
- description: OpenID Connect authentication of the launching user.
  flows: []
  scope: openid
- description: Retrieve profile information about the current logged-in user.
  flows: []
  scope: profile
- description: Retrieve the FHIR resource representing the current logged-in user.
  flows: []
  scope: fhirUser
- description: All operations access to all FHIR resource types for the patient in context.
  flows: []
  scope: patient/*.*
- description: All operations access to all FHIR resource types for the authorized user.
  flows: []
  scope: user/*.*
- description: Request a refresh_token usable after the end user is no longer online (background refresh).
  flows: []
  scope: offline_access
- description: Obtain launch context when the app is launched from within the EHR (EHR Launch).
  flows: []
  scope: launch
- description: Request that a patient be selected at launch time (Standalone Launch).
  flows: []
  scope: launch/patient
- description: Read and search (SMART v1) access to Medication resources for the patient in context.
  flows: []
  scope: patient/Medication.read
- description: Read + search (SMART v2) access to Medication resources for the patient in context.
  flows: []
  scope: patient/Medication.rs
- description: Create access to Medication resources for the patient in context.
  flows: []
  scope: patient/Medication.c
- description: Update access to Medication resources for the patient in context.
  flows: []
  scope: patient/Medication.u
- description: Read and search (SMART v1) access to AllergyIntolerance resources for the patient in context.
  flows: []
  scope: patient/AllergyIntolerance.read
- description: Read + search (SMART v2) access to AllergyIntolerance resources for the patient in context.
  flows: []
  scope: patient/AllergyIntolerance.rs
- description: Create access to AllergyIntolerance resources for the patient in context.
  flows: []
  scope: patient/AllergyIntolerance.c
- description: Update access to AllergyIntolerance resources for the patient in context.
  flows: []
  scope: patient/AllergyIntolerance.u
- description: Read and search (SMART v1) access to CarePlan resources for the patient in context.
  flows: []
  scope: patient/CarePlan.read
- description: Read + search (SMART v2) access to CarePlan resources for the patient in context.
  flows: []
  scope: patient/CarePlan.rs
- description: Create access to CarePlan resources for the patient in context.
  flows: []
  scope: patient/CarePlan.c
- description: Update access to CarePlan resources for the patient in context.
  flows: []
  scope: patient/CarePlan.u
- description: Read and search (SMART v1) access to CareTeam resources for the patient in context.
  flows: []
  scope: patient/CareTeam.read
- description: Read + search (SMART v2) access to CareTeam resources for the patient in context.
  flows: []
  scope: patient/CareTeam.rs
- description: Create access to CareTeam resources for the patient in context.
  flows: []
  scope: patient/CareTeam.c
- description: Update access to CareTeam resources for the patient in context.
  flows: []
  scope: patient/CareTeam.u
- description: Read and search (SMART v1) access to Condition resources for the patient in context.
  flows: []
  scope: patient/Condition.read
- description: Read + search (SMART v2) access to Condition resources for the patient in context.
  flows: []
  scope: patient/Condition.rs
- description: Create access to Condition resources for the patient in context.
  flows: []
  scope: patient/Condition.c
- description: Update access to Condition resources for the patient in context.
  flows: []
  scope: patient/Condition.u
- description: Read and search (SMART v1) access to Device resources for the patient in context.
  flows: []
  scope: patient/Device.read
- description: Read + search (SMART v2) access to Device resources for the patient in context.
  flows: []
  scope: patient/Device.rs
- description: Create access to Device resources for the patient in context.
  flows: []
  scope: patient/Device.c
- description: Update access to Device resources for the patient in context.
  flows: []
  scope: patient/Device.u
- description: Read and search (SMART v1) access to DiagnosticReport resources for the patient in context.
  flows: []
  scope: patient/DiagnosticReport.read
- description: Read + search (SMART v2) access to DiagnosticReport resources for the patient in context.
  flows: []
  scope: patient/DiagnosticReport.rs
- description: Create access to DiagnosticReport resources for the patient in context.
  flows: []
  scope: patient/DiagnosticReport.c
- description: Update access to DiagnosticReport resources for the patient in context.
  flows: []
  scope: patient/DiagnosticReport.u
- description: Read and search (SMART v1) access to DocumentReference resources for the patient in context.
  flows: []
  scope: patient/DocumentReference.read
- description: Read + search (SMART v2) access to DocumentReference resources for the patient in context.
  flows: []
  scope: patient/DocumentReference.rs
- description: Create access to DocumentReference resources for the patient in context.
  flows: []
  scope: patient/DocumentReference.c
- description: Update access to DocumentReference resources for the patient in context.
  flows: []
  scope: patient/DocumentReference.u
- description: Read and search (SMART v1) access to Encounter resources for the patient in context.
  flows: []
  scope: patient/Encounter.read
- description: Read + search (SMART v2) access to Encounter resources for the patient in context.
  flows: []
  scope: patient/Encounter.rs
- description: Create access to Encounter resources for the patient in context.
  flows: []
  scope: patient/Encounter.c
- description: Update access to Encounter resources for the patient in context.
  flows: []
  scope: patient/Encounter.u
- description: Read and search (SMART v1) access to Goal resources for the patient in context.
  flows: []
  scope: patient/Goal.read
- description: Read + search (SMART v2) access to Goal resources for the patient in context.
  flows: []
  scope: patient/Goal.rs
- description: Create access to Goal resources for the patient in context.
  flows: []
  scope: patient/Goal.c
- description: Update access to Goal resources for the patient in context.
  flows: []
  scope: patient/Goal.u
- description: Read and search (SMART v1) access to Immunization resources for the patient in context.
  flows: []
  scope: patient/Immunization.read
- description: Read + search (SMART v2) access to Immunization resources for the patient in context.
  flows: []
  scope: patient/Immunization.rs
- description: Create access to Immunization resources for the patient in context.
  flows: []
  scope: patient/Immunization.c
- description: Update access to Immunization resources for the patient in context.
  flows: []
  scope: patient/Immunization.u
- description: Read and search (SMART v1) access to Location resources for the patient in context.
  flows: []
  scope: patient/Location.read
- description: Read + search (SMART v2) access to Location resources for the patient in context.
  flows: []
  scope: patient/Location.rs
- description: Create access to Location resources for the patient in context.
  flows: []
  scope: patient/Location.c
- description: Update access to Location resources for the patient in context.
  flows: []
  scope: patient/Location.u
- description: Read and search (SMART v1) access to MedicationRequest resources for the patient in context.
  flows: []
  scope: patient/MedicationRequest.read
- description: Read + search (SMART v2) access to MedicationRequest resources for the patient in context.
  flows: []
  scope: patient/MedicationRequest.rs
- description: Create access to MedicationRequest resources for the patient in context.
  flows: []
  scope: patient/MedicationRequest.c
- description: Update access to MedicationRequest resources for the patient in context.
  flows: []
  scope: patient/MedicationRequest.u
- description: Read and search (SMART v1) access to MedicationAdministration resources for the patient in context.
  flows: []
  scope: patient/MedicationAdministration.read
- description: Read + search (SMART v2) access to MedicationAdministration resources for the patient in context.
  flows: []
  scope: patient/MedicationAdministration.rs
- description: Create access to MedicationAdministration resources for the patient in context.
  flows: []
  scope: patient/MedicationAdministration.c
- description: Update access to MedicationAdministration resources for the patient in context.
  flows: []
  scope: patient/MedicationAdministration.u
- description: Read and search (SMART v1) access to Observation resources for the patient in context.
  flows: []
  scope: patient/Observation.read
- description: Read + search (SMART v2) access to Observation resources for the patient in context.
  flows: []
  scope: patient/Observation.rs
- description: Create access to Observation resources for the patient in context.
  flows: []
  scope: patient/Observation.c
- description: Update access to Observation resources for the patient in context.
  flows: []
  scope: patient/Observation.u
- description: Read and search (SMART v1) access to Organization resources for the patient in context.
  flows: []
  scope: patient/Organization.read
- description: Read + search (SMART v2) access to Organization resources for the patient in context.
  flows: []
  scope: patient/Organization.rs
- description: Create access to Organization resources for the patient in context.
  flows: []
  scope: patient/Organization.c
- description: Update access to Organization resources for the patient in context.
  flows: []
  scope: patient/Organization.u
- description: Read and search (SMART v1) access to Patient resources for the patient in context.
  flows: []
  scope: patient/Patient.read
- description: Read + search (SMART v2) access to Patient resources for the patient in context.
  flows: []
  scope: patient/Patient.rs
- description: Create access to Patient resources for the patient in context.
  flows: []
  scope: patient/Patient.c
- description: Update access to Patient resources for the patient in context.
  flows: []
  scope: patient/Patient.u
- description: Read and search (SMART v1) access to Practitioner resources for the patient in context.
  flows: []
  scope: patient/Practitioner.read
- description: Read + search (SMART v2) access to Practitioner resources for the patient in context.
  flows: []
  scope: patient/Practitioner.rs
- description: Create access to Practitioner resources for the patient in context.
  flows: []
  scope: patient/Practitioner.c
- description: Update access to Practitioner resources for the patient in context.
  flows: []
  scope: patient/Practitioner.u
- description: Read and search (SMART v1) access to PractitionerRole resources for the patient in context.
  flows: []
  scope: patient/PractitionerRole.read
- description: Read + search (SMART v2) access to PractitionerRole resources for the patient in context.
  flows: []
  scope: patient/PractitionerRole.rs
- description: Create access to PractitionerRole resources for the patient in context.
  flows: []
  scope: patient/PractitionerRole.c
- description: Update access to PractitionerRole resources for the patient in context.
  flows: []
  scope: patient/PractitionerRole.u
- description: Read and search (SMART v1) access to Procedure resources for the patient in context.
  flows: []
  scope: patient/Procedure.read
- description: Read + search (SMART v2) access to Procedure resources for the patient in context.
  flows: []
  scope: patient/Procedure.rs
- description: Create access to Procedure resources for the patient in context.
  flows: []
  scope: patient/Procedure.c
- description: Update access to Procedure resources for the patient in context.
  flows: []
  scope: patient/Procedure.u
- description: Read and search (SMART v1) access to Provenance resources for the patient in context.
  flows: []
  scope: patient/Provenance.read
- description: Read + search (SMART v2) access to Provenance resources for the patient in context.
  flows: []
  scope: patient/Provenance.rs
- description: Create access to Provenance resources for the patient in context.
  flows: []
  scope: patient/Provenance.c
- description: Update access to Provenance resources for the patient in context.
  flows: []
  scope: patient/Provenance.u
- description: Read and search (SMART v1) access to Medication resources for the authorized user.
  flows: []
  scope: user/Medication.read
- description: Read + search (SMART v2) access to Medication resources for the authorized user.
  flows: []
  scope: user/Medication.rs
- description: Create access to Medication resources for the authorized user.
  flows: []
  scope: user/Medication.c
- description: Update access to Medication resources for the authorized user.
  flows: []
  scope: user/Medication.u
- description: Read and search (SMART v1) access to AllergyIntolerance resources for the authorized user.
  flows: []
  scope: user/AllergyIntolerance.read
- description: Read + search (SMART v2) access to AllergyIntolerance resources for the authorized user.
  flows: []
  scope: user/AllergyIntolerance.rs
- description: Create access to AllergyIntolerance resources for the authorized user.
  flows: []
  scope: user/AllergyIntolerance.c
- description: Update access to AllergyIntolerance resources for the authorized user.
  flows: []
  scope: user/AllergyIntolerance.u
- description: Read and search (SMART v1) access to CarePlan resources for the authorized user.
  flows: []
  scope: user/CarePlan.read
- description: Read + search (SMART v2) access to CarePlan resources for the authorized user.
  flows: []
  scope: user/CarePlan.rs
- description: Create access to CarePlan resources for the authorized user.
  flows: []
  scope: user/CarePlan.c
- description: Update access to CarePlan resources for the authorized user.
  flows: []
  scope: user/CarePlan.u
- description: Read and search (SMART v1) access to CareTeam resources for the authorized user.
  flows: []
  scope: user/CareTeam.read
- description: Read + search (SMART v2) access to CareTeam resources for the authorized user.
  flows: []
  scope: user/CareTeam.rs
- description: Create access to CareTeam resources for the authorized user.
  flows: []
  scope: user/CareTeam.c
- description: Update access to CareTeam resources for the authorized user.
  flows: []
  scope: user/CareTeam.u
- description: Read and search (SMART v1) access to Condition resources for the authorized user.
  flows: []
  scope: user/Condition.read
- description: Read + search (SMART v2) access to Condition resources for the authorized user.
  flows: []
  scope: user/Condition.rs
- description: Create access to Condition resources for the authorized user.
  flows: []
  scope: user/Condition.c
- description: Update access to Condition resources for the authorized user.
  flows: []
  scope: user/Condition.u
- description: Read and search (SMART v1) access to Device resources for the authorized user.
  flows: []
  scope: user/Device.read
- description: Read + search (SMART v2) access to Device resources for the authorized user.
  flows: []
  scope: user/Device.rs
- description: Create access to Device resources for the authorized user.
  flows: []
  scope: user/Device.c
- description: Update access to Device resources for the authorized user.
  flows: []
  scope: user/Device.u
- description: Read and search (SMART v1) access to DiagnosticReport resources for the authorized user.
  flows: []
  scope: user/DiagnosticReport.read
- description: Read + search (SMART v2) access to DiagnosticReport resources for the authorized user.
  flows: []
  scope: user/DiagnosticReport.rs
- description: Create access to DiagnosticReport resources for the authorized user.
  flows: []
  scope: user/DiagnosticReport.c
- description: Update access to DiagnosticReport resources for the authorized user.
  flows: []
  scope: user/DiagnosticReport.u
- description: Read and search (SMART v1) access to DocumentReference resources for the authorized user.
  flows: []
  scope: user/DocumentReference.read
- description: Read + search (SMART v2) access to DocumentReference resources for the authorized user.
  flows: []
  scope: user/DocumentReference.rs
- description: Create access to DocumentReference resources for the authorized user.
  flows: []
  scope: user/DocumentReference.c
- description: Update access to DocumentReference resources for the authorized user.
  flows: []
  scope: user/DocumentReference.u
- description: Read and search (SMART v1) access to Encounter resources for the authorized user.
  flows: []
  scope: user/Encounter.read
- description: Read + search (SMART v2) access to Encounter resources for the authorized user.
  flows: []
  scope: user/Encounter.rs
- description: Create access to Encounter resources for the authorized user.
  flows: []
  scope: user/Encounter.c
- description: Update access to Encounter resources for the authorized user.
  flows: []
  scope: user/Encounter.u
- description: Read and search (SMART v1) access to Goal resources for the authorized user.
  flows: []
  scope: user/Goal.read
- description: Read + search (SMART v2) access to Goal resources for the authorized user.
  flows: []
  scope: user/Goal.rs
- description: Create access to Goal resources for the authorized user.
  flows: []
  scope: user/Goal.c
- description: Update access to Goal resources for the authorized user.
  flows: []
  scope: user/Goal.u
- description: Read and search (SMART v1) access to Immunization resources for the authorized user.
  flows: []
  scope: user/Immunization.read
- description: Read + search (SMART v2) access to Immunization resources for the authorized user.
  flows: []
  scope: user/Immunization.rs
- description: Create access to Immunization resources for the authorized user.
  flows: []
  scope: user/Immunization.c
- description: Update access to Immunization resources for the authorized user.
  flows: []
  scope: user/Immunization.u
- description: Read and search (SMART v1) access to Location resources for the authorized user.
  flows: []
  scope: user/Location.read
- description: Read + search (SMART v2) access to Location resources for the authorized user.
  flows: []
  scope: user/Location.rs
- description: Create access to Location resources for the authorized user.
  flows: []
  scope: user/Location.c
- description: Update access to Location resources for the authorized user.
  flows: []
  scope: user/Location.u
- description: Read and search (SMART v1) access to MedicationRequest resources for the authorized user.
  flows: []
  scope: user/MedicationRequest.read
- description: Read + search (SMART v2) access to MedicationRequest resources for the authorized user.
  flows: []
  scope: user/MedicationRequest.rs
- description: Create access to MedicationRequest resources for the authorized user.
  flows: []
  scope: user/MedicationRequest.c
- description: Update access to MedicationRequest resources for the authorized user.
  flows: []
  scope: user/MedicationRequest.u
- description: Read and search (SMART v1) access to MedicationAdministration resources for the authorized user.
  flows: []
  scope: user/MedicationAdministration.read
- description: Read + search (SMART v2) access to MedicationAdministration resources for the authorized user.
  flows: []
  scope: user/MedicationAdministration.rs
- description: Create access to MedicationAdministration resources for the authorized user.
  flows: []
  scope: user/MedicationAdministration.c
- description: Update access to MedicationAdministration resources for the authorized user.
  flows: []
  scope: user/MedicationAdministration.u
- description: Read and search (SMART v1) access to Observation resources for the authorized user.
  flows: []
  scope: user/Observation.read
- description: Read + search (SMART v2) access to Observation resources for the authorized user.
  flows: []
  scope: user/Observation.rs
- description: Create access to Observation resources for the authorized user.
  flows: []
  scope: user/Observation.c
- description: Update access to Observation resources for the authorized user.
  flows: []
  scope: user/Observation.u
- description: Read and search (SMART v1) access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.read
- description: Read + search (SMART v2) access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.rs
- description: Create access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.c
- description: Update access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.u
- description: Read and search (SMART v1) access to Patient resources for the authorized user.
  flows: []
  scope: user/Patient.read
- description: Read + search (SMART v2) access to Patient resources for the authorized user.
  flows: []
  scope: user/Patient.rs
- description: Create access to Patient resources for the authorized user.
  flows: []
  scope: user/Patient.c
- description: Update access to Patient resources for the authorized user.
  flows: []
  scope: user/Patient.u
- description: Read and search (SMART v1) access to Practitioner resources for the authorized user.
  flows: []
  scope: user/Practitioner.read
- description: Read + search (SMART v2) access to Practitioner resources for the authorized user.
  flows: []
  scope: user/Practitioner.rs
- description: Create access to Practitioner resources for the authorized user.
  flows: []
  scope: user/Practitioner.c
- description: Update access to Practitioner resources for the authorized user.
  flows: []
  scope: user/Practitioner.u
- description: Read and search (SMART v1) access to PractitionerRole resources for the authorized user.
  flows: []
  scope: user/PractitionerRole.read
- description: Read + search (SMART v2) access to PractitionerRole resources for the authorized user.
  flows: []
  scope: user/PractitionerRole.rs
- description: Create access to PractitionerRole resources for the authorized user.
  flows: []
  scope: user/PractitionerRole.c
- description: Update access to PractitionerRole resources for the authorized user.
  flows: []
  scope: user/PractitionerRole.u
- description: Read and search (SMART v1) access to Procedure resources for the authorized user.
  flows: []
  scope: user/Procedure.read
- description: Read + search (SMART v2) access to Procedure resources for the authorized user.
  flows: []
  scope: user/Procedure.rs
- description: Create access to Procedure resources for the authorized user.
  flows: []
  scope: user/Procedure.c
- description: Update access to Procedure resources for the authorized user.
  flows: []
  scope: user/Procedure.u
- description: Read and search (SMART v1) access to Provenance resources for the authorized user.
  flows: []
  scope: user/Provenance.read
- description: Read + search (SMART v2) access to Provenance resources for the authorized user.
  flows: []
  scope: user/Provenance.rs
- description: Create access to Provenance resources for the authorized user.
  flows: []
  scope: user/Provenance.c
- description: Update access to Provenance resources for the authorized user.
  flows: []
  scope: user/Provenance.u
- description: Read and search (SMART v1) access to Medication resources for the backend system (no user).
  flows: []
  scope: system/Medication.read
- description: Read + search (SMART v2) access to Medication resources for the backend system (no user).
  flows: []
  scope: system/Medication.rs
- description: Create access to Medication resources for the backend system (no user).
  flows: []
  scope: system/Medication.c
- description: Update access to Medication resources for the backend system (no user).
  flows: []
  scope: system/Medication.u
- description: Read and search (SMART v1) access to AllergyIntolerance resources for the backend system (no user).
  flows: []
  scope: system/AllergyIntolerance.read
- description: Read + search (SMART v2) access to AllergyIntolerance resources for the backend system (no user).
  flows: []
  scope: system/AllergyIntolerance.rs
- description: Create access to AllergyIntolerance resources for the backend system (no user).
  flows: []
  scope: system/AllergyIntolerance.c
- description: Update access to AllergyIntolerance resources for the backend system (no user).
  flows: []
  scope: system/AllergyIntolerance.u
- description: Read and search (SMART v1) access to CarePlan resources for the backend system (no user).
  flows: []
  scope: system/CarePlan.read
- description: Read + search (SMART v2) access to CarePlan resources for the backend system (no user).
  flows: []
  scope: system/CarePlan.rs
- description: Create access to CarePlan resources for the backend system (no user).
  flows: []
  scope: system/CarePlan.c
- description: Update access to CarePlan resources for the backend system (no user).
  flows: []
  scope: system/CarePlan.u
- description: Read and search (SMART v1) access to CareTeam resources for the backend system (no user).
  flows: []
  scope: system/CareTeam.read
- description: Read + search (SMART v2) access to CareTeam resources for the backend system (no user).
  flows: []
  scope: system/CareTeam.rs
- description: Create access to CareTeam resources for the backend system (no user).
  flows: []
  scope: system/CareTeam.c
- description: Update access to CareTeam resources for the backend system (no user).
  flows: []
  scope: system/CareTeam.u
- description: Read and search (SMART v1) access to Condition resources for the backend system (no user).
  flows: []
  scope: system/Condition.read
- description: Read + search (SMART v2) access to Condition resources for the backend system (no user).
  flows: []
  scope: system/Condition.rs
- description: Create access to Condition resources for the backend system (no user).
  flows: []
  scope: system/Condition.c
- description: Update access to Condition resources for the backend system (no user).
  flows: []
  scope: system/Condition.u
- description: Read and search (SMART v1) access to Device resources for the backend system (no user).
  flows: []
  scope: system/Device.read
- description: Read + search (SMART v2) access to Device resources for the backend system (no user).
  flows: []
  scope: system/Device.rs
- description: Create access to Device resources for the backend system (no user).
  flows: []
  scope: system/Device.c
- description: Update access to Device resources for the backend system (no user).
  flows: []
  scope: system/Device.u
- description: Read and search (SMART v1) access to DiagnosticReport resources for the backend system (no user).
  flows: []
  scope: system/DiagnosticReport.read
- description: Read + search (SMART v2) access to DiagnosticReport resources for the backend system (no user).
  flows: []
  scope: system/DiagnosticReport.rs
- description: Create access to DiagnosticReport resources for the backend system (no user).
  flows: []
  scope: system/DiagnosticReport.c
- description: Update access to DiagnosticReport resources for the backend system (no user).
  flows: []
  scope: system/DiagnosticReport.u
- description: Read and search (SMART v1) access to DocumentReference resources for the backend system (no user).
  flows: []
  scope: system/DocumentReference.read
- description: Read + search (SMART v2) access to DocumentReference resources for the backend system (no user).
  flows: []
  scope: system/DocumentReference.rs
- description: Create access to DocumentReference resources for the backend system (no user).
  flows: []
  scope: system/DocumentReference.c
- description: Update access to DocumentReference resources for the backend system (no user).
  flows: []
  scope: system/DocumentReference.u
- description: Read and search (SMART v1) access to Encounter resources for the backend system (no user).
  flows: []
  scope: system/Encounter.read
- description: Read + search (SMART v2) access to Encounter resources for the backend system (no user).
  flows: []
  scope: system/Encounter.rs
- description: Create access to Encounter resources for the backend system (no user).
  flows: []
  scope: system/Encounter.c
- description: Update access to Encounter resources for the backend system (no user).
  flows: []
  scope: system/Encounter.u
- description: Read and search (SMART v1) access to Goal resources for the backend system (no user).
  flows: []
  scope: system/Goal.read
- description: Read + search (SMART v2) access to Goal resources for the backend system (no user).
  flows: []
  scope: system/Goal.rs
- description: Create access to Goal resources for the backend system (no user).
  flows: []
  scope: system/Goal.c
- description: Update access to Goal resources for the backend system (no user).
  flows: []
  scope: system/Goal.u
- description: Read and search (SMART v1) access to Immunization resources for the backend system (no user).
  flows: []
  scope: system/Immunization.read
- description: Read + search (SMART v2) access to Immunization resources for the backend system (no user).
  flows: []
  scope: system/Immunization.rs
- description: Create access to Immunization resources for the backend system (no user).
  flows: []
  scope: system/Immunization.c
- description: Update access to Immunization resources for the backend system (no user).
  flows: []
  scope: system/Immunization.u
- description: Read and search (SMART v1) access to Location resources for the backend system (no user).
  flows: []
  scope: system/Location.read
- description: Read + search (SMART v2) access to Location resources for the backend system (no user).
  flows: []
  scope: system/Location.rs
- description: Create access to Location resources for the backend system (no user).
  flows: []
  scope: system/Location.c
- description: Update access to Location resources for the backend system (no user).
  flows: []
  scope: system/Location.u
- description: Read and search (SMART v1) access to MedicationRequest resources for the backend system (no user).
  flows: []
  scope: system/MedicationRequest.read
- description: Read + search (SMART v2) access to MedicationRequest resources for the backend system (no user).
  flows: []
  scope: system/MedicationRequest.rs
- description: Create access to MedicationRequest resources for the backend system (no user).
  flows: []
  scope: system/MedicationRequest.c
- description: Update access to MedicationRequest resources for the backend system (no user).
  flows: []
  scope: system/MedicationRequest.u
- description: Read and search (SMART v1) access to MedicationAdministration resources for the backend system (no user).
  flows: []
  scope: system/MedicationAdministration.read
- description: Read + search (SMART v2) access to MedicationAdministration resources for the backend system (no user).
  flows: []
  scope: system/MedicationAdministration.rs
- description: Create access to MedicationAdministration resources for the backend system (no user).
  flows: []
  scope: system/MedicationAdministration.c
- description: Update access to MedicationAdministration resources for the backend system (no user).
  flows: []
  scope: system/MedicationAdministration.u
- description: Read and search (SMART v1) access to Observation resources for the backend system (no user).
  flows: []
  scope: system/Observation.read
- description: Read + search (SMART v2) access to Observation resources for the backend system (no user).
  flows: []
  scope: system/Observation.rs
- description: Create access to Observation resources for the backend system (no user).
  flows: []
  scope: system/Observation.c
- description: Update access to Observation resources for the backend system (no user).
  flows: []
  scope: system/Observation.u
- description: Read and search (SMART v1) access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.read
- description: Read + search (SMART v2) access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.rs
- description: Create access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.c
- description: Update access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.u
- description: Read and search (SMART v1) access to Patient resources for the backend system (no user).
  flows: []
  scope: system/Patient.read
- description: Read + search (SMART v2) access to Patient resources for the backend system (no user).
  flows: []
  scope: system/Patient.rs
- description: Create access to Patient resources for the backend system (no user).
  flows: []
  scope: system/Patient.c
- description: Update access to Patient resources for the backend system (no user).
  flows: []
  scope: system/Patient.u
- description: Read and search (SMART v1) access to Practitioner resources for the backend system (no user).
  flows: []
  scope: system/Practitioner.read
- description: Read + search (SMART v2) access to Practitioner resources for the backend system (no user).
  flows: []
  scope: system/Practitioner.rs
- description: Create access to Practitioner resources for the backend system (no user).
  flows: []
  scope: system/Practitioner.c
- description: Update access to Practitioner resources for the backend system (no user).
  flows: []
  scope: system/Practitioner.u
- description: Read and search (SMART v1) access to PractitionerRole resources for the backend system (no user).
  flows: []
  scope: system/PractitionerRole.read
- description: Read + search (SMART v2) access to PractitionerRole resources for the backend system (no user).
  flows: []
  scope: system/PractitionerRole.rs
- description: Create access to PractitionerRole resources for the backend system (no user).
  flows: []
  scope: system/PractitionerRole.c
- description: Update access to PractitionerRole resources for the backend system (no user).
  flows: []
  scope: system/PractitionerRole.u
- description: Read and search (SMART v1) access to Procedure resources for the backend system (no user).
  flows: []
  scope: system/Procedure.read
- description: Read + search (SMART v2) access to Procedure resources for the backend system (no user).
  flows: []
  scope: system/Procedure.rs
- description: Create access to Procedure resources for the backend system (no user).
  flows: []
  scope: system/Procedure.c
- description: Update access to Procedure resources for the backend system (no user).
  flows: []
  scope: system/Procedure.u
- description: Read and search (SMART v1) access to Provenance resources for the backend system (no user).
  flows: []
  scope: system/Provenance.read
- description: Read + search (SMART v2) access to Provenance resources for the backend system (no user).
  flows: []
  scope: system/Provenance.rs
- description: Create access to Provenance resources for the backend system (no user).
  flows: []
  scope: system/Provenance.c
- description: Update access to Provenance resources for the backend system (no user).
  flows: []
  scope: system/Provenance.u
- description: Read and search (SMART v1) access to Group resources for the backend system (no user).
  flows: []
  scope: system/Group.read
- description: Read + search (SMART v2) access to Group resources for the backend system (no user).
  flows: []
  scope: system/Group.rs
- description: Create access to Group resources for the backend system (no user).
  flows: []
  scope: system/Group.c
- description: Update access to Group resources for the backend system (no user).
  flows: []
  scope: system/Group.u
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: r access to Patient resources for the patient in context.
  flows: []
  scope: patient/Patient.r
- description: r access to Patient resources for the authorized user.
  flows: []
  scope: user/Patient.r
- description: r access to Patient resources for the backend system (no user).
  flows: []
  scope: system/Patient.r
- description: r access to AllergyIntolerance resources for the patient in context.
  flows: []
  scope: patient/AllergyIntolerance.r
- description: r access to AllergyIntolerance resources for the authorized user.
  flows: []
  scope: user/AllergyIntolerance.r
- description: r access to AllergyIntolerance resources for the backend system (no user).
  flows: []
  scope: system/AllergyIntolerance.r
- description: r access to CarePlan resources for the patient in context.
  flows: []
  scope: patient/CarePlan.r
- description: r access to CarePlan resources for the authorized user.
  flows: []
  scope: user/CarePlan.r
- description: r access to CarePlan resources for the backend system (no user).
  flows: []
  scope: system/CarePlan.r
- description: r access to CareTeam resources for the patient in context.
  flows: []
  scope: patient/CareTeam.r
- description: r access to CareTeam resources for the authorized user.
  flows: []
  scope: user/CareTeam.r
- description: r access to CareTeam resources for the backend system (no user).
  flows: []
  scope: system/CareTeam.r
- description: r access to Media resources for the patient in context.
  flows: []
  scope: patient/Media.r
- description: r access to Media resources for the authorized user.
  flows: []
  scope: user/Media.r
- description: r access to Media resources for the backend system (no user).
  flows: []
  scope: system/Media.r
- description: r access to MedicationDispense resources for the patient in context.
  flows: []
  scope: patient/MedicationDispense.r
- description: r access to MedicationDispense resources for the authorized user.
  flows: []
  scope: user/MedicationDispense.r
- description: r access to MedicationDispense resources for the backend system (no user).
  flows: []
  scope: system/MedicationDispense.r
- description: r access to Specimen resources for the patient in context.
  flows: []
  scope: patient/Specimen.r
- description: r access to Specimen resources for the authorized user.
  flows: []
  scope: user/Specimen.r
- description: r access to Specimen resources for the backend system (no user).
  flows: []
  scope: system/Specimen.r
- description: r access to Condition resources for the patient in context.
  flows: []
  scope: patient/Condition.r
- description: r access to Condition resources for the authorized user.
  flows: []
  scope: user/Condition.r
- description: r access to Condition resources for the backend system (no user).
  flows: []
  scope: system/Condition.r
- description: r access to Device resources for the patient in context.
  flows: []
  scope: patient/Device.r
- description: r access to Device resources for the authorized user.
  flows: []
  scope: user/Device.r
- description: r access to Device resources for the backend system (no user).
  flows: []
  scope: system/Device.r
- description: r access to DiagnosticReport resources for the patient in context.
  flows: []
  scope: patient/DiagnosticReport.r
- description: r access to DiagnosticReport resources for the authorized user.
  flows: []
  scope: user/DiagnosticReport.r
- description: r access to DiagnosticReport resources for the backend system (no user).
  flows: []
  scope: system/DiagnosticReport.r
- description: r access to DocumentReference resources for the patient in context.
  flows: []
  scope: patient/DocumentReference.r
- description: r access to DocumentReference resources for the authorized user.
  flows: []
  scope: user/DocumentReference.r
- description: r access to DocumentReference resources for the backend system (no user).
  flows: []
  scope: system/DocumentReference.r
- description: r access to Encounter resources for the patient in context.
  flows: []
  scope: patient/Encounter.r
- description: r access to Encounter resources for the authorized user.
  flows: []
  scope: user/Encounter.r
- description: r access to Encounter resources for the backend system (no user).
  flows: []
  scope: system/Encounter.r
- description: r access to Goal resources for the patient in context.
  flows: []
  scope: patient/Goal.r
- description: r access to Goal resources for the authorized user.
  flows: []
  scope: user/Goal.r
- description: r access to Goal resources for the backend system (no user).
  flows: []
  scope: system/Goal.r
- description: r access to Immunization resources for the patient in context.
  flows: []
  scope: patient/Immunization.r
- description: r access to Immunization resources for the authorized user.
  flows: []
  scope: user/Immunization.r
- description: r access to Immunization resources for the backend system (no user).
  flows: []
  scope: system/Immunization.r
- description: r access to Location resources for the patient in context.
  flows: []
  scope: patient/Location.r
- description: r access to Location resources for the authorized user.
  flows: []
  scope: user/Location.r
- description: r access to Location resources for the backend system (no user).
  flows: []
  scope: system/Location.r
- description: r access to Medication resources for the patient in context.
  flows: []
  scope: patient/Medication.r
- description: r access to Medication resources for the authorized user.
  flows: []
  scope: user/Medication.r
- description: r access to Medication resources for the backend system (no user).
  flows: []
  scope: system/Medication.r
- description: r access to MedicationRequest resources for the patient in context.
  flows: []
  scope: patient/MedicationRequest.r
- description: r access to MedicationRequest resources for the authorized user.
  flows: []
  scope: user/MedicationRequest.r
- description: r access to MedicationRequest resources for the backend system (no user).
  flows: []
  scope: system/MedicationRequest.r
- description: r access to Observation resources for the patient in context.
  flows: []
  scope: patient/Observation.r
- description: r access to Observation resources for the authorized user.
  flows: []
  scope: user/Observation.r
- description: r access to Observation resources for the backend system (no user).
  flows: []
  scope: system/Observation.r
- description: r access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.r
- description: r access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.r
- description: r access to Organization resources for the patient in context.
  flows: []
  scope: patient/Organization.r
- description: r access to Practitioner resources for the patient in context.
  flows: []
  scope: patient/Practitioner.r
- description: r access to Practitioner resources for the authorized user.
  flows: []
  scope: user/Practitioner.r
- description: r access to Practitioner resources for the backend system (no user).
  flows: []
  scope: system/Practitioner.r
- description: r access to PractitionerRole resources for the patient in context.
  flows: []
  scope: patient/PractitionerRole.r
- description: r access to PractitionerRole resources for the authorized user.
  flows: []
  scope: user/PractitionerRole.r
- description: r access to PractitionerRole resources for the backend system (no user).
  flows: []
  scope: system/PractitionerRole.r
- description: r access to Procedure resources for the patient in context.
  flows: []
  scope: patient/Procedure.r
- description: r access to Procedure resources for the authorized user.
  flows: []
  scope: user/Procedure.r
- description: r access to Procedure resources for the backend system (no user).
  flows: []
  scope: system/Procedure.r
- description: r access to Coverage resources for the patient in context.
  flows: []
  scope: patient/Coverage.r
- description: r access to Coverage resources for the authorized user.
  flows: []
  scope: user/Coverage.r
- description: r access to Coverage resources for the backend system (no user).
  flows: []
  scope: system/Coverage.r
- description: r access to Claim resources for the patient in context.
  flows: []
  scope: patient/Claim.r
- description: r access to Claim resources for the authorized user.
  flows: []
  scope: user/Claim.r
- description: r access to Claim resources for the backend system (no user).
  flows: []
  scope: system/Claim.r
- description: r access to MedicationAdministration resources for the patient in context.
  flows: []
  scope: patient/MedicationAdministration.r
- description: r access to MedicationAdministration resources for the authorized user.
  flows: []
  scope: user/MedicationAdministration.r
- description: r access to MedicationAdministration resources for the backend system (no user).
  flows: []
  scope: system/MedicationAdministration.r
- description: r access to Provenance resources for the patient in context.
  flows: []
  scope: patient/Provenance.r
- description: r access to Provenance resources for the authorized user.
  flows: []
  scope: user/Provenance.r
- description: r access to Provenance resources for the backend system (no user).
  flows: []
  scope: system/Provenance.r
- description: r access to RelatedPerson resources for the patient in context.
  flows: []
  scope: patient/RelatedPerson.r
- description: r access to RelatedPerson resources for the authorized user.
  flows: []
  scope: user/RelatedPerson.r
- description: r access to RelatedPerson resources for the backend system (no user).
  flows: []
  scope: system/RelatedPerson.r
- description: r access to ServiceRequest resources for the patient in context.
  flows: []
  scope: patient/ServiceRequest.r
- description: r access to ServiceRequest resources for the authorized user.
  flows: []
  scope: user/ServiceRequest.r
- description: r access to ServiceRequest resources for the backend system (no user).
  flows: []
  scope: system/ServiceRequest.r
- description: r access to Endpoint resources for the patient in context.
  flows: []
  scope: patient/Endpoint.r
- description: r access to Endpoint resources for the authorized user.
  flows: []
  scope: user/Endpoint.r
- description: r access to Binary resources for the patient in context.
  flows: []
  scope: patient/Binary.r
- description: r access to Binary resources for the authorized user.
  flows: []
  scope: user/Binary.r
- description: r access to Binary resources for the backend system (no user).
  flows: []
  scope: system/Binary.r
- description: r access to Group resources for the backend system (no user).
  flows: []
  scope: system/Group.r
- description: r access to all FHIR resource types for the backend system (no user).
  flows: []
  scope: system/*.r
- description: r access to all FHIR resource types for the authorized user.
  flows: []
  scope: user/*.r
- description: r access to all FHIR resource types for the patient in context.
  flows: []
  scope: patient/*.r
- description: r access to QuestionnaireResponse resources for the patient in context.
  flows: []
  scope: patient/QuestionnaireResponse.r
- description: r access to QuestionnaireResponse resources for the authorized user.
  flows: []
  scope: user/QuestionnaireResponse.r
- description: r access to QuestionnaireResponse resources for the backend system (no user).
  flows: []
  scope: system/QuestionnaireResponse.r
- description: ''
  flows: []
  scope: patient/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: user/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: system/Condition.r?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: patient/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: user/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: system/Condition.read?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: ''
  flows: []
  scope: patient/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: user/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: system/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: patient/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: user/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: system/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: ''
  flows: []
  scope: patient/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: user/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: system/Condition.r?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: patient/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: user/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: system/Condition.read?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: user/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: system/Observation.r?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: patient/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: user/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: system/Observation.r?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: user/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: system/Observation.read?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org//CodeSystem-observation-category|social-history
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|exam
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging
- description: ''
  flows: []
  scope: patient/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: user/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: ''
  flows: []
  scope: system/Observation.read?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: Delete access to Organization resources for the backend system (no user).
  flows: []
  scope: system/Organization.d
- description: Delete access to Organization resources for the authorized user.
  flows: []
  scope: user/Organization.d
- description: Delete access to Coverage resources for the authorized user.
  flows: []
  scope: user/Coverage.d
- description: Delete access to Coverage resources for the backend system (no user).
  flows: []
  scope: system/Coverage.d
- description: r access to Questionnaire resources for the patient in context.
  flows: []
  scope: patient/Questionnaire.r
- description: Read and search (SMART v1) access to Questionnaire resources for the patient in context.
  flows: []
  scope: patient/Questionnaire.read
- description: Create access to Questionnaire resources for the backend system (no user).
  flows: []
  scope: system/Questionnaire.c
- description: Update access to Questionnaire resources for the backend system (no user).
  flows: []
  scope: system/Questionnaire.u
- description: r access to Questionnaire resources for the backend system (no user).
  flows: []
  scope: system/Questionnaire.r
- description: r access to Questionnaire resources for the authorized user.
  flows: []
  scope: user/Questionnaire.r
- description: Read and search (SMART v1) access to Questionnaire resources for the backend system (no user).
  flows: []
  scope: system/Questionnaire.read
- description: Read and search (SMART v1) access to Questionnaire resources for the authorized user.
  flows: []
  scope: user/Questionnaire.read
- description: Read + search (SMART v2) access to Questionnaire resources for the patient in context.
  flows: []
  scope: patient/Questionnaire.rs
- description: Read and search (SMART v1) access to Basic resources for the patient in context.
  flows: []
  scope: patient/Basic.read
- description: Read and search (SMART v1) access to Basic resources for the backend system (no user).
  flows: []
  scope: system/Basic.read
- description: Read and search (SMART v1) access to Basic resources for the authorized user.
  flows: []
  scope: user/Basic.read
- description: r access to Basic resources for the patient in context.
  flows: []
  scope: patient/Basic.r
- description: Read and search (SMART v1) access to Basic resources for the patient in context.
  flows: []
  scope: patient/Basic.read
- description: Read + search (SMART v2) access to Basic resources for the patient in context.
  flows: []
  scope: patient/Basic.rs
- description: r access to FamilyMemberHistory resources for the patient in context.
  flows: []
  scope: patient/FamilyMemberHistory.r
- description: Read and search (SMART v1) access to FamilyMemberHistory resources for the patient in context.
  flows: []
  scope: patient/FamilyMemberHistory.read
- description: Read + search (SMART v2) access to FamilyMemberHistory resources for the patient in context.
  flows: []
  scope: patient/FamilyMemberHistory.rs
- description: Update access to FamilyMemberHistory resources for the backend system (no user).
  flows: []
  scope: system/FamilyMemberHistory.u
- description: Create access to FamilyMemberHistory resources for the backend system (no user).
  flows: []
  scope: system/FamilyMemberHistory.c
- description: Read + search (SMART v2) access to ChargeItem resources for the patient in context.
  flows: []
  scope: patient/ChargeItem.rs
- description: Read + search (SMART v2) access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.rs
- description: Read and search (SMART v1) access to ChargeItem resources for the patient in context.
  flows: []
  scope: patient/ChargeItem.read
- description: Read and search (SMART v1) access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.read
- description: create access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.create
- description: create access to ChargeItem resources for the authorized user.
  flows: []
  scope: user/ChargeItem.create
- description: Create access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.c
- description: Create access to ChargeItem resources for the authorized user.
  flows: []
  scope: user/ChargeItem.c
- description: Update access to ChargeItem resources for the authorized user.
  flows: []
  scope: user/ChargeItem.u
- description: Update access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.u
- description: update access to ChargeItem resources for the authorized user.
  flows: []
  scope: user/ChargeItem.update
- description: update access to ChargeItem resources for the backend system (no user).
  flows: []
  scope: system/ChargeItem.update
slug: eclinicalworks-scopes
source_filename: eclinicalworks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://fhir4.eclinicalworks.com/fhir/r4/FEIGCD/.well-known/smart-configuration\ndocs: https://fhir.eclinicalworks.com/ecwopendev/documentation\nnote: SMART on FHIR scope set read verbatim from the SMART configuration document served by the eClinicalWorks\n  FHIR Facade. The identical 486-scope set is served on the healow patient-facing facade (https://fhir4.healow.com/fhir/r4/{practice_code}/.well-known/smart-configuration).\n  Scope descriptions for the patient/user/system resource scopes are derived mechanically from the SMART\n  v1/v2 scope grammar; the identity and launch-context descriptions are taken from the eClinicalWorks\n  \"Scopes Supported by eClinicalWorks\" documentation page. Both SMART v1 (.read/.write) and SMART v2 (.rs/.c/.u/.d/.cruds)\n  forms are advertised (capabilities include permission-v1 and permission-v2).\nauthorization_servers:\n- name: eClinicalWorks FHIR Authorization Server\n  issuer: https://fhir4.eclinicalworks.com/fhir/r4/{practice_code}\n\
  \  authorization_endpoint: https://oauthserver.eclinicalworks.com/oauth/oauth2/authorize\n  token_endpoint: https://oauthserver.eclinicalworks.com/oauth/oauth2/token\n  jwks_uri: https://oauthserver.eclinicalworks.com/oauth/oauth2/jwks\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_jwt\n  code_challenge_methods_supported:\n  - S256\n  smart_capabilities:\n  - launch-ehr\n  - launch-standalone\n  - client-public\n  - client-confidential-symmetric\n  - context-passthrough-banner\n  - context-passthrough-style\n  - context-ehr-patient\n  - context-ehr-encounter\n  - context-standalone-patient\n  - context-standalone-encounter\n  - permission-offline\n  - permission-patient\n  - permission-user\n  - sso-openid-connect\n  - context-banner\n  - context-style\n  - permission-v2\n  - client-confidential-asymmetric\n  -\
  \ permission-v1\n  - authorize-post\nsummary:\n  scope_count: 486\n  by_category:\n    identity: 4\n    patient: 159\n    user: 156\n    launch-context: 2\n    system: 165\nscopes:\n- scope: openid\n  category: identity\n  description: OpenID Connect authentication of the launching user.\n- scope: profile\n  category: identity\n  description: Retrieve profile information about the current logged-in user.\n- scope: fhirUser\n  category: identity\n  description: Retrieve the FHIR resource representing the current logged-in user.\n- scope: patient/*.*\n  category: patient\n  description: All operations access to all FHIR resource types for the patient in context.\n- scope: user/*.*\n  category: user\n  description: All operations access to all FHIR resource types for the authorized user.\n- scope: offline_access\n  category: identity\n  description: Request a refresh_token usable after the end user is no longer online (background refresh).\n- scope: launch\n  category: launch-context\n  description:\
  \ Obtain launch context when the app is launched from within the EHR (EHR Launch).\n- scope: launch/patient\n  category: launch-context\n  description: Request that a patient be selected at launch time (Standalone Launch).\n- scope: patient/Medication.read\n  category: patient\n  description: Read and search (SMART v1) access to Medication resources for the patient in context.\n- scope: patient/Medication.rs\n  category: patient\n  description: Read + search (SMART v2) access to Medication resources for the patient in context.\n- scope: patient/Medication.c\n  category: patient\n  description: Create access to Medication resources for the patient in context.\n- scope: patient/Medication.u\n  category: patient\n  description: Update access to Medication resources for the patient in context.\n- scope: patient/AllergyIntolerance.read\n  category: patient\n  description: Read and search (SMART v1) access to AllergyIntolerance resources for the patient in context.\n- scope: patient/AllergyIntolerance.rs\n\
  \  category: patient\n  description: Read + search (SMART v2) access to AllergyIntolerance resources for the patient in context.\n- scope: patient/AllergyIntolerance.c\n  category: patient\n  description: Create access to AllergyIntolerance resources for the patient in context.\n- scope: patient/AllergyIntolerance.u\n  category: patient\n  description: Update access to AllergyIntolerance resources for the patient in context.\n- scope: patient/CarePlan.read\n  category: patient\n  description: Read and search (SMART v1) access to CarePlan resources for the patient in context.\n- scope: patient/CarePlan.rs\n  category: patient\n  description: Read + search (SMART v2) access to CarePlan resources for the patient in context.\n- scope: patient/CarePlan.c\n  category: patient\n  description: Create access to CarePlan resources for the patient in context.\n- scope: patient/CarePlan.u\n  category: patient\n  description: Update access to CarePlan resources for the patient in context.\n- scope:\
  \ patient/CareTeam.read\n  category: patient\n  description: Read and search (SMART v1) access to CareTeam resources for the patient in context.\n- scope: patient/CareTeam.rs\n  category: patient\n  description: Read + search (SMART v2) access to CareTeam resources for the patient in context.\n- scope: patient/CareTeam.c\n  category: patient\n  description: Create access to CareTeam resources for the patient in context.\n- scope: patient/CareTeam.u\n  category: patient\n  description: Update access to CareTeam resources for the patient in context.\n- scope: patient/Condition.read\n  category: patient\n  description: Read and search (SMART v1) access to Condition resources for the patient in context.\n- scope: patient/Condition.rs\n  category: patient\n  description: Read + search (SMART v2) access to Condition resources for the patient in context.\n- scope: patient/Condition.c\n  category: patient\n  description: Create access to Condition resources for the patient in context.\n- scope:\
  \ patient/Condition.u\n  category: patient\n  description: Update access to Condition resources for the patient in context.\n- scope: patient/Device.read\n  category: patient\n  description: Read and search (SMART v1) access to Device resources for the patient in context.\n- scope: patient/Device.rs\n  category: patient\n  description: Read + search (SMART v2) access to Device resources for the patient in context.\n- scope: patient/Device.c\n  category: patient\n  description: Create access to Device resources for the patient in context.\n- scope: patient/Device.u\n  category: patient\n  description: Update access to Device resources for the patient in context.\n- scope: patient/DiagnosticReport.read\n  category: patient\n  description: Read and search (SMART v1) access to DiagnosticReport resources for the patient in context.\n- scope: patient/DiagnosticReport.rs\n  category: patient\n  description: Read + search (SMART v2) access to DiagnosticReport resources for the patient in context.\n\
  - scope: patient/DiagnosticReport.c\n  category: patient\n  description: Create access to DiagnosticReport resources for the patient in context.\n- scope: patient/DiagnosticReport.u\n  category: patient\n  description: Update access to DiagnosticReport resources for the patient in context.\n- scope: patient/DocumentReference.read\n  category: patient\n  description: Read and search (SMART v1) access to DocumentReference resources for the patient in context.\n- scope: patient/DocumentReference.rs\n  category: patient\n  description: Read + search (SMART v2) access to DocumentReference resources for the patient in context.\n- scope: patient/DocumentReference.c\n  category: patient\n  description: Create access to DocumentReference resources for the patient in context.\n- scope: patient/DocumentReference.u\n  category: patient\n  description: Update access to DocumentReference resources for the patient in context.\n- scope: patient/Encounter.read\n  category: patient\n  description: Read\
  \ and search (SMART v1) access to Encounter resources for the patient in context.\n- scope: patient/Encounter.rs\n  category: patient\n  description: Read + search (SMART v2) access to Encounter resources for the patient in context.\n- scope: patient/Encounter.c\n  category: patient\n  description: Create access to Encounter resources for the patient in context.\n- scope: patient/Encounter.u\n  category: patient\n  description: Update access to Encounter resources for the patient in context.\n- scope: patient/Goal.read\n  category: patient\n  description: Read and search (SMART v1) access to Goal resources for the patient in context.\n- scope: patient/Goal.rs\n  category: patient\n  description: Read + search (SMART v2) access to Goal resources for the patient in context.\n- scope: patient/Goal.c\n  category: patient\n  description: Create access to Goal resources for the patient in context.\n- scope: patient/Goal.u\n  category: patient\n  description: Update access to Goal resources for\
  \ the patient in context.\n- scope: patient/Immunization.read\n  category: patient\n  description: Read and search (SMART v1) access to Immunization resources for the patient in context.\n- scope: patient/Immunization.rs\n  category: patient\n  description: Read + search (SMART v2) access to Immunization resources for the patient in context.\n- scope: patient/Immunization.c\n  category: patient\n  description: Create access to Immunization resources for the patient in context.\n- scope: patient/Immunization.u\n  category: patient\n  description: Update access to Immunization resources for the patient in context.\n- scope: patient/Location.read\n  category: patient\n  description: Read and search (SMART v1) access to Location resources for the patient in context.\n- scope: patient/Location.rs\n  category: patient\n  description: Read + search (SMART v2) access to Location resources for the patient in context.\n- scope: patient/Location.c\n  category: patient\n  description: Create access\
  \ to Location resources for the patient in context.\n- scope: patient/Location.u\n  category: patient\n  description: Update access to Location resources for the patient in context.\n- scope: patient/MedicationRequest.read\n  category: patient\n  description: Read and search (SMART v1) access to MedicationRequest resources for the patient in context.\n- scope: patient/MedicationRequest.rs\n  category: patient\n  description: Read + search (SMART v2) access to MedicationRequest resources for the patient in context.\n- scope: patient/MedicationRequest.c\n  category: patient\n  description: Create access to MedicationRequest resources for the patient in context.\n- scope: patient/MedicationRequest.u\n  category: patient\n  description: Update access to MedicationRequest resources for the patient in context.\n- scope: patient/MedicationAdministration.read\n  category: patient\n  description: Read and search (SMART v1) access to MedicationAdministration resources for the patient\n    in context.\n\
  - scope: patient/MedicationAdministration.rs\n  category: patient\n  description: Read + search (SMART v2) access to MedicationAdministration resources for the patient in\n    context.\n- scope: patient/MedicationAdministration.c\n  category: patient\n  description: Create access to MedicationAdministration resources for the patient in context.\n- scope: patient/MedicationAdministration.u\n  category: patient\n  description: Update access to MedicationAdministration resources for the patient in context.\n- scope: patient/Observation.read\n  category: patient\n  description: Read and search (SMART v1) access to Observation resources for the patient in context.\n- scope: patient/Observation.rs\n  category: patient\n  description: Read + search (SMART v2) access to Observation resources for the patient in context.\n- scope: patient/Observation.c\n  category: patient\n  description: Create access to Observation resources for the patient in context.\n- scope: patient/Observation.u\n  category:\
  \ patient\n  description: Update access to Observation resources for the patient in context.\n- scope: patient/Organization.read\n  category: patient\n  description: Read and search (SMART v1) access to Organization resources for the patient in context.\n- scope: patient/Organization.rs\n  category: patient\n  description: Read + search (SMART v2) access to Organization resources for the patient in context.\n- scope: patient/Organization.c\n  category: patient\n  description: Create access to Organization resources for the patient in context.\n- scope: patient/Organization.u\n  category: patient\n  description: Update access to Organization resources for the patient in context.\n- scope: patient/Patient.read\n  category: patient\n  description: Read and search (SMART v1) access to Patient resources for the patient in context.\n- scope: patient/Patient.rs\n  category: patient\n  description: Read + search (SMART v2) access to Patient resources for the patient in context.\n- scope: patient/Patient.c\n\
  \  category: patient\n  description: Create access to Patient resources for the patient in context.\n- scope: patient/Patient.u\n  category: patient\n  description: Update access to Patient resources for the patient in context.\n- scope: patient/Practitioner.read\n  category: patient\n  description: Read and search (SMART v1) access to Practitioner resources for the patient in context.\n- scope: patient/Practitioner.rs\n  category: patient\n  description: Read + search (SMART v2) access to Practitioner resources for the patient in context.\n- scope: patient/Practitioner.c\n  category: patient\n  description: Create access to Practitioner resources for the patient in context.\n- scope: patient/Practitioner.u\n  category: patient\n  description: Update access to Practitioner resources for the patient in context.\n- scope: patient/PractitionerRole.read\n  category: patient\n  description: Read and search (SMART v1) access to PractitionerRole resources for the patient in context.\n- scope:\
  \ patient/PractitionerRole.rs\n  category: patient\n  description: Read + search (SMART v2) access to PractitionerRole resources for the patient in context.\n- scope: patient/PractitionerRole.c\n  category: patient\n  description: Create access to PractitionerRole resources for the patient in context.\n- scope: patient/PractitionerRole.u\n  category: patient\n  description: Update access to PractitionerRole resources for the patient in context.\n- scope: patient/Procedure.read\n  category: patient\n  description: Read and search (SMART v1) access to Procedure resources for the patient in context.\n- scope: patient/Procedure.rs\n  category: patient\n  description: Read + search (SMART v2) access to Procedure resources for the patient in context.\n- scope: patient/Procedure.c\n  category: patient\n  description: Create access to Procedure resources for the patient in context.\n- scope: patient/Procedure.u\n  category: patient\n  description: Update access to Procedure resources for the patient\
  \ in context.\n- scope: patient/Provenance.read\n  category: patient\n  description: Read and search (SMART v1) access to Provenance resources for the patient in context.\n- scope: patient/Provenance.rs\n  category: patient\n  description: Read + search (SMART v2) access to Provenance resources for the patient in context.\n- scope: patient/Provenance.c\n  category: patient\n  description: Create access to Provenance resources for the patient in context.\n- scope: patient/Provenance.u\n  category: patient\n  description: Update access to Provenance resources for the patient in context.\n- scope: user/Medication.read\n  category: user\n  description: Read and search (SMART v1) access to Medication resources for the authorized user.\n- scope: user/Medication.rs\n  category: user\n  description: Read + search (SMART v2) access to Medication resources for the authorized user.\n- scope: user/Medication.c\n  category: user\n  description: Create access to Medication resources for the authorized\
  \ user.\n- scope: user/Medication.u\n  category: user\n  description: Update access to Medication resources for the authorized user.\n- scope: user/AllergyIntolerance.read\n  category: user\n  description: Read and search (SMART v1) access to AllergyIntolerance resources for the authorized user.\n- scope: user/AllergyIntolerance.rs\n  category: user\n  description: Read + search (SMART v2) access to AllergyIntolerance resources for the authorized user.\n- scope: user/AllergyIntolerance.c\n  category: user\n  description: Create access to AllergyIntolerance resources for the authorized user.\n- scope: user/AllergyIntolerance.u\n  category: user\n  description: Update access to AllergyIntolerance resources for the authorized user.\n- scope: user/CarePlan.read\n  category: user\n  description: Read and search (SMART v1) access to CarePlan resources for the authorized user.\n- scope: user/CarePlan.rs\n  category: user\n  description: Read + search (SMART v2) access to CarePlan resources for\
  \ the authorized user.\n- scope: user/CarePlan.c\n  category: user\n  description: Create access to CarePlan resources for the authorized user.\n- scope: user/CarePlan.u\n  category: user\n  description: Update access to CarePlan resources for the authorized user.\n- scope: user/CareTeam.read\n  category: user\n  description: Read and search (SMART v1) access to CareTeam resources for the authorized user.\n- scope: user/CareTeam.rs\n  category: user\n  description: Read + search (SMART v2) access to CareTeam resources for the authorized user.\n- scope: user/CareTeam.c\n  category: user\n  description: Create access to CareTeam resources for the authorized user.\n- scope: user/CareTeam.u\n  category: user\n  description: Update access to CareTeam resources for the authorized user.\n- scope: user/Condition.read\n  category: user\n  description: Read and search (SMART v1) access to Condition resources for the authorized user.\n- scope: user/Condition.rs\n  category: user\n  description: Read\
  \ + search (SMART v2) access to Condition resources for the authorized user.\n- scope: user/Condition.c\n  category: user\n  description: Create access to Condition resources for the authorized user.\n- scope: user/Condition.u\n  category: user\n  description: Update access to Condition resources for the authorized user.\n- scope: user/Device.read\n  category: user\n  description: Read and search (SMART v1) access to Device resources for the authorized user.\n- scope: user/Device.rs\n  category: user\n  description: Read + search (SMART v2) access to Device resources for the authorized user.\n- scope: user/Device.c\n  category: user\n  description: Create access to Device resources for the authorized user.\n- scope: user/Device.u\n  category: user\n  description: Update access to Device resources for the authorized user.\n- scope: user/DiagnosticReport.read\n  category: user\n  description: Read and search (SMART v1) access to DiagnosticReport resources for the authorized user.\n- scope:\
  \ user/DiagnosticReport.rs\n  category: user\n  description: Read + search (SMART v2) access to DiagnosticReport resources for the authorized user.\n- scope: user/DiagnosticReport.c\n  category: user\n  description: Create access to DiagnosticReport resources for the authorized user.\n- scope: user/DiagnosticReport.u\n  category: user\n  description: Update access to DiagnosticReport resources for the authorized user.\n- scope: user/DocumentReference.read\n  category: user\n  description: Read and search (SMART v1) access to DocumentReference resources for the authorized user.\n- scope: user/DocumentReference.rs\n  category: user\n  description: Read + search (SMART v2) access to DocumentReference resources for the authorized user.\n- scope: user/DocumentReference.c\n  category: user\n  description: Create access to DocumentReference resources for the authorized user.\n- scope: user/DocumentReference.u\n  category: user\n  description: Update access to DocumentReference resources for the\
  \ authorized user.\n- scope: user/Encounter.read\n  category: user\n  description: Read and search (SMART v1) access to Encounter resources for the authorized user.\n- scope: user/Encounter.rs\n  category: user\n  description: Read + search (SMART v2) access to Encounter resources for the authorized user.\n- scope: user/Encounter.c\n  category: user\n  description: Create access to Encounter resources for the authorized user.\n- scope: user/Encounter.u\n  category: user\n  description: Update access to Encounter resources for the authorized user.\n- scope: user/Goal.read\n  category: user\n  description: Read and search (SMART v1) access to Goal resources for the authorized user.\n- scope: user/Goal.rs\n  category: user\n  description: Read + search (SMART v2) access to Goal resources for the authorized user.\n- scope: user/Goal.c\n  category: user\n  description: Create access to Goal resources for the authorized user.\n- scope: user/Goal.u\n  category: user\n  description: Update access\
  \ to Goal resources for the authorized user.\n- scope: user/Immunization.read\n  category: user\n  description: Read and search (SMART v1) access to Immunization resources for the authorized user.\n- scope: user/Immunization.rs\n  category: user\n  description: Read + search (SMART v2) access to Immunization resources for the authorized user.\n- scope: user/Immunization.c\n  category: user\n  description: Create access to Immunization resources for the authorized user.\n- scope: user/Immunization.u\n  category: user\n  description: Update access to Immunization resources for the authorized user.\n- scope: user/Location.read\n  category: user\n  description: Read and search (SMART v1) access to Location resources for the authorized user.\n- scope: user/Location.rs\n  category: user\n  description: Read + search (SMART v2) access to Location resources for the authorized user.\n- scope: user/Location.c\n  category: user\n  description: Create access to Location resources for the authorized\
  \ user.\n- scope: user/Location.u\n  category: user\n  description: Update access to Location resources for the authorized user.\n- scope: user/MedicationRequest.read\n  category: user\n  description: Read and search (SMART v1) access to MedicationRequest resources for the authorized user.\n- scope: user/MedicationRequest.rs\n  category: user\n  description: Read + search (SMART v2) access to MedicationRequest resources for the authorized user.\n- scope: user/MedicationRequest.c\n  category: user\n  description: Create access to MedicationRequest resources for the authorized user.\n- scope: user/MedicationRequest.u\n  category: user\n  description: Update access to MedicationRequest resources for the authorized user.\n- scope: user/MedicationAdministration.read\n  category: user\n  description: Read and search (SMART v1) access to MedicationAdministration resources for the authorized\n    user.\n- scope: user/MedicationAdministration.rs\n  category: user\n  description: Read + search (SMART\
  \ v2) access to MedicationAdministration resources for the authorized\n    user.\n- scope: user/MedicationAdministration.c\n  category: user\n  description: Create access to MedicationAdministration resources for the authorized user.\n- scope: user/MedicationAdministration.u\n  category: user\n  description: Update access to MedicationAdministration resources for the authorized user.\n- scope: user/Observation.read\n  category: user\n  description: Read and search (SMART v1) access to Observation resources for the authorized user.\n- scope: user/Observation.rs\n  category: user\n  description: Read + search (SMART v2) access to Observation resources for the authorized user.\n- scope: user/Observation.c\n  category: user\n  description: Create access to Observation resources for the authorized user.\n- scope: user/Observation.u\n  category: user\n  description: Update access to Observation resources for the authorized user.\n- scope: user/Organization.read\n  category: user\n  description:\
  \ Read and search (SMART v1) access to Organization resources for the authorized user.\n- scope: user/Organization.rs\n  category: user\n  description: Read + search (SMART v2) access to Organization resources for the authorized user.\n- scope: user/Organization.c\n  category: user\n  description: Create access to Organization resources for the authorized user.\n- scope: user/Organization.u\n  category: user\n  description: Update access to Organization resources for the authorized user.\n- scope: user/Patient.read\n  category: user\n  description: Read and search (SMART v1) access to Patient resources for the authorized user.\n- scope: user/Patient.rs\n  category: user\n  description: Read + search (SMART v2) access to Patient resources for the authorized user.\n- scope: user/Patient.c\n  category: user\n  description: Create access to Patient resources for the authorized user.\n- scope: user/Patient.u\n  category: user\n  description: Update access to Patient resources for the authorized\
  \ user.\n- scope: user/Practitioner.read\n  category: user\n  description: Read and search (SMART v1) access to Practitioner resources for the authorized user.\n- scope: user/Practitioner.rs\n  category: user\n  description: Read + search (SMART v2) access to Practitioner resources for the authorized user.\n- scope: user/Practitioner.c\n  category: user\n  description: Create access to Practitioner resources for the authorized user.\n- scope: user/Practitioner.u\n  category: user\n  description: Update access to Practitioner resources for the authorized user.\n- scope: user/PractitionerRole.read\n  category: user\n  description: Read and search (SMART v1) access to PractitionerRole resources for the authorized user.\n- scope: user/PractitionerRole.rs\n  category: user\n  description: Read + search (SMART v2) access to PractitionerRole resources for the authorized user.\n- scope: user/PractitionerRole.c\n  category: user\n  description: Create access to PractitionerRole resources for the\
  \ authorized user.\n- scope: user/PractitionerRole.u\n  category: user\n  description: Update access to PractitionerRole resources for the authorized user.\n- scope: user/Procedure.read\n  category: user\n  description: Read and search (SMART v1) access to Procedure resources for the authorized user.\n- scope: user/Procedure.rs\n  category: user\n  description: Read + search (SMART v2) access to Procedure resources for the authorized user.\n- scope: user/Procedure.c\n  category: user\n  description: Create access to Procedure resources for the authorized user.\n- scope: user/Procedure.u\n  category: user\n  description: Update access to Procedure resources for the authorized user.\n- scope: user/Provenance.read\n  category: user\n  description: Read and search (SMART v1) access to Provenance resources for the authorized user.\n- scope: user/Provenance.rs\n  category: user\n  description: Read + search (SMART v2) access to Provenance resources for the authorized user.\n- scope: user/Provenance.c\n\
  \  category: user\n  description: Create access to Provenance resources for the authorized user.\n- scope: user/Provenance.u\n  category: user\n  description: Update access to Provenance resources for the authorized user.\n- scope: system/Medication.read\n  category: system\n  description: Read and search (SMART v1) access to Medication resources for the backend system (no user).\n- scope: system/Medication.rs\n  category: system\n  description: Read + search (SMART v2) access to Medication resources for the backend system (no user).\n- scope: system/Medication.c\n  category: system\n  description: Create access to Medication resources for the backend system (no user).\n- scope: system/Medication.u\n  category: system\n  description: Update access to Medication resources for the backend system (no user).\n- scope: system/AllergyIntolerance.read\n  category: system\n  description: Read and search (SMART v1) access to AllergyIntolerance resources for the backend system\n    (no user).\n\
  - scope: system/AllergyIntolerance.rs\n  category: system\n  description: Read + search (SMART v2) access to AllergyIntolerance resources for the backend system\n    (no user).\n- scope: system/AllergyIntolerance.c\n  category: system\n  description: Create access to AllergyIntolerance resources for the backend system (no user).\n- scope: system/AllergyIntolerance.u\n  category: system\n  description: Update access to AllergyIntolerance resources for the backend system (no user).\n- scope: system/CarePlan.read\n  category: system\n  description: Read and search (SMART v1) access to CarePlan resources for the backend system (no user).\n- scope: system/CarePlan.rs\n  category: system\n  description: Read + search (SMART v2) access to CarePlan resources for the backend system (no user).\n- scope: system/CarePlan.c\n  category: system\n  description: Create access to CarePlan resources for the backend system (no user).\n- scope: system/CarePlan.u\n  category: system\n  description: Update\
  \ access to CarePlan resources for the backend system (no user).\n- scope: system/CareTeam.read\n  category: system\n  description: Read and search (SMART v1) access to CareTeam resources for the backend system (no user).\n- scope: system/CareTeam.rs\n  category: system\n  description: Read + search (SMART v2) access to CareTeam resources for the backend system (no user).\n- scope: system/CareTeam.c\n  category: system\n  description: Create access to CareTeam resources for the backend system (no user).\n- scope: system/CareTeam.u\n  category: system\n  description: Update access to CareTeam resources for the backend system (no user).\n- scope: system/Condition.read\n  category: system\n  description: Read and search (SMART v1) access to Condition resources for the backend system (no user).\n- scope: system/Condition.rs\n  category: system\n  description: Read + search (SMART v2) access to Condition resources for the backend system (no user).\n- scope: system/Condition.c\n  category: system\n\
  \  description: Create access to Condition resources for the backend system (no user).\n- scope: system/Condition.u\n  category: system\n  description: Update access to Condition resources for the backend system (no user).\n- scope: system/Device.read\n  category: system\n  description: Read and search (SMART v1) access to Device resources for the backend system (no user).\n- scope: system/Device.rs\n  category: system\n  description: Read + search (SMART v2) access to Device resources for the backend system (no user).\n- scope: system/Device.c\n  category: system\n  description: Create access to Device resources for the backend system (no user).\n- scope: system/Device.u\n  category: system\n  description: Update access to Device resources for the backend system (no user).\n- scope: system/DiagnosticReport.read\n  category: system\n  description: Read and search (SMART v1) access to DiagnosticReport resources for the backend system\n    (no user).\n- scope: system/DiagnosticReport.rs\n\
  \  category: system\n  description: Read + search (SMART v2) access to DiagnosticReport resources for the backend system (no\n    user).\n- scope: system/DiagnosticReport.c\n  category: system\n  description: Create access to DiagnosticReport resources for the backend system (no user).\n- scope: system/DiagnosticReport.u\n  category: system\n  description: Update access to DiagnosticReport resources for the backend system (no user).\n- scope: system/DocumentReference.read\n  category: system\n  description: Read and search (SMART v1) access to DocumentReference resources for the backend system\n    (no user).\n- scope: system/DocumentReference.rs\n  category: system\n  description: Read + search (SMART v2) access to DocumentReference resources for the backend system (no\n    user).\n- scope: system/DocumentReference.c\n  category: system\n  description: Create access to DocumentReference resources for the backend system (no user).\n- scope: system/DocumentReference.u\n  category: system\n\
  \  description: Update access to DocumentReference resources for the backend system (no user).\n- scope: system/Encounter.read\n  category: system\n  description: Read and search (SMART v1) access to Encounter resources for the backend system (no user).\n- scope: system/Encounter.rs\n  category: system\n  description: Read + search (SMART v2) access to Encounter resources for the backend system (no user).\n- scope: system/Encounter.c\n  category: system\n  description: Create access to Encounter resources for the backend system (no user).\n- scope: system/Encounter.u\n  category: system\n  description: Update access to Encounter resources for the backend system (no user).\n- scope: system/Goal.read\n  category: system\n  description: Read and search (SMART v1) access to Goal resources for the backend system (no user).\n- scope: system/Goal.rs\n  category: system\n  description: Read + search (SMART v2) access to Goal resources for the backend system (no user).\n- scope: system/Goal.c\n\
  \  category: system\n  description: Create access to Goal resources for the backend system (no user).\n- scope: system/Goal.u\n  category: system\n  description: Update access to Goal resources for the backend system (no user).\n- scope: system/Immunization.read\n  category: system\n  description: Read and search (SMART v1) access to Immunization resources for the bac\n\n# --- truncated at 32 KB (66 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/eclinicalworks/refs/heads/main/scopes/eclinicalworks-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eclinicalworks/refs/heads/main/scopes/eclinicalworks-scopes.yml
summary_line: 486 scopes
tags:
- EHR
- FHIR
- Healthcare
- Electronic Health Records
- Practice Management
- Clinical Data
- Health Information Exchange
- Patient Data
- Appointments
- Billing
- SMART on FHIR
- US Core
- USCDI
- Bulk Data
- Remote Patient Monitoring
- Interoperability
- ONC Certified
- CDS Hooks
- healow
token_urls: []
---
