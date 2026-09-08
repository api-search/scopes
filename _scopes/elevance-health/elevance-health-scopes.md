---
api_specs:
- filename: elevance-health-claims-api-openapi.yml
  format: yaml
  label: Elevance Health Claims API
  slug: elevance-health-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-claims-api-openapi.yml
- filename: elevance-health-conformance-api-openapi.yml
  format: yaml
  label: Elevance Health Conformance API
  slug: elevance-health-conformance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-conformance-api-openapi.yml
- filename: elevance-health-coverage-api-openapi.yml
  format: yaml
  label: Elevance Health Coverage API
  slug: elevance-health-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-coverage-api-openapi.yml
- filename: elevance-health-patient-api-openapi.yml
  format: yaml
  label: Elevance Health Patient API
  slug: elevance-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-patient-api-openapi.yml
- filename: elevance-health-provider-directory-api-openapi.yml
  format: yaml
  label: Elevance Health Provider Directory API
  slug: elevance-health-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-provider-directory-api-openapi.yml
authorization_urls:
- https://totalview.healthos.elevancehealth.com/oauth2.code/registered/api/v1/authorize
- https://patient360.anthem.com/P360Member/identityserver/connect/authorize
description: OAuth 2.0 / SMART on FHIR scopes actually advertised by Elevance Health, read from the providers own discovery documents rather than inferred. Supersedes the 2026-07-11 derived file, which listed three scopes taken from a hand-written scaffold spec.
docs: https://patient360c.anthem.com/P360Member/fhir/documentation
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Elevance Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Elevance Health publishes 272 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Elevance Health API on a user''s behalf.


  Tokens are issued from https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Elevance Health
provider_slug: elevance-health
schemes:
- api: Patient Access API (production, FHIR R4)
  flows:
  - authorizationUrl: https://totalview.healthos.elevancehealth.com/oauth2.code/registered/api/v1/authorize
    flow: authorizationCode
    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token
  - flow: clientCredentials
    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token
  name: totalview-patient-access
  source: well-known/elevance-health-totalview-smart-configuration.json
- api: Patient360 FHIR (DSTU2)
  flows:
  - authorizationUrl: https://patient360.anthem.com/P360Member/identityserver/connect/authorize
    flow: authorizationCode
    tokenUrl: https://patient360.anthem.com/P360Member/identityserver/connect/token
  name: patient360-smart
  source: well-known/elevance-health-patient360-smart-configuration.json
- api: Provider Directory API and Formulary API
  flows:
  - flow: clientCredentials
    note: Token endpoint issued per registered application by secure email; not published.
    tokenUrl: null
  name: provider-directory-and-formulary
  source: https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf
