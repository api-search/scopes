---
authorization_urls:
- https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize
description: OAuth 2.0 / SMART App Launch scopes advertised by the Veradigm (formerly Allscripts) FHIR authorization server. Read verbatim from the scopes_supported array of the live SMART configuration document served on the published Veradigm EHR R4 sandbox base URL, and cross-checked against the identical scopes_supported array in the OpenID Connect discovery document on the issuer. Nothing here is inferred - the descriptions restate the SMART App Launch v1/v2 semantics of the scope strings the server itself publishes. Veradigm's Process Overview page states that a registered FHIR application may use SMART v1 (.read) scopes or SMART v2 (.rs) scopes but never both; an application requesting both is not approved.
docs: https://developer.veradigm.com/Fhir/ProcessOverview
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Allscripts Healthcare Solutions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allscripts Healthcare Solutions publishes 237 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allscripts Healthcare Solutions API on a user''s behalf.


  Tokens are issued from https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allscripts Healthcare Solutions
provider_slug: allscripts-healthcare-solutions
schemes:
- flows:
  - authorizationUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token
  - flow: clientCredentials
    note: SMART Backend Services. Only FHIR applications registered with App Type "System" may use client_credentials; the developer registers a JWKS URL and the server authenticates a private_key_jwt assertion against it.
    tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token
  issuer: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization
  jwks_uri: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration/jwks
  name: SMART on FHIR (OAuth 2.0 + OpenID Connect)
  source: well-known/allscripts-healthcare-solutions-smart-configuration.json
scope_count: 237
scope_names:
- fhir
- fhirUser
- launch
- launch/patient
- offline_access
- online_access
- openid
- patient/*.read
- patient/*.rs
- patient/AllergyIntolerance.read
- patient/AllergyIntolerance.rs
- patient/Binary.read
- patient/Binary.rs
- patient/CarePlan.read
- patient/CarePlan.rs
- patient/CareTeam.read
- patient/CareTeam.rs
- patient/Condition.read
- patient/Condition.rs
- patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- patient/Coverage.read
- patient/Coverage.rs
- patient/Device.read
- patient/Device.rs
- patient/DiagnosticOrder.read
- patient/DiagnosticOrder.rs
- patient/DiagnosticReport.read
- patient/DiagnosticReport.rs
- patient/DocumentReference.read
- patient/DocumentReference.rs
- patient/Encounter.read
- patient/Encounter.rs
- patient/Goal.read
- patient/Goal.rs
- patient/Group.read
- patient/Group.rs
- patient/Immunization.read
- patient/Immunization.rs
- patient/Location.read
- patient/Location.rs
- patient/Medication.read
- patient/Medication.rs
- patient/MedicationAdministration.read
- patient/MedicationAdministration.rs
- patient/MedicationDispense.read
- patient/MedicationDispense.rs
- patient/MedicationOrder.read
- patient/MedicationOrder.rs
- patient/MedicationRequest.read
- patient/MedicationRequest.rs
- patient/MedicationStatement.read
- patient/MedicationStatement.rs
- patient/Observation.read
- patient/Observation.rs
- patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- patient/Organization.read
- patient/Organization.rs
- patient/Patient.read
- patient/Patient.rs
- patient/Practitioner.read
- patient/Practitioner.rs
- patient/PractitionerRole.read
- patient/PractitionerRole.rs
- patient/Procedure.read
- patient/Procedure.rs
- patient/Provenance.read
- patient/Provenance.rs
- patient/Questionnaire.read
- patient/Questionnaire.rs
- patient/QuestionnaireResponse.read
- patient/QuestionnaireResponse.rs
- patient/RelatedPerson.read
- patient/RelatedPerson.rs
- patient/ServiceRequest.read
- patient/ServiceRequest.rs
- patient/Specimen.read
- patient/Specimen.rs
- profile
- system/*.read
- system/*.rs
- system/AllergyIntolerance.read
- system/AllergyIntolerance.rs
- system/Binary.read
- system/Binary.rs
- system/CarePlan.read
- system/CarePlan.rs
- system/CareTeam.read
- system/CareTeam.rs
- system/Condition.read
- system/Condition.rs
- system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- system/Coverage.read
- system/Coverage.rs
- system/Device.read
- system/Device.rs
- system/DiagnosticOrder.read
- system/DiagnosticOrder.rs
- system/DiagnosticReport.read
- system/DiagnosticReport.rs
- system/DocumentReference.read
- system/DocumentReference.rs
- system/Encounter.read
- system/Encounter.rs
- system/Goal.read
- system/Goal.rs
- system/Group.read
- system/Group.rs
- system/Immunization.read
- system/Immunization.rs
- system/Location.read
- system/Location.rs
- system/Medication.read
- system/Medication.rs
- system/MedicationAdministration.read
- system/MedicationAdministration.rs
- system/MedicationDispense.read
- system/MedicationDispense.rs
- system/MedicationOrder.read
- system/MedicationOrder.rs
- system/MedicationRequest.read
- system/MedicationRequest.rs
- system/MedicationStatement.read
- system/MedicationStatement.rs
- system/Observation.read
- system/Observation.rs
- system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- system/Organization.read
- system/Organization.rs
- system/Patient.read
- system/Patient.rs
- system/Practitioner.read
- system/Practitioner.rs
- system/PractitionerRole.read
- system/PractitionerRole.rs
- system/Procedure.read
- system/Procedure.rs
- system/Provenance.read
- system/Provenance.rs
- system/Questionnaire.read
- system/Questionnaire.rs
- system/QuestionnaireResponse.read
- system/QuestionnaireResponse.rs
- system/RelatedPerson.read
- system/RelatedPerson.rs
- system/ServiceRequest.read
- system/ServiceRequest.rs
- system/Specimen.read
- system/Specimen.rs
- user/*.*
- user/*.read
- user/*.rs
- user/AllergyIntolerance.read
- user/AllergyIntolerance.rs
- user/Binary.read
- user/Binary.rs
- user/CarePlan.read
- user/CarePlan.rs
- user/CareTeam.read
- user/CareTeam.rs
- user/Condition.read
- user/Condition.rs
- user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- user/Coverage.read
- user/Coverage.rs
- user/Device.read
- user/Device.rs
- user/DiagnosticOrder.read
- user/DiagnosticOrder.rs
- user/DiagnosticReport.read
- user/DiagnosticReport.rs
- user/DocumentReference.read
- user/DocumentReference.rs
- user/Encounter.read
- user/Encounter.rs
- user/Goal.read
- user/Goal.rs
- user/Group.read
- user/Group.rs
- user/Immunization.read
- user/Immunization.rs
- user/Location.read
- user/Location.rs
- user/Medication.read
- user/Medication.rs
- user/MedicationAdministration.read
- user/MedicationAdministration.rs
- user/MedicationDispense.read
- user/MedicationDispense.rs
- user/MedicationOrder.read
- user/MedicationOrder.rs
- user/MedicationRequest.read
- user/MedicationRequest.rs
- user/MedicationStatement.read
- user/MedicationStatement.rs
- user/Observation.read
- user/Observation.rs
- user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- user/Organization.read
- user/Organization.rs
- user/Patient.read
- user/Patient.rs
- user/Practitioner.read
- user/Practitioner.rs
- user/PractitionerRole.read
- user/PractitionerRole.rs
- user/Procedure.read
- user/Procedure.rs
- user/Provenance.read
- user/Provenance.rs
- user/Questionnaire.read
- user/Questionnaire.rs
- user/QuestionnaireResponse.read
- user/QuestionnaireResponse.rs
- user/RelatedPerson.read
- user/RelatedPerson.rs
- user/ServiceRequest.read
- user/ServiceRequest.rs
- user/Specimen.read
- user/Specimen.rs
scopes:
- description: Veradigm scope granting FHIR API access.
  flows:
  - authorizationCode
  scope: fhir
- description: SMART - return the FHIR resource representing the current user.
  flows:
  - authorizationCode
  scope: fhirUser
- description: SMART - request the full EHR launch context.
  flows:
  - authorizationCode
  scope: launch
- description: SMART - request the patient launch context in a standalone launch.
  flows:
  - authorizationCode
  scope: launch/patient
- description: Request a refresh token that survives the end of the session.
  flows:
  - authorizationCode
  scope: offline_access
- description: Request a refresh token valid only while the user session is live.
  flows:
  - authorizationCode
  scope: online_access
- description: OpenID Connect - request an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: SMART v1 (.read) - read every supported resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/*.read
- description: SMART v2 (.rs) - read and search every supported resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/*.rs
- description: SMART v1 (.read) - read the AllergyIntolerance resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: SMART v2 (.rs) - read and search the AllergyIntolerance resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.rs
- description: SMART v1 (.read) - read the Binary resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Binary.read
- description: SMART v2 (.rs) - read and search the Binary resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Binary.rs
- description: SMART v1 (.read) - read the CarePlan resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/CarePlan.read
- description: SMART v2 (.rs) - read and search the CarePlan resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/CarePlan.rs
- description: SMART v1 (.read) - read the CareTeam resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/CareTeam.read
- description: SMART v2 (.rs) - read and search the CareTeam resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/CareTeam.rs
- description: SMART v1 (.read) - read the Condition resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: SMART v2 (.rs) - read and search the Condition resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Condition.rs
- description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern.
  flows:
  - authorizationCode
  scope: patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis.
  flows:
  - authorizationCode
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item.
  flows:
  - authorizationCode
  scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: SMART v1 (.read) - read the Coverage resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: SMART v2 (.rs) - read and search the Coverage resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Coverage.rs
- description: SMART v1 (.read) - read the Device resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Device.read
- description: SMART v2 (.rs) - read and search the Device resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Device.rs
- description: SMART v1 (.read) - read the DiagnosticOrder resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticOrder.read
- description: SMART v2 (.rs) - read and search the DiagnosticOrder resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticOrder.rs
- description: SMART v1 (.read) - read the DiagnosticReport resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.read
- description: SMART v2 (.rs) - read and search the DiagnosticReport resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.rs
- description: SMART v1 (.read) - read the DocumentReference resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: SMART v2 (.rs) - read and search the DocumentReference resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/DocumentReference.rs
- description: SMART v1 (.read) - read the Encounter resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: SMART v2 (.rs) - read and search the Encounter resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Encounter.rs
- description: SMART v1 (.read) - read the Goal resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Goal.read
- description: SMART v2 (.rs) - read and search the Goal resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Goal.rs
- description: SMART v1 (.read) - read the Group resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Group.read
- description: SMART v2 (.rs) - read and search the Group resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Group.rs
- description: SMART v1 (.read) - read the Immunization resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: SMART v2 (.rs) - read and search the Immunization resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Immunization.rs
- description: SMART v1 (.read) - read the Location resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Location.read
- description: SMART v2 (.rs) - read and search the Location resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Location.rs
- description: SMART v1 (.read) - read the Medication resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Medication.read
- description: SMART v2 (.rs) - read and search the Medication resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Medication.rs
- description: SMART v1 (.read) - read the MedicationAdministration resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationAdministration.read
- description: SMART v2 (.rs) - read and search the MedicationAdministration resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationAdministration.rs
- description: SMART v1 (.read) - read the MedicationDispense resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.read
- description: SMART v2 (.rs) - read and search the MedicationDispense resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.rs
- description: SMART v1 (.read) - read the MedicationOrder resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationOrder.read
- description: SMART v2 (.rs) - read and search the MedicationOrder resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationOrder.rs
- description: SMART v1 (.read) - read the MedicationRequest resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: SMART v2 (.rs) - read and search the MedicationRequest resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.rs
- description: SMART v1 (.read) - read the MedicationStatement resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationStatement.read
- description: SMART v2 (.rs) - read and search the MedicationStatement resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationStatement.rs
- description: SMART v1 (.read) - read the Observation resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Observation.rs
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh.
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory.
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|social-history.
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|survey.
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs.
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: SMART v1 (.read) - read the Organization resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Organization.read
- description: SMART v2 (.rs) - read and search the Organization resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Organization.rs
- description: SMART v1 (.read) - read the Patient resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: SMART v2 (.rs) - read and search the Patient resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Patient.rs
- description: SMART v1 (.read) - read the Practitioner resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Practitioner.read
- description: SMART v2 (.rs) - read and search the Practitioner resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Practitioner.rs
- description: SMART v1 (.read) - read the PractitionerRole resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.read
- description: SMART v2 (.rs) - read and search the PractitionerRole resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.rs
- description: SMART v1 (.read) - read the Procedure resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Procedure.read
- description: SMART v2 (.rs) - read and search the Procedure resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Procedure.rs
- description: SMART v1 (.read) - read the Provenance resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Provenance.read
- description: SMART v2 (.rs) - read and search the Provenance resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Provenance.rs
- description: SMART v1 (.read) - read the Questionnaire resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Questionnaire.read
- description: SMART v2 (.rs) - read and search the Questionnaire resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Questionnaire.rs
- description: SMART v1 (.read) - read the QuestionnaireResponse resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/QuestionnaireResponse.read
- description: SMART v2 (.rs) - read and search the QuestionnaireResponse resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/QuestionnaireResponse.rs
- description: SMART v1 (.read) - read the RelatedPerson resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.read
- description: SMART v2 (.rs) - read and search the RelatedPerson resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.rs
- description: SMART v1 (.read) - read the ServiceRequest resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/ServiceRequest.read
- description: SMART v2 (.rs) - read and search the ServiceRequest resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/ServiceRequest.rs
- description: SMART v1 (.read) - read the Specimen resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Specimen.read
- description: SMART v2 (.rs) - read and search the Specimen resource for the patient in context.
  flows:
  - authorizationCode
  scope: patient/Specimen.rs
- description: OpenID Connect - request the profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: SMART v1 (.read) - read every supported resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/*.read
- description: SMART v2 (.rs) - read and search every supported resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/*.rs
- description: SMART v1 (.read) - read the AllergyIntolerance resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/AllergyIntolerance.read
- description: SMART v2 (.rs) - read and search the AllergyIntolerance resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/AllergyIntolerance.rs
- description: SMART v1 (.read) - read the Binary resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Binary.read
- description: SMART v2 (.rs) - read and search the Binary resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Binary.rs
- description: SMART v1 (.read) - read the CarePlan resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/CarePlan.read
- description: SMART v2 (.rs) - read and search the CarePlan resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/CarePlan.rs
- description: SMART v1 (.read) - read the CareTeam resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/CareTeam.read
- description: SMART v2 (.rs) - read and search the CareTeam resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/CareTeam.rs
- description: SMART v1 (.read) - read the Condition resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Condition.read
- description: SMART v2 (.rs) - read and search the Condition resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Condition.rs
- description: SMART v2 (.rs) - read and search the Condition resource for a backend System application (no user). Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern.
  flows:
  - clientCredentials
  scope: system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: SMART v2 (.rs) - read and search the Condition resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis.
  flows:
  - clientCredentials
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: SMART v2 (.rs) - read and search the Condition resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item.
  flows:
  - clientCredentials
  scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: SMART v1 (.read) - read the Coverage resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Coverage.read
- description: SMART v2 (.rs) - read and search the Coverage resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Coverage.rs
- description: SMART v1 (.read) - read the Device resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Device.read
- description: SMART v2 (.rs) - read and search the Device resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Device.rs
- description: SMART v1 (.read) - read the DiagnosticOrder resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DiagnosticOrder.read
- description: SMART v2 (.rs) - read and search the DiagnosticOrder resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DiagnosticOrder.rs
- description: SMART v1 (.read) - read the DiagnosticReport resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DiagnosticReport.read
- description: SMART v2 (.rs) - read and search the DiagnosticReport resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DiagnosticReport.rs
- description: SMART v1 (.read) - read the DocumentReference resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DocumentReference.read
- description: SMART v2 (.rs) - read and search the DocumentReference resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/DocumentReference.rs
- description: SMART v1 (.read) - read the Encounter resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Encounter.read
- description: SMART v2 (.rs) - read and search the Encounter resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Encounter.rs
- description: SMART v1 (.read) - read the Goal resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Goal.read
- description: SMART v2 (.rs) - read and search the Goal resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Goal.rs
- description: SMART v1 (.read) - read the Group resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Group.read
- description: SMART v2 (.rs) - read and search the Group resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Group.rs
- description: SMART v1 (.read) - read the Immunization resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Immunization.read
- description: SMART v2 (.rs) - read and search the Immunization resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Immunization.rs
- description: SMART v1 (.read) - read the Location resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Location.read
- description: SMART v2 (.rs) - read and search the Location resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Location.rs
- description: SMART v1 (.read) - read the Medication resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Medication.read
- description: SMART v2 (.rs) - read and search the Medication resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Medication.rs
- description: SMART v1 (.read) - read the MedicationAdministration resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationAdministration.read
- description: SMART v2 (.rs) - read and search the MedicationAdministration resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationAdministration.rs
- description: SMART v1 (.read) - read the MedicationDispense resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationDispense.read
- description: SMART v2 (.rs) - read and search the MedicationDispense resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationDispense.rs
- description: SMART v1 (.read) - read the MedicationOrder resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationOrder.read
- description: SMART v2 (.rs) - read and search the MedicationOrder resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationOrder.rs
- description: SMART v1 (.read) - read the MedicationRequest resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationRequest.read
- description: SMART v2 (.rs) - read and search the MedicationRequest resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationRequest.rs
- description: SMART v1 (.read) - read the MedicationStatement resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationStatement.read
- description: SMART v2 (.rs) - read and search the MedicationStatement resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/MedicationStatement.rs
- description: SMART v1 (.read) - read the Observation resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Observation.read
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Observation.rs
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user). Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh.
  flows:
  - clientCredentials
  scope: system/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory.
  flows:
  - clientCredentials
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|social-history.
  flows:
  - clientCredentials
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|survey.
  flows:
  - clientCredentials
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: SMART v2 (.rs) - read and search the Observation resource for a backend System application (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs.
  flows:
  - clientCredentials
  scope: system/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: SMART v1 (.read) - read the Organization resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Organization.read
- description: SMART v2 (.rs) - read and search the Organization resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Organization.rs
- description: SMART v1 (.read) - read the Patient resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Patient.read
- description: SMART v2 (.rs) - read and search the Patient resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Patient.rs
- description: SMART v1 (.read) - read the Practitioner resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Practitioner.read
- description: SMART v2 (.rs) - read and search the Practitioner resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Practitioner.rs
- description: SMART v1 (.read) - read the PractitionerRole resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/PractitionerRole.read
- description: SMART v2 (.rs) - read and search the PractitionerRole resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/PractitionerRole.rs
- description: SMART v1 (.read) - read the Procedure resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Procedure.read
- description: SMART v2 (.rs) - read and search the Procedure resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Procedure.rs
- description: SMART v1 (.read) - read the Provenance resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Provenance.read
- description: SMART v2 (.rs) - read and search the Provenance resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Provenance.rs
- description: SMART v1 (.read) - read the Questionnaire resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Questionnaire.read
- description: SMART v2 (.rs) - read and search the Questionnaire resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Questionnaire.rs
- description: SMART v1 (.read) - read the QuestionnaireResponse resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/QuestionnaireResponse.read
- description: SMART v2 (.rs) - read and search the QuestionnaireResponse resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/QuestionnaireResponse.rs
- description: SMART v1 (.read) - read the RelatedPerson resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/RelatedPerson.read
- description: SMART v2 (.rs) - read and search the RelatedPerson resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/RelatedPerson.rs
- description: SMART v1 (.read) - read the ServiceRequest resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/ServiceRequest.read
- description: SMART v2 (.rs) - read and search the ServiceRequest resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/ServiceRequest.rs
- description: SMART v1 (.read) - read the Specimen resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Specimen.read
- description: SMART v2 (.rs) - read and search the Specimen resource for a backend System application (no user).
  flows:
  - clientCredentials
  scope: system/Specimen.rs
- description: SMART - all advertised operations on every supported resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/*.*
- description: SMART v1 (.read) - read every supported resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/*.read
- description: SMART v2 (.rs) - read and search every supported resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/*.rs
- description: SMART v1 (.read) - read the AllergyIntolerance resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.read
- description: SMART v2 (.rs) - read and search the AllergyIntolerance resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.rs
- description: SMART v1 (.read) - read the Binary resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Binary.read
- description: SMART v2 (.rs) - read and search the Binary resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Binary.rs
- description: SMART v1 (.read) - read the CarePlan resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/CarePlan.read
- description: SMART v2 (.rs) - read and search the CarePlan resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/CarePlan.rs
- description: SMART v1 (.read) - read the CareTeam resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/CareTeam.read
- description: SMART v2 (.rs) - read and search the CareTeam resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/CareTeam.rs
- description: SMART v1 (.read) - read the Condition resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Condition.read
- description: SMART v2 (.rs) - read and search the Condition resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Condition.rs
- description: SMART v2 (.rs) - read and search the Condition resource for the signed-in Veradigm EHR user. Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern.
  flows:
  - authorizationCode
  scope: user/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern
- description: SMART v2 (.rs) - read and search the Condition resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis.
  flows:
  - authorizationCode
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis
- description: SMART v2 (.rs) - read and search the Condition resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item.
  flows:
  - authorizationCode
  scope: user/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item
- description: SMART v1 (.read) - read the Coverage resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Coverage.read
- description: SMART v2 (.rs) - read and search the Coverage resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Coverage.rs
- description: SMART v1 (.read) - read the Device resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Device.read
- description: SMART v2 (.rs) - read and search the Device resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Device.rs
- description: SMART v1 (.read) - read the DiagnosticOrder resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DiagnosticOrder.read
- description: SMART v2 (.rs) - read and search the DiagnosticOrder resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DiagnosticOrder.rs
- description: SMART v1 (.read) - read the DiagnosticReport resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.read
- description: SMART v2 (.rs) - read and search the DiagnosticReport resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.rs
- description: SMART v1 (.read) - read the DocumentReference resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DocumentReference.read
- description: SMART v2 (.rs) - read and search the DocumentReference resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/DocumentReference.rs
- description: SMART v1 (.read) - read the Encounter resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Encounter.read
- description: SMART v2 (.rs) - read and search the Encounter resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Encounter.rs
- description: SMART v1 (.read) - read the Goal resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Goal.read
- description: SMART v2 (.rs) - read and search the Goal resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Goal.rs
- description: SMART v1 (.read) - read the Group resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Group.read
- description: SMART v2 (.rs) - read and search the Group resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Group.rs
- description: SMART v1 (.read) - read the Immunization resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Immunization.read
- description: SMART v2 (.rs) - read and search the Immunization resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Immunization.rs
- description: SMART v1 (.read) - read the Location resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Location.read
- description: SMART v2 (.rs) - read and search the Location resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Location.rs
- description: SMART v1 (.read) - read the Medication resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Medication.read
- description: SMART v2 (.rs) - read and search the Medication resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Medication.rs
- description: SMART v1 (.read) - read the MedicationAdministration resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationAdministration.read
- description: SMART v2 (.rs) - read and search the MedicationAdministration resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationAdministration.rs
- description: SMART v1 (.read) - read the MedicationDispense resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationDispense.read
- description: SMART v2 (.rs) - read and search the MedicationDispense resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationDispense.rs
- description: SMART v1 (.read) - read the MedicationOrder resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationOrder.read
- description: SMART v2 (.rs) - read and search the MedicationOrder resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationOrder.rs
- description: SMART v1 (.read) - read the MedicationRequest resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationRequest.read
- description: SMART v2 (.rs) - read and search the MedicationRequest resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationRequest.rs
- description: SMART v1 (.read) - read the MedicationStatement resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationStatement.read
- description: SMART v2 (.rs) - read and search the MedicationStatement resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/MedicationStatement.rs
- description: SMART v1 (.read) - read the Observation resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Observation.read
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Observation.rs
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user. Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh.
  flows:
  - authorizationCode
  scope: user/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory.
  flows:
  - authorizationCode
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|social-history.
  flows:
  - authorizationCode
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|survey.
  flows:
  - authorizationCode
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey
- description: SMART v2 (.rs) - read and search the Observation resource for the signed-in Veradigm EHR user. Restricted to category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs.
  flows:
  - authorizationCode
  scope: user/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs
- description: SMART v1 (.read) - read the Organization resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Organization.read
- description: SMART v2 (.rs) - read and search the Organization resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Organization.rs
- description: SMART v1 (.read) - read the Patient resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Patient.read
- description: SMART v2 (.rs) - read and search the Patient resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Patient.rs
- description: SMART v1 (.read) - read the Practitioner resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Practitioner.read
- description: SMART v2 (.rs) - read and search the Practitioner resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Practitioner.rs
- description: SMART v1 (.read) - read the PractitionerRole resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/PractitionerRole.read
- description: SMART v2 (.rs) - read and search the PractitionerRole resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/PractitionerRole.rs
- description: SMART v1 (.read) - read the Procedure resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Procedure.read
- description: SMART v2 (.rs) - read and search the Procedure resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Procedure.rs
- description: SMART v1 (.read) - read the Provenance resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Provenance.read
- description: SMART v2 (.rs) - read and search the Provenance resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Provenance.rs
- description: SMART v1 (.read) - read the Questionnaire resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Questionnaire.read
- description: SMART v2 (.rs) - read and search the Questionnaire resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Questionnaire.rs
- description: SMART v1 (.read) - read the QuestionnaireResponse resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/QuestionnaireResponse.read
- description: SMART v2 (.rs) - read and search the QuestionnaireResponse resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/QuestionnaireResponse.rs
- description: SMART v1 (.read) - read the RelatedPerson resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/RelatedPerson.read
- description: SMART v2 (.rs) - read and search the RelatedPerson resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/RelatedPerson.rs
- description: SMART v1 (.read) - read the ServiceRequest resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/ServiceRequest.read
- description: SMART v2 (.rs) - read and search the ServiceRequest resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/ServiceRequest.rs
- description: SMART v1 (.read) - read the Specimen resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Specimen.read
- description: SMART v2 (.rs) - read and search the Specimen resource for the signed-in Veradigm EHR user.
  flows:
  - authorizationCode
  scope: user/Specimen.rs
slug: allscripts-healthcare-solutions-scopes
source_filename: allscripts-healthcare-solutions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://fhir.fhirpoint.open.allscripts.com/fhirroute/fhir/CP00101/.well-known/smart-configuration\ndocs: https://developer.veradigm.com/Fhir/ProcessOverview\ndescription: OAuth 2.0 / SMART App Launch scopes advertised by the Veradigm (formerly Allscripts) FHIR\n  authorization server. Read verbatim from the scopes_supported array of the live SMART configuration\n  document served on the published Veradigm EHR R4 sandbox base URL, and cross-checked against the identical\n  scopes_supported array in the OpenID Connect discovery document on the issuer. Nothing here is inferred\n  - the descriptions restate the SMART App Launch v1/v2 semantics of the scope strings the server itself\n  publishes. Veradigm's Process Overview page states that a registered FHIR application may use SMART\n  v1 (.read) scopes or SMART v2 (.rs) scopes but never both; an application requesting both is not approved.\nschemes:\n- name: SMART on FHIR (OAuth\
  \ 2.0 + OpenID Connect)\n  source: well-known/allscripts-healthcare-solutions-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize\n    tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n    note: SMART Backend Services. Only FHIR applications registered with App Type \"System\" may use client_credentials;\n      the developer registers a JWKS URL and the server authenticates a private_key_jwt assertion against\n      it.\n  issuer: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization\n  jwks_uri: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration/jwks\nsummary:\n  scope_count: 237\n  by_context:\n    openid-connect:\
  \ 8\n    patient: 76\n    system: 76\n    user: 77\n  smart_versions:\n  - v1 (.read)\n  - v2 (.rs)\n  note: Veradigm does not allow SMART v1 and SMART v2 scopes on the same registered application.\nscopes:\n- scope: fhir\n  context: openid-connect\n  description: Veradigm scope granting FHIR API access.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: fhirUser\n  context: openid-connect\n  description: SMART - return the FHIR resource representing the current user.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: launch\n  context: openid-connect\n  description: SMART - request the full EHR launch context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: launch/patient\n  context: openid-connect\n  description: SMART - request the patient launch context\
  \ in a standalone launch.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: offline_access\n  context: openid-connect\n  description: Request a refresh token that survives the end of the session.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: online_access\n  context: openid-connect\n  description: Request a refresh token valid only while the user session is live.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: openid\n  context: openid-connect\n  description: OpenID Connect - request an ID token.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/*.read\n  context: patient\n  description: SMART v1 (.read) - read every supported resource for the patient in context.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/*.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search every supported resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/AllergyIntolerance.read\n  context: patient\n  description: SMART v1 (.read) - read the AllergyIntolerance resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/AllergyIntolerance.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the AllergyIntolerance resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Binary.read\n  context: patient\n\
  \  description: SMART v1 (.read) - read the Binary resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Binary.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Binary resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/CarePlan.read\n  context: patient\n  description: SMART v1 (.read) - read the CarePlan resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/CarePlan.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the CarePlan resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope:\
  \ patient/CareTeam.read\n  context: patient\n  description: SMART v1 (.read) - read the CareTeam resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/CareTeam.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the CareTeam resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Condition.read\n  context: patient\n  description: SMART v1 (.read) - read the Condition resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Condition.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Condition resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  context: patient\n  description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted\n    to category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  context: patient\n  description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n\
  \  context: patient\n  description: SMART v2 (.rs) - read and search the Condition resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Coverage.read\n  context: patient\n  description: SMART v1 (.read) - read the Coverage resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Coverage.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Coverage resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Device.read\n  context: patient\n  description: SMART v1 (.read) - read the Device resource for the patient in context.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Device.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Device resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DiagnosticOrder.read\n  context: patient\n  description: SMART v1 (.read) - read the DiagnosticOrder resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DiagnosticOrder.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the DiagnosticOrder resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DiagnosticReport.read\n  context: patient\n  description:\
  \ SMART v1 (.read) - read the DiagnosticReport resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DiagnosticReport.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the DiagnosticReport resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DocumentReference.read\n  context: patient\n  description: SMART v1 (.read) - read the DocumentReference resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/DocumentReference.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the DocumentReference resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/Encounter.read\n  context: patient\n  description: SMART v1 (.read) - read the Encounter resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Encounter.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Encounter resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Goal.read\n  context: patient\n  description: SMART v1 (.read) - read the Goal resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Goal.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Goal resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/Group.read\n  context: patient\n  description: SMART v1 (.read) - read the Group resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Group.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Group resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Immunization.read\n  context: patient\n  description: SMART v1 (.read) - read the Immunization resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Immunization.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Immunization resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/Location.read\n  context: patient\n  description: SMART v1 (.read) - read the Location resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Location.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Location resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Medication.read\n  context: patient\n  description: SMART v1 (.read) - read the Medication resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Medication.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Medication resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/MedicationAdministration.read\n  context: patient\n  description: SMART v1 (.read) - read the MedicationAdministration resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationAdministration.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the MedicationAdministration resource for the patient\n    in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationDispense.read\n  context: patient\n  description: SMART v1 (.read) - read the MedicationDispense resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationDispense.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the MedicationDispense\
  \ resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationOrder.read\n  context: patient\n  description: SMART v1 (.read) - read the MedicationOrder resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationOrder.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the MedicationOrder resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationRequest.read\n  context: patient\n  description: SMART v1 (.read) - read the MedicationRequest resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope:\
  \ patient/MedicationRequest.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the MedicationRequest resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationStatement.read\n  context: patient\n  description: SMART v1 (.read) - read the MedicationStatement resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/MedicationStatement.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the MedicationStatement resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.read\n  context: patient\n  description: SMART v1 (.read) - read the Observation resource for the patient in context.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted\n    to category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation\
  \ resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/observation-category|social-history.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|survey\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/observation-category|survey.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Observation.rs?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Observation resource for the patient in context. Restricted\n    to category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Organization.read\n  context: patient\n  description: SMART v1 (.read) - read the Organization resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Organization.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Organization resource for the patient in context.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Patient.read\n  context: patient\n  description: SMART v1 (.read) - read the Patient resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Patient.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Patient resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Practitioner.read\n  context: patient\n  description: SMART v1 (.read) - read the Practitioner resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Practitioner.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search\
  \ the Practitioner resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/PractitionerRole.read\n  context: patient\n  description: SMART v1 (.read) - read the PractitionerRole resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/PractitionerRole.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the PractitionerRole resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Procedure.read\n  context: patient\n  description: SMART v1 (.read) - read the Procedure resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope:\
  \ patient/Procedure.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Procedure resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Provenance.read\n  context: patient\n  description: SMART v1 (.read) - read the Provenance resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Provenance.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Provenance resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Questionnaire.read\n  context: patient\n  description: SMART v1 (.read) - read the Questionnaire resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: patient/Questionnaire.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Questionnaire resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/QuestionnaireResponse.read\n  context: patient\n  description: SMART v1 (.read) - read the QuestionnaireResponse resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/QuestionnaireResponse.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the QuestionnaireResponse resource for the patient in\n    context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/RelatedPerson.read\n  context: patient\n  description: SMART v1 (.read) - read the RelatedPerson resource for the patient\
  \ in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/RelatedPerson.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the RelatedPerson resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/ServiceRequest.read\n  context: patient\n  description: SMART v1 (.read) - read the ServiceRequest resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/ServiceRequest.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the ServiceRequest resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Specimen.read\n  context:\
  \ patient\n  description: SMART v1 (.read) - read the Specimen resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: patient/Specimen.rs\n  context: patient\n  description: SMART v2 (.rs) - read and search the Specimen resource for the patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: profile\n  context: openid-connect\n  description: OpenID Connect - request the profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/*.read\n  context: system\n  description: SMART v1 (.read) - read every supported resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/*.rs\n\
  \  context: system\n  description: SMART v2 (.rs) - read and search every supported resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/AllergyIntolerance.read\n  context: system\n  description: SMART v1 (.read) - read the AllergyIntolerance resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/AllergyIntolerance.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the AllergyIntolerance resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Binary.read\n  context: system\n  description: SMART v1 (.read) - read the Binary resource for a backend System application\
  \ (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Binary.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the Binary resource for a backend System application (no\n    user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/CarePlan.read\n  context: system\n  description: SMART v1 (.read) - read the CarePlan resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/CarePlan.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the CarePlan resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/CareTeam.read\n\
  \  context: system\n  description: SMART v1 (.read) - read the CareTeam resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/CareTeam.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the CareTeam resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Condition.read\n  context: system\n  description: SMART v1 (.read) - read the Condition resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Condition.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the Condition resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Condition.rs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  context: system\n  description: SMART v2 (.rs) - read and search the Condition resource for a backend System application\n    (no user). Restricted to category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern.\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  context: system\n  description: SMART v2 (.rs) - read and search the Condition resource for a backend System application\n    (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis.\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: system/Condition.rs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n  context: system\n  description: SMART v2 (.rs) - read and search the Condition resource for a backend System application\n    (no user). Restricted to category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item.\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Coverage.read\n  context: system\n  description: SMART v1 (.read) - read the Coverage resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Coverage.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the Coverage resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: system/Device.read\n  context: system\n  description: SMART v1 (.read) - read the Device resource for a backend System application (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/Device.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the Device resource for a backend System application (no\n    user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/DiagnosticOrder.read\n  context: system\n  description: SMART v1 (.read) - read the DiagnosticOrder resource for a backend System application (no\n    user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/DiagnosticOrder.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the DiagnosticOrder resource for a backend System application\n\
  \    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/DiagnosticReport.read\n  context: system\n  description: SMART v1 (.read) - read the DiagnosticReport resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/DiagnosticReport.rs\n  context: system\n  description: SMART v2 (.rs) - read and search the DiagnosticReport resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n- scope: system/DocumentReference.read\n  context: system\n  description: SMART v1 (.read) - read the DocumentReference resource for a backend System application\n    (no user).\n  flows:\n  - clientCredentials\n  sources:\n  - well-known/allscripts-healthcare-solutions-smart-configuration.json\n\
  - scope: system/DocumentReference.r\n\n# --- truncated at 32 KB (68 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/allscripts-healthcare-solutions/refs/heads/main/scopes/allscripts-healthcare-solutions-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts-healthcare-solutions/refs/heads/main/scopes/allscripts-healthcare-solutions-scopes.yml
summary_line: 237 scopes · authorizationCode/clientCredentials
tags:
- Healthcare IT
- EHR
- Clinical
- FHIR
- HL7
- SMART on FHIR
- USCDI
- Interoperability
- Patient Access
- 21st Century Cures
- Veradigm
token_urls:
- https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token
---