scope_count: 272
scope_names:
- patient/AllergyIntolerance.*
- patient/AllergyIntolerance.read
- patient/AuditEvent.*
- patient/AuditEvent.read
- patient/Basic.*
- patient/Basic.read
- patient/Binary.*
- patient/Binary.read
- patient/CarePlan.*
- patient/CarePlan.read
- patient/CareTeam.*
- patient/CareTeam.read
- patient/Claim.*
- patient/Claim.read
- patient/Condition.*
- patient/Condition.read
- patient/Coverage.*
- patient/Coverage.read
- patient/Device.*
- patient/Device.read
- patient/DiagnosticReport.*
- patient/DiagnosticReport.read
- patient/DocumentReference.*
- patient/DocumentReference.read
- patient/Encounter.*
- patient/Encounter.read
- patient/ExplanationOfBenefit.*
- patient/ExplanationOfBenefit.read
- patient/Goal.*
- patient/Goal.read
- patient/Immunization.*
- patient/Immunization.read
- patient/Location.*
- patient/Location.read
- patient/MedicationDispense.*
- patient/MedicationDispense.read
- patient/MedicationRequest.*
- patient/MedicationRequest.read
- patient/Observation.*
- patient/Observation.read
- patient/Organization.*
- patient/Organization.read
- patient/Patient.*
- patient/Patient.read
- patient/Practitioner.*
- patient/Practitioner.read
- patient/Procedure.*
- patient/Procedure.read
- patient/Provenance.*
- patient/Provenance.read
- patient/QuestionnaireResponse.*
- patient/QuestionnaireResponse.read
- patient/RelatedPerson.*
- patient/RelatedPerson.read
- patient/ServiceRequest.*
- patient/ServiceRequest.read
- patient/Specimen.*
- patient/Specimen.read
- patient/*.*
- patient/*.read
- launch
- launch/patient
- openid
- profile
- fhirUser
- offline_access
- online_access
- patient/AllergyIntolerance.*
- patient/AllergyIntolerance.read
- patient/AuditEvent.*
- patient/AuditEvent.read
- patient/Binary.*
- patient/Binary.read
- patient/CarePlan.*
- patient/CarePlan.read
- patient/Claim.*
- patient/Claim.read
- patient/Condition.*
- patient/Condition.read
- patient/Coverage.*
- patient/Coverage.read
- patient/Device.*
- patient/Device.read
- patient/DiagnosticOrder.*
- patient/DiagnosticOrder.read
- patient/DiagnosticReport.*
- patient/DiagnosticReport.read
- patient/Encounter.*
- patient/Encounter.read
- patient/Goal.*
- patient/Goal.read
- patient/Group.*
- patient/Group.read
- patient/Immunization.*
- patient/Immunization.read
- patient/Location.*
- patient/Location.read
- patient/MedicationAdministration.*
- patient/MedicationAdministration.read
- patient/MedicationDispense.*
- patient/MedicationDispense.read
- patient/MedicationOrder.*
- patient/MedicationOrder.read
- patient/MedicationStatement.*
- patient/MedicationStatement.read
- patient/Observation.*
- patient/Observation.read
- patient/OperationDefinition.*
- patient/OperationDefinition.read
- patient/Organization.*
- patient/Organization.read
- patient/Patient.*
- patient/Patient.read
- patient/Person.*
- patient/Person.read
- patient/Practitioner.*
- patient/Practitioner.read
- patient/Procedure.*
- patient/Procedure.read
- patient/ProcedureRequest.*
- patient/ProcedureRequest.read
- patient/Provenance.*
- patient/Provenance.read
- patient/ReferralRequest.*
- patient/ReferralRequest.read
- patient/RelatedPerson.*
- patient/RelatedPerson.read
- patient/Specimen.*
- patient/Specimen.read
- patient/ValueSet.*
- patient/ValueSet.read
- patient/*.*
- patient/*.read
- user/AllergyIntolerance.*
- user/AllergyIntolerance.read
- user/AuditEvent.*
- user/AuditEvent.read
- user/Binary.*
- user/Binary.read
- user/CarePlan.*
- user/CarePlan.read
- user/Claim.*
- user/Claim.read
- user/Condition.*
- user/Condition.read
- user/Coverage.*
- user/Coverage.read
- user/Device.*
- user/Device.read
- user/DiagnosticOrder.*
- user/DiagnosticOrder.read
- user/DiagnosticReport.*
- user/DiagnosticReport.read
- user/Encounter.*
- user/Encounter.read
- user/Goal.*
- user/Goal.read
- user/Group.*
- user/Group.read
- user/Immunization.*
- user/Immunization.read
- user/Location.*
- user/Location.read
- user/MedicationAdministration.*
- user/MedicationAdministration.read
- user/MedicationDispense.*
- user/MedicationDispense.read
- user/MedicationOrder.*
- user/MedicationOrder.read
- user/MedicationStatement.*
- user/MedicationStatement.read
- user/Observation.*
- user/Observation.read
- user/OperationDefinition.*
- user/OperationDefinition.read
- user/Organization.*
- user/Organization.read
- user/Patient.*
- user/Patient.read
- user/Person.*
- user/Person.read
- user/Practitioner.*
- user/Practitioner.read
- user/Procedure.*
- user/Procedure.read
- user/ProcedureRequest.*
- user/ProcedureRequest.read
- user/Provenance.*
- user/Provenance.read
- user/ReferralRequest.*
- user/ReferralRequest.read
- user/RelatedPerson.*
- user/RelatedPerson.read
- user/Specimen.*
- user/Specimen.read
- user/ValueSet.*
- user/ValueSet.read
- user/*.*
- user/*.read
- system/AllergyIntolerance.*
- system/AllergyIntolerance.read
- system/AuditEvent.*
- system/AuditEvent.read
- system/Binary.*
- system/Binary.read
- system/CarePlan.*
- system/CarePlan.read
- system/Claim.*
- system/Claim.read
- system/Condition.*
- system/Condition.read
- system/Coverage.*
- system/Coverage.read
- system/Device.*
- system/Device.read
- system/DiagnosticOrder.*
- system/DiagnosticOrder.read
- system/DiagnosticReport.*
- system/DiagnosticReport.read
- system/Encounter.*
- system/Encounter.read
- system/Goal.*
- system/Goal.read
- system/Group.*
- system/Group.read
- system/Immunization.*
- system/Immunization.read
- system/Location.*
- system/Location.read
- system/MedicationAdministration.*
- system/MedicationAdministration.read
- system/MedicationDispense.*
- system/MedicationDispense.read
- system/MedicationOrder.*
- system/MedicationOrder.read
- system/MedicationStatement.*
- system/MedicationStatement.read
- system/Observation.*
- system/Observation.read
- system/OperationDefinition.*
- system/OperationDefinition.read
- system/Organization.*
- system/Organization.read
- system/Patient.*
- system/Patient.read
- system/Person.*
- system/Person.read
- system/Practitioner.*
- system/Practitioner.read
- system/Procedure.*
- system/Procedure.read
- system/ProcedureRequest.*
- system/ProcedureRequest.read
- system/Provenance.*
- system/Provenance.read
- system/ReferralRequest.*
- system/ReferralRequest.read
- system/RelatedPerson.*
- system/RelatedPerson.read
- system/Specimen.*
- system/Specimen.read
- system/ValueSet.*
- system/ValueSet.read
- system/*.*
- system/*.read
- launch
- launch/patient
- openid
- profile
- fhirUser
- offline_access
- online_access
scopes:
- description: patient-scoped read and write access to AllergyIntolerance resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/AllergyIntolerance.*
- description: patient-scoped read access to AllergyIntolerance resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/AllergyIntolerance.read
- description: patient-scoped read and write access to AuditEvent resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/AuditEvent.*
- description: patient-scoped read access to AuditEvent resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/AuditEvent.read
- description: patient-scoped read and write access to Basic resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Basic.*
- description: patient-scoped read access to Basic resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Basic.read
- description: patient-scoped read and write access to Binary resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Binary.*
- description: patient-scoped read access to Binary resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Binary.read
- description: patient-scoped read and write access to CarePlan resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/CarePlan.*
- description: patient-scoped read access to CarePlan resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/CarePlan.read
- description: patient-scoped read and write access to CareTeam resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/CareTeam.*
- description: patient-scoped read access to CareTeam resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/CareTeam.read
- description: patient-scoped read and write access to Claim resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Claim.*
- description: patient-scoped read access to Claim resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Claim.read
- description: patient-scoped read and write access to Condition resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Condition.*
- description: patient-scoped read access to Condition resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Condition.read
- description: patient-scoped read and write access to Coverage resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Coverage.*
- description: patient-scoped read access to Coverage resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Coverage.read
- description: patient-scoped read and write access to Device resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Device.*
- description: patient-scoped read access to Device resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Device.read
- description: patient-scoped read and write access to DiagnosticReport resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/DiagnosticReport.*
- description: patient-scoped read access to DiagnosticReport resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/DiagnosticReport.read
- description: patient-scoped read and write access to DocumentReference resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/DocumentReference.*
- description: patient-scoped read access to DocumentReference resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/DocumentReference.read
- description: patient-scoped read and write access to Encounter resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Encounter.*
- description: patient-scoped read access to Encounter resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Encounter.read
- description: patient-scoped read and write access to ExplanationOfBenefit resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/ExplanationOfBenefit.*
- description: patient-scoped read access to ExplanationOfBenefit resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/ExplanationOfBenefit.read
- description: patient-scoped read and write access to Goal resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Goal.*
- description: patient-scoped read access to Goal resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Goal.read
- description: patient-scoped read and write access to Immunization resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Immunization.*
- description: patient-scoped read access to Immunization resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Immunization.read
- description: patient-scoped read and write access to Location resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Location.*
- description: patient-scoped read access to Location resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Location.read
- description: patient-scoped read and write access to MedicationDispense resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/MedicationDispense.*
- description: patient-scoped read access to MedicationDispense resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/MedicationDispense.read
- description: patient-scoped read and write access to MedicationRequest resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/MedicationRequest.*
- description: patient-scoped read access to MedicationRequest resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/MedicationRequest.read
- description: patient-scoped read and write access to Observation resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Observation.*
- description: patient-scoped read access to Observation resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Observation.read
- description: patient-scoped read and write access to Organization resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Organization.*
- description: patient-scoped read access to Organization resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Organization.read
- description: patient-scoped read and write access to Patient resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Patient.*
- description: patient-scoped read access to Patient resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Patient.read
- description: patient-scoped read and write access to Practitioner resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Practitioner.*
- description: patient-scoped read access to Practitioner resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Practitioner.read
- description: patient-scoped read and write access to Procedure resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Procedure.*
- description: patient-scoped read access to Procedure resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Procedure.read
- description: patient-scoped read and write access to Provenance resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Provenance.*
- description: patient-scoped read access to Provenance resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Provenance.read
- description: patient-scoped read and write access to QuestionnaireResponse resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/QuestionnaireResponse.*
- description: patient-scoped read access to QuestionnaireResponse resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/QuestionnaireResponse.read
- description: patient-scoped read and write access to RelatedPerson resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/RelatedPerson.*
- description: patient-scoped read access to RelatedPerson resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/RelatedPerson.read
- description: patient-scoped read and write access to ServiceRequest resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/ServiceRequest.*
- description: patient-scoped read access to ServiceRequest resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/ServiceRequest.read
- description: patient-scoped read and write access to Specimen resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Specimen.*
- description: patient-scoped read access to Specimen resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/Specimen.read
- description: patient-scoped read and write access to all resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/*.*
- description: patient-scoped read access to all resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: patient/*.read
- description: SMART EHR launch context
  flows:
  - authorizationCode
  - clientCredentials
  scope: launch
- description: SMART standalone patient launch context
  flows:
  - authorizationCode
  - clientCredentials
  scope: launch/patient
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: Basic profile claims
  flows:
  - authorizationCode
  - clientCredentials
  scope: profile
- description: Identity of the authorizing FHIR user
  flows:
  - authorizationCode
  - clientCredentials
  scope: fhirUser
- description: Refresh token / offline access
  flows:
  - authorizationCode
  - clientCredentials
  scope: offline_access
- description: Refresh token valid only while the user is online
  flows:
  - authorizationCode
  - clientCredentials
  scope: online_access
- description: patient-scoped read and write access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.*
- description: patient-scoped read access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: patient-scoped read and write access to AuditEvent resources
  flows:
  - authorizationCode
  scope: patient/AuditEvent.*
- description: patient-scoped read access to AuditEvent resources
  flows:
  - authorizationCode
  scope: patient/AuditEvent.read
- description: patient-scoped read and write access to Binary resources
  flows:
  - authorizationCode
  scope: patient/Binary.*
- description: patient-scoped read access to Binary resources
  flows:
  - authorizationCode
  scope: patient/Binary.read
- description: patient-scoped read and write access to CarePlan resources
  flows:
  - authorizationCode
  scope: patient/CarePlan.*
- description: patient-scoped read access to CarePlan resources
  flows:
  - authorizationCode
  scope: patient/CarePlan.read
- description: patient-scoped read and write access to Claim resources
  flows:
  - authorizationCode
  scope: patient/Claim.*
- description: patient-scoped read access to Claim resources
  flows:
  - authorizationCode
  scope: patient/Claim.read
- description: patient-scoped read and write access to Condition resources
  flows:
  - authorizationCode
  scope: patient/Condition.*
- description: patient-scoped read access to Condition resources
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: patient-scoped read and write access to Coverage resources
  flows:
  - authorizationCode
  scope: patient/Coverage.*
- description: patient-scoped read access to Coverage resources
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: patient-scoped read and write access to Device resources
  flows:
  - authorizationCode
  scope: patient/Device.*
- description: patient-scoped read access to Device resources
  flows:
  - authorizationCode
  scope: patient/Device.read
- description: patient-scoped read and write access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: patient/DiagnosticOrder.*
- description: patient-scoped read access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: patient/DiagnosticOrder.read
- description: patient-scoped read and write access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.*
- description: patient-scoped read access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.read
- description: patient-scoped read and write access to Encounter resources
  flows:
  - authorizationCode
  scope: patient/Encounter.*
- description: patient-scoped read access to Encounter resources
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: patient-scoped read and write access to Goal resources
  flows:
  - authorizationCode
  scope: patient/Goal.*
- description: patient-scoped read access to Goal resources
  flows:
  - authorizationCode
  scope: patient/Goal.read
- description: patient-scoped read and write access to Group resources
  flows:
  - authorizationCode
  scope: patient/Group.*
- description: patient-scoped read access to Group resources
  flows:
  - authorizationCode
  scope: patient/Group.read
- description: patient-scoped read and write access to Immunization resources
  flows:
  - authorizationCode
  scope: patient/Immunization.*
- description: patient-scoped read access to Immunization resources
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: patient-scoped read and write access to Location resources
  flows:
  - authorizationCode
  scope: patient/Location.*
- description: patient-scoped read access to Location resources
  flows:
  - authorizationCode
  scope: patient/Location.read
- description: patient-scoped read and write access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: patient/MedicationAdministration.*
- description: patient-scoped read access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: patient/MedicationAdministration.read
- description: patient-scoped read and write access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.*
- description: patient-scoped read access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.read
- description: patient-scoped read and write access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: patient/MedicationOrder.*
- description: patient-scoped read access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: patient/MedicationOrder.read
- description: patient-scoped read and write access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: patient/MedicationStatement.*
- description: patient-scoped read access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: patient/MedicationStatement.read
- description: patient-scoped read and write access to Observation resources
  flows:
  - authorizationCode
  scope: patient/Observation.*
- description: patient-scoped read access to Observation resources
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: patient-scoped read and write access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: patient/OperationDefinition.*
- description: patient-scoped read access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: patient/OperationDefinition.read
- description: patient-scoped read and write access to Organization resources
  flows:
  - authorizationCode
  scope: patient/Organization.*
- description: patient-scoped read access to Organization resources
  flows:
  - authorizationCode
  scope: patient/Organization.read
- description: patient-scoped read and write access to Patient resources
  flows:
  - authorizationCode
  scope: patient/Patient.*
- description: patient-scoped read access to Patient resources
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: patient-scoped read and write access to Person resources
  flows:
  - authorizationCode
  scope: patient/Person.*
- description: patient-scoped read access to Person resources
  flows:
  - authorizationCode
  scope: patient/Person.read
- description: patient-scoped read and write access to Practitioner resources
  flows:
  - authorizationCode
  scope: patient/Practitioner.*
- description: patient-scoped read access to Practitioner resources
  flows:
  - authorizationCode
  scope: patient/Practitioner.read
- description: patient-scoped read and write access to Procedure resources
  flows:
  - authorizationCode
  scope: patient/Procedure.*
- description: patient-scoped read access to Procedure resources
  flows:
  - authorizationCode
  scope: patient/Procedure.read
- description: patient-scoped read and write access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: patient/ProcedureRequest.*
- description: patient-scoped read access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: patient/ProcedureRequest.read
- description: patient-scoped read and write access to Provenance resources
  flows:
  - authorizationCode
  scope: patient/Provenance.*
- description: patient-scoped read access to Provenance resources
  flows:
  - authorizationCode
  scope: patient/Provenance.read
- description: patient-scoped read and write access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: patient/ReferralRequest.*
- description: patient-scoped read access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: patient/ReferralRequest.read
- description: patient-scoped read and write access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.*
- description: patient-scoped read access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.read
- description: patient-scoped read and write access to Specimen resources
  flows:
  - authorizationCode
  scope: patient/Specimen.*
- description: patient-scoped read access to Specimen resources
  flows:
  - authorizationCode
  scope: patient/Specimen.read
- description: patient-scoped read and write access to ValueSet resources
  flows:
  - authorizationCode
  scope: patient/ValueSet.*
- description: patient-scoped read access to ValueSet resources
  flows:
  - authorizationCode
  scope: patient/ValueSet.read
- description: patient-scoped read and write access to all resources
  flows:
  - authorizationCode
  scope: patient/*.*
- description: patient-scoped read access to all resources
  flows:
  - authorizationCode
  scope: patient/*.read
- description: user-scoped read and write access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.*
- description: user-scoped read access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.read
- description: user-scoped read and write access to AuditEvent resources
  flows:
  - authorizationCode
  scope: user/AuditEvent.*
- description: user-scoped read access to AuditEvent resources
  flows:
  - authorizationCode
  scope: user/AuditEvent.read
- description: user-scoped read and write access to Binary resources
  flows:
  - authorizationCode
  scope: user/Binary.*
- description: user-scoped read access to Binary resources
  flows:
  - authorizationCode
  scope: user/Binary.read
- description: user-scoped read and write access to CarePlan resources
  flows:
  - authorizationCode
  scope: user/CarePlan.*
- description: user-scoped read access to CarePlan resources
  flows:
  - authorizationCode
  scope: user/CarePlan.read
- description: user-scoped read and write access to Claim resources
  flows:
  - authorizationCode
  scope: user/Claim.*
- description: user-scoped read access to Claim resources
  flows:
  - authorizationCode
  scope: user/Claim.read
- description: user-scoped read and write access to Condition resources
  flows:
  - authorizationCode
  scope: user/Condition.*
- description: user-scoped read access to Condition resources
  flows:
  - authorizationCode
  scope: user/Condition.read
- description: user-scoped read and write access to Coverage resources
  flows:
  - authorizationCode
  scope: user/Coverage.*
- description: user-scoped read access to Coverage resources
  flows:
  - authorizationCode
  scope: user/Coverage.read
- description: user-scoped read and write access to Device resources
  flows:
  - authorizationCode
  scope: user/Device.*
- description: user-scoped read access to Device resources
  flows:
  - authorizationCode
  scope: user/Device.read
- description: user-scoped read and write access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: user/DiagnosticOrder.*
- description: user-scoped read access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: user/DiagnosticOrder.read
- description: user-scoped read and write access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.*
- description: user-scoped read access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.read
- description: user-scoped read and write access to Encounter resources
  flows:
  - authorizationCode
  scope: user/Encounter.*
- description: user-scoped read access to Encounter resources
  flows:
  - authorizationCode
  scope: user/Encounter.read
- description: user-scoped read and write access to Goal resources
  flows:
  - authorizationCode
  scope: user/Goal.*
- description: user-scoped read access to Goal resources
  flows:
  - authorizationCode
  scope: user/Goal.read
- description: user-scoped read and write access to Group resources
  flows:
  - authorizationCode
  scope: user/Group.*
- description: user-scoped read access to Group resources
  flows:
  - authorizationCode
  scope: user/Group.read
- description: user-scoped read and write access to Immunization resources
  flows:
  - authorizationCode
  scope: user/Immunization.*
- description: user-scoped read access to Immunization resources
  flows:
  - authorizationCode
  scope: user/Immunization.read
- description: user-scoped read and write access to Location resources
  flows:
  - authorizationCode
  scope: user/Location.*
- description: user-scoped read access to Location resources
  flows:
  - authorizationCode
  scope: user/Location.read
- description: user-scoped read and write access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: user/MedicationAdministration.*
- description: user-scoped read access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: user/MedicationAdministration.read
- description: user-scoped read and write access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: user/MedicationDispense.*
- description: user-scoped read access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: user/MedicationDispense.read
- description: user-scoped read and write access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: user/MedicationOrder.*
- description: user-scoped read access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: user/MedicationOrder.read
- description: user-scoped read and write access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: user/MedicationStatement.*
- description: user-scoped read access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: user/MedicationStatement.read
- description: user-scoped read and write access to Observation resources
  flows:
  - authorizationCode
  scope: user/Observation.*
- description: user-scoped read access to Observation resources
  flows:
  - authorizationCode
  scope: user/Observation.read
- description: user-scoped read and write access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: user/OperationDefinition.*
- description: user-scoped read access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: user/OperationDefinition.read
- description: user-scoped read and write access to Organization resources
  flows:
  - authorizationCode
  scope: user/Organization.*
- description: user-scoped read access to Organization resources
  flows:
  - authorizationCode
  scope: user/Organization.read
- description: user-scoped read and write access to Patient resources
  flows:
  - authorizationCode
  scope: user/Patient.*
- description: user-scoped read access to Patient resources
  flows:
  - authorizationCode
  scope: user/Patient.read
- description: user-scoped read and write access to Person resources
  flows:
  - authorizationCode
  scope: user/Person.*
- description: user-scoped read access to Person resources
  flows:
  - authorizationCode
  scope: user/Person.read
- description: user-scoped read and write access to Practitioner resources
  flows:
  - authorizationCode
  scope: user/Practitioner.*
- description: user-scoped read access to Practitioner resources
  flows:
  - authorizationCode
  scope: user/Practitioner.read
- description: user-scoped read and write access to Procedure resources
  flows:
  - authorizationCode
  scope: user/Procedure.*
- description: user-scoped read access to Procedure resources
  flows:
  - authorizationCode
  scope: user/Procedure.read
- description: user-scoped read and write access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: user/ProcedureRequest.*
- description: user-scoped read access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: user/ProcedureRequest.read
- description: user-scoped read and write access to Provenance resources
  flows:
  - authorizationCode
  scope: user/Provenance.*
- description: user-scoped read access to Provenance resources
  flows:
  - authorizationCode
  scope: user/Provenance.read
- description: user-scoped read and write access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: user/ReferralRequest.*
- description: user-scoped read access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: user/ReferralRequest.read
- description: user-scoped read and write access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: user/RelatedPerson.*
- description: user-scoped read access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: user/RelatedPerson.read
- description: user-scoped read and write access to Specimen resources
  flows:
  - authorizationCode
  scope: user/Specimen.*
- description: user-scoped read access to Specimen resources
  flows:
  - authorizationCode
  scope: user/Specimen.read
- description: user-scoped read and write access to ValueSet resources
  flows:
  - authorizationCode
  scope: user/ValueSet.*
- description: user-scoped read access to ValueSet resources
  flows:
  - authorizationCode
  scope: user/ValueSet.read
- description: user-scoped read and write access to all resources
  flows:
  - authorizationCode
  scope: user/*.*
- description: user-scoped read access to all resources
  flows:
  - authorizationCode
  scope: user/*.read
- description: system-scoped read and write access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: system/AllergyIntolerance.*
- description: system-scoped read access to AllergyIntolerance resources
  flows:
  - authorizationCode
  scope: system/AllergyIntolerance.read
- description: system-scoped read and write access to AuditEvent resources
  flows:
  - authorizationCode
  scope: system/AuditEvent.*
- description: system-scoped read access to AuditEvent resources
  flows:
  - authorizationCode
  scope: system/AuditEvent.read
- description: system-scoped read and write access to Binary resources
  flows:
  - authorizationCode
  scope: system/Binary.*
- description: system-scoped read access to Binary resources
  flows:
  - authorizationCode
  scope: system/Binary.read
- description: system-scoped read and write access to CarePlan resources
  flows:
  - authorizationCode
  scope: system/CarePlan.*
- description: system-scoped read access to CarePlan resources
  flows:
  - authorizationCode
  scope: system/CarePlan.read
- description: system-scoped read and write access to Claim resources
  flows:
  - authorizationCode
  scope: system/Claim.*
- description: system-scoped read access to Claim resources
  flows:
  - authorizationCode
  scope: system/Claim.read
- description: system-scoped read and write access to Condition resources
  flows:
  - authorizationCode
  scope: system/Condition.*
- description: system-scoped read access to Condition resources
  flows:
  - authorizationCode
  scope: system/Condition.read
- description: system-scoped read and write access to Coverage resources
  flows:
  - authorizationCode
  scope: system/Coverage.*
- description: system-scoped read access to Coverage resources
  flows:
  - authorizationCode
  scope: system/Coverage.read
- description: system-scoped read and write access to Device resources
  flows:
  - authorizationCode
  scope: system/Device.*
- description: system-scoped read access to Device resources
  flows:
  - authorizationCode
  scope: system/Device.read
- description: system-scoped read and write access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: system/DiagnosticOrder.*
- description: system-scoped read access to DiagnosticOrder resources
  flows:
  - authorizationCode
  scope: system/DiagnosticOrder.read
- description: system-scoped read and write access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: system/DiagnosticReport.*
- description: system-scoped read access to DiagnosticReport resources
  flows:
  - authorizationCode
  scope: system/DiagnosticReport.read
- description: system-scoped read and write access to Encounter resources
  flows:
  - authorizationCode
  scope: system/Encounter.*
- description: system-scoped read access to Encounter resources
  flows:
  - authorizationCode
  scope: system/Encounter.read
- description: system-scoped read and write access to Goal resources
  flows:
  - authorizationCode
  scope: system/Goal.*
- description: system-scoped read access to Goal resources
  flows:
  - authorizationCode
  scope: system/Goal.read
- description: system-scoped read and write access to Group resources
  flows:
  - authorizationCode
  scope: system/Group.*
- description: system-scoped read access to Group resources
  flows:
  - authorizationCode
  scope: system/Group.read
- description: system-scoped read and write access to Immunization resources
  flows:
  - authorizationCode
  scope: system/Immunization.*
- description: system-scoped read access to Immunization resources
  flows:
  - authorizationCode
  scope: system/Immunization.read
- description: system-scoped read and write access to Location resources
  flows:
  - authorizationCode
  scope: system/Location.*
- description: system-scoped read access to Location resources
  flows:
  - authorizationCode
  scope: system/Location.read
- description: system-scoped read and write access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: system/MedicationAdministration.*
- description: system-scoped read access to MedicationAdministration resources
  flows:
  - authorizationCode
  scope: system/MedicationAdministration.read
- description: system-scoped read and write access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: system/MedicationDispense.*
- description: system-scoped read access to MedicationDispense resources
  flows:
  - authorizationCode
  scope: system/MedicationDispense.read
- description: system-scoped read and write access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: system/MedicationOrder.*
- description: system-scoped read access to MedicationOrder resources
  flows:
  - authorizationCode
  scope: system/MedicationOrder.read
- description: system-scoped read and write access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: system/MedicationStatement.*
- description: system-scoped read access to MedicationStatement resources
  flows:
  - authorizationCode
  scope: system/MedicationStatement.read
- description: system-scoped read and write access to Observation resources
  flows:
  - authorizationCode
  scope: system/Observation.*
- description: system-scoped read access to Observation resources
  flows:
  - authorizationCode
  scope: system/Observation.read
- description: system-scoped read and write access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: system/OperationDefinition.*
- description: system-scoped read access to OperationDefinition resources
  flows:
  - authorizationCode
  scope: system/OperationDefinition.read
- description: system-scoped read and write access to Organization resources
  flows:
  - authorizationCode
  scope: system/Organization.*
- description: system-scoped read access to Organization resources
  flows:
  - authorizationCode
  scope: system/Organization.read
- description: system-scoped read and write access to Patient resources
  flows:
  - authorizationCode
  scope: system/Patient.*
- description: system-scoped read access to Patient resources
  flows:
  - authorizationCode
  scope: system/Patient.read
- description: system-scoped read and write access to Person resources
  flows:
  - authorizationCode
  scope: system/Person.*
- description: system-scoped read access to Person resources
  flows:
  - authorizationCode
  scope: system/Person.read
- description: system-scoped read and write access to Practitioner resources
  flows:
  - authorizationCode
  scope: system/Practitioner.*
- description: system-scoped read access to Practitioner resources
  flows:
  - authorizationCode
  scope: system/Practitioner.read
- description: system-scoped read and write access to Procedure resources
  flows:
  - authorizationCode
  scope: system/Procedure.*
- description: system-scoped read access to Procedure resources
  flows:
  - authorizationCode
  scope: system/Procedure.read
- description: system-scoped read and write access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: system/ProcedureRequest.*
- description: system-scoped read access to ProcedureRequest resources
  flows:
  - authorizationCode
  scope: system/ProcedureRequest.read
- description: system-scoped read and write access to Provenance resources
  flows:
  - authorizationCode
  scope: system/Provenance.*
- description: system-scoped read access to Provenance resources
  flows:
  - authorizationCode
  scope: system/Provenance.read
- description: system-scoped read and write access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: system/ReferralRequest.*
- description: system-scoped read access to ReferralRequest resources
  flows:
  - authorizationCode
  scope: system/ReferralRequest.read
- description: system-scoped read and write access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: system/RelatedPerson.*
- description: system-scoped read access to RelatedPerson resources
  flows:
  - authorizationCode
  scope: system/RelatedPerson.read
- description: system-scoped read and write access to Specimen resources
  flows:
  - authorizationCode
  scope: system/Specimen.*
- description: system-scoped read access to Specimen resources
  flows:
  - authorizationCode
  scope: system/Specimen.read
- description: system-scoped read and write access to ValueSet resources
  flows:
  - authorizationCode
  scope: system/ValueSet.*
- description: system-scoped read access to ValueSet resources
  flows:
  - authorizationCode
  scope: system/ValueSet.read
- description: system-scoped read and write access to all resources
  flows:
  - authorizationCode
  scope: system/*.*
- description: system-scoped read access to all resources
  flows:
  - authorizationCode
  scope: system/*.read
- description: SMART EHR launch context
  flows:
  - authorizationCode
  scope: launch
- description: SMART standalone patient launch context
  flows:
  - authorizationCode
  scope: launch/patient
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims
  flows:
  - authorizationCode
  scope: profile
- description: Identity of the authorizing FHIR user
  flows:
  - authorizationCode
  scope: fhirUser
- description: Refresh token / offline access
  flows:
  - authorizationCode
  scope: offline_access
- description: Refresh token valid only while the user is online
  flows:
  - authorizationCode
  scope: online_access
slug: elevance-health-scopes
source_filename: elevance-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: Anonymous GET of the SMART App Launch and OpenID Connect discovery documents on each Elevance\n  Health FHIR host\ndocs: https://patient360c.anthem.com/P360Member/fhir/documentation\ndescription: OAuth 2.0 / SMART on FHIR scopes actually advertised by Elevance Health, read from the providers\n  own discovery documents rather than inferred. Supersedes the 2026-07-11 derived file, which listed three\n  scopes taken from a hand-written scaffold spec.\nsummary:\n  schemes: 3\n  scopes_total: 272\n  patient360_smart_scopes: 205\n  totalview_patient_access_scopes: 67\n  patient360_identityserver_oidc_scopes: 1048\nnotes:\n- The Patient360 IdentityServer OpenID Connect discovery document advertises 1048 scopes, a superset that\n  covers the whole CareEvolution HIEBus resource surface. Only the 205 scopes the SMART configuration\n  advertises for the FHIR base are enumerated here; the full list is in well-known/elevance-health-patient360c-openid-configuration.json.\n\
  - The Provider Directory and Formulary APIs use OAuth 2.0 client credentials and publish no scope list;\n  their token endpoint is issued privately by secure email after registration.\nschemes:\n- name: totalview-patient-access\n  api: Patient Access API (production, FHIR R4)\n  source: well-known/elevance-health-totalview-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://totalview.healthos.elevancehealth.com/oauth2.code/registered/api/v1/authorize\n    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token\n- name: patient360-smart\n  api: Patient360 FHIR (DSTU2)\n  source: well-known/elevance-health-patient360-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient360.anthem.com/P360Member/identityserver/connect/authorize\n    tokenUrl:\
  \ https://patient360.anthem.com/P360Member/identityserver/connect/token\n- name: provider-directory-and-formulary\n  api: Provider Directory API and Formulary API\n  source: https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: Token endpoint issued per registered application by secure email; not published.\nscopes:\n- scope: patient/AllergyIntolerance.*\n  flows: &id001\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to AllergyIntolerance resources\n- scope: patient/AllergyIntolerance.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to AllergyIntolerance resources\n- scope: patient/AuditEvent.*\n  flows: *id001\n  sources:\n  -\
  \ well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to AuditEvent resources\n- scope: patient/AuditEvent.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to AuditEvent resources\n- scope: patient/Basic.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Basic resources\n- scope: patient/Basic.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Basic resources\n- scope: patient/Binary.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Binary resources\n- scope: patient/Binary.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read access to Binary resources\n- scope: patient/CarePlan.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to CarePlan resources\n- scope: patient/CarePlan.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to CarePlan resources\n- scope: patient/CareTeam.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to CareTeam resources\n- scope: patient/CareTeam.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to CareTeam resources\n- scope: patient/Claim.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped\
  \ read and write access to Claim resources\n- scope: patient/Claim.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Claim resources\n- scope: patient/Condition.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Condition resources\n- scope: patient/Condition.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Condition resources\n- scope: patient/Coverage.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Coverage resources\n- scope: patient/Coverage.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to\
  \ Coverage resources\n- scope: patient/Device.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Device resources\n- scope: patient/Device.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Device resources\n- scope: patient/DiagnosticReport.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to DiagnosticReport resources\n- scope: patient/DiagnosticReport.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to DiagnosticReport resources\n- scope: patient/DocumentReference.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read\
  \ and write access to DocumentReference resources\n- scope: patient/DocumentReference.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to DocumentReference resources\n- scope: patient/Encounter.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Encounter resources\n- scope: patient/Encounter.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Encounter resources\n- scope: patient/ExplanationOfBenefit.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to ExplanationOfBenefit resources\n- scope: patient/ExplanationOfBenefit.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read access to ExplanationOfBenefit resources\n- scope: patient/Goal.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Goal resources\n- scope: patient/Goal.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Goal resources\n- scope: patient/Immunization.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Immunization resources\n- scope: patient/Immunization.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Immunization resources\n- scope: patient/Location.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description:\
  \ patient-scoped read and write access to Location resources\n- scope: patient/Location.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Location resources\n- scope: patient/MedicationDispense.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to MedicationDispense resources\n- scope: patient/MedicationDispense.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to MedicationDispense resources\n- scope: patient/MedicationRequest.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to MedicationRequest resources\n- scope: patient/MedicationRequest.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read access to MedicationRequest resources\n- scope: patient/Observation.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Observation resources\n- scope: patient/Observation.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Observation resources\n- scope: patient/Organization.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Organization resources\n- scope: patient/Organization.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Organization resources\n- scope: patient/Patient.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read and write access to Patient resources\n- scope: patient/Patient.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Patient resources\n- scope: patient/Practitioner.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Practitioner resources\n- scope: patient/Practitioner.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Practitioner resources\n- scope: patient/Procedure.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Procedure resources\n- scope: patient/Procedure.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read access to Procedure resources\n- scope: patient/Provenance.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Provenance resources\n- scope: patient/Provenance.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to Provenance resources\n- scope: patient/QuestionnaireResponse.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to QuestionnaireResponse resources\n- scope: patient/QuestionnaireResponse.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to QuestionnaireResponse resources\n- scope: patient/RelatedPerson.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read and write access to RelatedPerson resources\n- scope: patient/RelatedPerson.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to RelatedPerson resources\n- scope: patient/ServiceRequest.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to ServiceRequest resources\n- scope: patient/ServiceRequest.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to ServiceRequest resources\n- scope: patient/Specimen.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to Specimen resources\n- scope: patient/Specimen.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: patient-scoped read access to Specimen resources\n- scope: patient/*.*\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read and write access to all resources\n- scope: patient/*.read\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: patient-scoped read access to all resources\n- scope: launch\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: SMART EHR launch context\n- scope: launch/patient\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: SMART standalone patient launch context\n- scope: openid\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: OpenID Connect authentication\n- scope: profile\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n\
  \  description: Basic profile claims\n- scope: fhirUser\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: Identity of the authorizing FHIR user\n- scope: offline_access\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: Refresh token / offline access\n- scope: online_access\n  flows: *id001\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n  description: Refresh token valid only while the user is online\n- scope: patient/AllergyIntolerance.*\n  flows: &id002\n  - authorizationCode\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to AllergyIntolerance resources\n- scope: patient/AllergyIntolerance.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to AllergyIntolerance\
  \ resources\n- scope: patient/AuditEvent.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to AuditEvent resources\n- scope: patient/AuditEvent.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to AuditEvent resources\n- scope: patient/Binary.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Binary resources\n- scope: patient/Binary.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Binary resources\n- scope: patient/CarePlan.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to CarePlan resources\n\
  - scope: patient/CarePlan.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to CarePlan resources\n- scope: patient/Claim.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Claim resources\n- scope: patient/Claim.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Claim resources\n- scope: patient/Condition.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Condition resources\n- scope: patient/Condition.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Condition resources\n- scope: patient/Coverage.*\n\
  \  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Coverage resources\n- scope: patient/Coverage.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Coverage resources\n- scope: patient/Device.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Device resources\n- scope: patient/Device.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Device resources\n- scope: patient/DiagnosticOrder.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to DiagnosticOrder resources\n- scope: patient/DiagnosticOrder.read\n\
  \  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to DiagnosticOrder resources\n- scope: patient/DiagnosticReport.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to DiagnosticReport resources\n- scope: patient/DiagnosticReport.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to DiagnosticReport resources\n- scope: patient/Encounter.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Encounter resources\n- scope: patient/Encounter.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Encounter resources\n- scope:\
  \ patient/Goal.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Goal resources\n- scope: patient/Goal.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Goal resources\n- scope: patient/Group.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Group resources\n- scope: patient/Group.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Group resources\n- scope: patient/Immunization.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Immunization resources\n- scope: patient/Immunization.read\n\
  \  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Immunization resources\n- scope: patient/Location.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Location resources\n- scope: patient/Location.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Location resources\n- scope: patient/MedicationAdministration.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to MedicationAdministration resources\n- scope: patient/MedicationAdministration.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to MedicationAdministration\
  \ resources\n- scope: patient/MedicationDispense.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to MedicationDispense resources\n- scope: patient/MedicationDispense.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to MedicationDispense resources\n- scope: patient/MedicationOrder.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to MedicationOrder resources\n- scope: patient/MedicationOrder.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to MedicationOrder resources\n- scope: patient/MedicationStatement.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n\
  \  description: patient-scoped read and write access to MedicationStatement resources\n- scope: patient/MedicationStatement.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to MedicationStatement resources\n- scope: patient/Observation.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Observation resources\n- scope: patient/Observation.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Observation resources\n- scope: patient/OperationDefinition.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to OperationDefinition resources\n- scope: patient/OperationDefinition.read\n  flows: *id002\n  sources:\n\
  \  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to OperationDefinition resources\n- scope: patient/Organization.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Organization resources\n- scope: patient/Organization.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Organization resources\n- scope: patient/Patient.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Patient resources\n- scope: patient/Patient.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Patient resources\n- scope: patient/Person.*\n  flows: *id002\n  sources:\n\
  \  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Person resources\n- scope: patient/Person.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Person resources\n- scope: patient/Practitioner.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Practitioner resources\n- scope: patient/Practitioner.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Practitioner resources\n- scope: patient/Procedure.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Procedure resources\n- scope: patient/Procedure.read\n  flows: *id002\n  sources:\n\
  \  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Procedure resources\n- scope: patient/ProcedureRequest.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to ProcedureRequest resources\n- scope: patient/ProcedureRequest.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to ProcedureRequest resources\n- scope: patient/Provenance.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Provenance resources\n- scope: patient/Provenance.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Provenance resources\n- scope: patient/ReferralRequest.*\n\
  \  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to ReferralRequest resources\n- scope: patient/ReferralRequest.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to ReferralRequest resources\n- scope: patient/RelatedPerson.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to RelatedPerson resources\n- scope: patient/RelatedPerson.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to RelatedPerson resources\n- scope: patient/Specimen.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to Specimen resources\n\
  - scope: patient/Specimen.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to Specimen resources\n- scope: patient/ValueSet.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to ValueSet resources\n- scope: patient/ValueSet.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to ValueSet resources\n- scope: patient/*.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read and write access to all resources\n- scope: patient/*.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: patient-scoped read access to all resources\n- scope: user/AllergyIntolerance.*\n  flows:\
  \ *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to AllergyIntolerance resources\n- scope: user/AllergyIntolerance.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to AllergyIntolerance resources\n- scope: user/AuditEvent.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to AuditEvent resources\n- scope: user/AuditEvent.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to AuditEvent resources\n- scope: user/Binary.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to Binary resources\n- scope: user/Binary.read\n  flows: *id002\n\
  \  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to Binary resources\n- scope: user/CarePlan.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to CarePlan resources\n- scope: user/CarePlan.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to CarePlan resources\n- scope: user/Claim.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to Claim resources\n- scope: user/Claim.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to Claim resources\n- scope: user/Condition.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n\
  \  description: user-scoped read and write access to Condition resources\n- scope: user/Condition.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to Condition resources\n- scope: user/Coverage.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to Coverage resources\n- scope: user/Coverage.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to Coverage resources\n- scope: user/Device.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to Device resources\n- scope: user/Device.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access\
  \ to Device resources\n- scope: user/DiagnosticOrder.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to DiagnosticOrder resources\n- scope: user/DiagnosticOrder.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to DiagnosticOrder resources\n- scope: user/DiagnosticReport.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read and write access to DiagnosticReport resources\n- scope: user/DiagnosticReport.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to DiagnosticReport resources\n- scope: user/Encounter.*\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped\
  \ read and write access to Encounter resources\n- scope: user/Encounter.read\n  flows: *id002\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  description: user-scoped read access to Encounter resources\n- scope: user/Goal.\n\n# --- truncated at 32 KB (54 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/scopes/elevance-health-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/scopes/elevance-health-scopes.yml
summary_line: 272 scopes · authorizationCode/clientCredentials
tags:
- Fortune 500
- Healthcare
- Health Insurance
- FHIR
- Interoperability
- CMS Interoperability
- SMART on FHIR
- Da Vinci PDEX
- CARIN Blue Button
- Payer
- Provider Directory
- Formulary
- HL7
token_urls:
- https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token
- https://patient360.anthem.com/P360Member/identityserver/connect/token
---
