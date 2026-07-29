---
api_specs:
- filename: advancedmd-fhir-single-api-openapi.json
  format: json
  label: AdvancedMD FHIR Single API (US Core 6.1.0)
  slug: advancedmd-fhir-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-single-api-openapi.json
- filename: advancedmd-fhir-bulk-api-openapi.json
  format: json
  label: AdvancedMD FHIR Bulk API
  slug: advancedmd-fhir-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-fhir-bulk-api-openapi.json
- filename: advancedmd-application-access-apis-swagger.json
  format: json
  label: AdvancedMD Application Access APIs (Legacy Patient APIs)
  slug: advancedmd-application-access-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/openapi/advancedmd-application-access-apis-swagger.json
authorization_urls:
- https://providerapi.advancedmd.com/v1/oauth2/authorize
description: SMART-on-FHIR OAuth 2.0 scope surface for the AdvancedMD certified FHIR APIs. The three OpenAPI documents in openapi/ declare only a bare bearerAuth scheme and carry no oauth2 flows, so the scope set is taken from the provider's published SMART discovery document and the portal authorization page rather than derived from the specs.
docs: https://fhir.advancedmd.com/fhir/launch-and-authorization
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Advancedmd Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AdvancedMD publishes 128 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the AdvancedMD API on a user''s behalf.


  Tokens are issued from https://providerapi.advancedmd.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AdvancedMD
provider_slug: advancedmd
schemes:
- flows:
  - authorizationUrl: https://providerapi.advancedmd.com/v1/oauth2/authorize
    flow: authorizationCode
    pkce: S256 (code_challenge_methods_supported)
    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token
    used_by: Patient and practitioner SMART apps against the FHIR Single API (3-legged OAuth).
  - client_authentication: private_key_jwt — RS384-signed client_assertion with client_assertion_type urn:ietf:params:oauth:client-assertion-type:jwt-bearer
    flow: clientCredentials
    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token
    used_by: SMART Backend Services authorization for the FHIR Bulk Data API.
  introspection_endpoint: https://providerapi.advancedmd.com/v1/oauth2/introspect
  issuer: https://providerapi.advancedmd.com/v1/r4
  jwks_uri: https://providerapi.advancedmd.com/v1/oauth2/.well-known/jwks.json
  management_endpoint: https://providerapi.advancedmd.com/v1/oauth2/manage
  name: SMART-on-FHIR OAuth 2.0
  revocation_endpoint: https://providerapi.advancedmd.com/v1/oauth2/revoke
  source: fhir/advancedmd-smart-configuration.json
scope_count: 128
scope_names:
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
- patient/CarePlan.read
- patient/CarePlan.rs
- patient/CareTeam.read
- patient/CareTeam.rs
- patient/Condition.read
- patient/Condition.rs
- patient/Consent.read
- patient/Consent.rs
- patient/Coverage.read
- patient/Coverage.rs
- patient/Device.read
- patient/Device.rs
- patient/DiagnosticReport.read
- patient/DiagnosticReport.rs
- patient/DocumentReference.read
- patient/DocumentReference.rs
- patient/Encounter.read
- patient/Encounter.rs
- patient/Endpoint.read
- patient/Endpoint.rs
- patient/ExplanationOfBenefit.read
- patient/ExplanationOfBenefit.rs
- patient/Goal.read
- patient/Goal.rs
- patient/Immunization.read
- patient/Immunization.rs
- patient/Location.read
- patient/Location.rs
- patient/Medication.read
- patient/Medication.rs
- patient/MedicationRequest.read
- patient/MedicationRequest.rs
- patient/MedicationDispense.read
- patient/MedicationDispense.rs
- patient/Observation.read
- patient/Observation.rs
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
- patient/ServiceRequest.read
- patient/ServiceRequest.rs
- patient/RelatedPerson.read
- patient/RelatedPerson.rs
- patient/Specimen.read
- patient/Specimen.rs
- system/*.read
- system/*.rs
- system/Consent.read
- system/Consent.rs
- system/ExplanationOfBenefit.read
- system/ExplanationOfBenefit.rs
- user/*.read
- user/*.rs
- user/AllergyIntolerance.read
- user/AllergyIntolerance.rs
- user/CarePlan.read
- user/CarePlan.rs
- user/CareTeam.read
- user/CareTeam.rs
- user/Condition.read
- user/Condition.rs
- user/Consent.read
- user/Consent.rs
- user/Coverage.read
- user/Coverage.rs
- user/Device.read
- user/Device.rs
- user/DiagnosticReport.read
- user/DiagnosticReport.rs
- user/DocumentReference.read
- user/DocumentReference.rs
- user/Encounter.read
- user/Encounter.rs
- user/Endpoint.read
- user/Endpoint.rs
- user/ExplanationOfBenefit.read
- user/ExplanationOfBenefit.rs
- user/Goal.read
- user/Goal.rs
- user/Immunization.read
- user/Immunization.rs
- user/Location.read
- user/Location.rs
- user/Medication.read
- user/Medication.rs
- user/MedicationRequest.read
- user/MedicationRequest.rs
- user/MedicationDispense.read
- user/MedicationDispense.rs
- user/Observation.read
- user/Observation.rs
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
- user/ServiceRequest.read
- user/ServiceRequest.rs
- user/RelatedPerson.read
- user/RelatedPerson.rs
- user/Specimen.read
- user/Specimen.rs
scopes:
- description: Returns the FHIR resource (Patient/… or Practitioner/…) representing the authorized user.
  flows:
  - authorizationCode
  scope: fhirUser
- description: EHR launch context — the app is launched from within AdvancedMD and inherits its context.
  flows:
  - authorizationCode
  scope: launch
- description: Standalone launch requesting a patient context be selected during authorization.
  flows:
  - authorizationCode
  scope: launch/patient
- description: Issues a refresh token usable while the user is offline.
  flows:
  - authorizationCode
  scope: offline_access
- description: Issues a refresh token usable only while the user remains online.
  flows:
  - authorizationCode
  scope: online_access
- description: OpenID Connect authentication; returns an id_token identifying the authorized user.
  flows:
  - authorizationCode
  scope: openid
- description: read + search (SMART v1 style) access to all supported FHIR resource types for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/*.read
- description: read + search (SMART v2 granular style) access to all supported FHIR resource types for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/*.rs
- description: read + search (SMART v1 style) access to the AllergyIntolerance FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.read
- description: read + search (SMART v2 granular style) access to the AllergyIntolerance FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.rs
- description: read + search (SMART v1 style) access to the CarePlan FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/CarePlan.read
- description: read + search (SMART v2 granular style) access to the CarePlan FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/CarePlan.rs
- description: read + search (SMART v1 style) access to the CareTeam FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/CareTeam.read
- description: read + search (SMART v2 granular style) access to the CareTeam FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/CareTeam.rs
- description: read + search (SMART v1 style) access to the Condition FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: read + search (SMART v2 granular style) access to the Condition FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Condition.rs
- description: read + search (SMART v1 style) access to the Consent FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Consent.read
- description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Consent.rs
- description: read + search (SMART v1 style) access to the Coverage FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: read + search (SMART v2 granular style) access to the Coverage FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Coverage.rs
- description: read + search (SMART v1 style) access to the Device FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Device.read
- description: read + search (SMART v2 granular style) access to the Device FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Device.rs
- description: read + search (SMART v1 style) access to the DiagnosticReport FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.read
- description: read + search (SMART v2 granular style) access to the DiagnosticReport FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.rs
- description: read + search (SMART v1 style) access to the DocumentReference FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: read + search (SMART v2 granular style) access to the DocumentReference FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/DocumentReference.rs
- description: read + search (SMART v1 style) access to the Encounter FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: read + search (SMART v2 granular style) access to the Encounter FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Encounter.rs
- description: read + search (SMART v1 style) access to the Endpoint FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Endpoint.read
- description: read + search (SMART v2 granular style) access to the Endpoint FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Endpoint.rs
- description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.rs
- description: read + search (SMART v1 style) access to the Goal FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Goal.read
- description: read + search (SMART v2 granular style) access to the Goal FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Goal.rs
- description: read + search (SMART v1 style) access to the Immunization FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: read + search (SMART v2 granular style) access to the Immunization FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Immunization.rs
- description: read + search (SMART v1 style) access to the Location FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Location.read
- description: read + search (SMART v2 granular style) access to the Location FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Location.rs
- description: read + search (SMART v1 style) access to the Medication FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Medication.read
- description: read + search (SMART v2 granular style) access to the Medication FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Medication.rs
- description: read + search (SMART v1 style) access to the MedicationRequest FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: read + search (SMART v2 granular style) access to the MedicationRequest FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.rs
- description: read + search (SMART v1 style) access to the MedicationDispense FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.read
- description: read + search (SMART v2 granular style) access to the MedicationDispense FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.rs
- description: read + search (SMART v1 style) access to the Observation FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: read + search (SMART v2 granular style) access to the Observation FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Observation.rs
- description: read + search (SMART v1 style) access to the Organization FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Organization.read
- description: read + search (SMART v2 granular style) access to the Organization FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Organization.rs
- description: read + search (SMART v1 style) access to the Patient FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: read + search (SMART v2 granular style) access to the Patient FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Patient.rs
- description: read + search (SMART v1 style) access to the Practitioner FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Practitioner.read
- description: read + search (SMART v2 granular style) access to the Practitioner FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Practitioner.rs
- description: read + search (SMART v1 style) access to the PractitionerRole FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.read
- description: read + search (SMART v2 granular style) access to the PractitionerRole FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.rs
- description: read + search (SMART v1 style) access to the Procedure FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Procedure.read
- description: read + search (SMART v2 granular style) access to the Procedure FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Procedure.rs
- description: read + search (SMART v1 style) access to the Provenance FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Provenance.read
- description: read + search (SMART v2 granular style) access to the Provenance FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Provenance.rs
- description: read + search (SMART v1 style) access to the ServiceRequest FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/ServiceRequest.read
- description: read + search (SMART v2 granular style) access to the ServiceRequest FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/ServiceRequest.rs
- description: read + search (SMART v1 style) access to the RelatedPerson FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.read
- description: read + search (SMART v2 granular style) access to the RelatedPerson FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/RelatedPerson.rs
- description: read + search (SMART v1 style) access to the Specimen FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Specimen.read
- description: read + search (SMART v2 granular style) access to the Specimen FHIR resource type for the single patient in context.
  flows:
  - authorizationCode
  scope: patient/Specimen.rs
- description: read + search (SMART v1 style) access to all supported FHIR resource types for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/*.read
- description: read + search (SMART v2 granular style) access to all supported FHIR resource types for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/*.rs
- description: read + search (SMART v1 style) access to the Consent FHIR resource type for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/Consent.read
- description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/Consent.rs
- description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/ExplanationOfBenefit.read
- description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource type for the whole system (backend services / Bulk Data).
  flows:
  - clientCredentials
  scope: system/ExplanationOfBenefit.rs
- description: read + search (SMART v1 style) access to all supported FHIR resource types for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/*.read
- description: read + search (SMART v2 granular style) access to all supported FHIR resource types for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/*.rs
- description: read + search (SMART v1 style) access to the AllergyIntolerance FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.read
- description: read + search (SMART v2 granular style) access to the AllergyIntolerance FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/AllergyIntolerance.rs
- description: read + search (SMART v1 style) access to the CarePlan FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/CarePlan.read
- description: read + search (SMART v2 granular style) access to the CarePlan FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/CarePlan.rs
- description: read + search (SMART v1 style) access to the CareTeam FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/CareTeam.read
- description: read + search (SMART v2 granular style) access to the CareTeam FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/CareTeam.rs
- description: read + search (SMART v1 style) access to the Condition FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Condition.read
- description: read + search (SMART v2 granular style) access to the Condition FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Condition.rs
- description: read + search (SMART v1 style) access to the Consent FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Consent.read
- description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Consent.rs
- description: read + search (SMART v1 style) access to the Coverage FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Coverage.read
- description: read + search (SMART v2 granular style) access to the Coverage FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Coverage.rs
- description: read + search (SMART v1 style) access to the Device FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Device.read
- description: read + search (SMART v2 granular style) access to the Device FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Device.rs
- description: read + search (SMART v1 style) access to the DiagnosticReport FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.read
- description: read + search (SMART v2 granular style) access to the DiagnosticReport FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/DiagnosticReport.rs
- description: read + search (SMART v1 style) access to the DocumentReference FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/DocumentReference.read
- description: read + search (SMART v2 granular style) access to the DocumentReference FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/DocumentReference.rs
- description: read + search (SMART v1 style) access to the Encounter FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Encounter.read
- description: read + search (SMART v2 granular style) access to the Encounter FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Encounter.rs
- description: read + search (SMART v1 style) access to the Endpoint FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Endpoint.read
- description: read + search (SMART v2 granular style) access to the Endpoint FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Endpoint.rs
- description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/ExplanationOfBenefit.read
- description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/ExplanationOfBenefit.rs
- description: read + search (SMART v1 style) access to the Goal FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Goal.read
- description: read + search (SMART v2 granular style) access to the Goal FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Goal.rs
- description: read + search (SMART v1 style) access to the Immunization FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Immunization.read
- description: read + search (SMART v2 granular style) access to the Immunization FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Immunization.rs
- description: read + search (SMART v1 style) access to the Location FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Location.read
- description: read + search (SMART v2 granular style) access to the Location FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Location.rs
- description: read + search (SMART v1 style) access to the Medication FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Medication.read
- description: read + search (SMART v2 granular style) access to the Medication FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Medication.rs
- description: read + search (SMART v1 style) access to the MedicationRequest FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/MedicationRequest.read
- description: read + search (SMART v2 granular style) access to the MedicationRequest FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/MedicationRequest.rs
- description: read + search (SMART v1 style) access to the MedicationDispense FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/MedicationDispense.read
- description: read + search (SMART v2 granular style) access to the MedicationDispense FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/MedicationDispense.rs
- description: read + search (SMART v1 style) access to the Observation FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Observation.read
- description: read + search (SMART v2 granular style) access to the Observation FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Observation.rs
- description: read + search (SMART v1 style) access to the Organization FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Organization.read
- description: read + search (SMART v2 granular style) access to the Organization FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Organization.rs
- description: read + search (SMART v1 style) access to the Patient FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Patient.read
- description: read + search (SMART v2 granular style) access to the Patient FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Patient.rs
- description: read + search (SMART v1 style) access to the Practitioner FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Practitioner.read
- description: read + search (SMART v2 granular style) access to the Practitioner FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Practitioner.rs
- description: read + search (SMART v1 style) access to the PractitionerRole FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/PractitionerRole.read
- description: read + search (SMART v2 granular style) access to the PractitionerRole FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/PractitionerRole.rs
- description: read + search (SMART v1 style) access to the Procedure FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Procedure.read
- description: read + search (SMART v2 granular style) access to the Procedure FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Procedure.rs
- description: read + search (SMART v1 style) access to the Provenance FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Provenance.read
- description: read + search (SMART v2 granular style) access to the Provenance FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Provenance.rs
- description: read + search (SMART v1 style) access to the ServiceRequest FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/ServiceRequest.read
- description: read + search (SMART v2 granular style) access to the ServiceRequest FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/ServiceRequest.rs
- description: read + search (SMART v1 style) access to the RelatedPerson FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/RelatedPerson.read
- description: read + search (SMART v2 granular style) access to the RelatedPerson FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/RelatedPerson.rs
- description: read + search (SMART v1 style) access to the Specimen FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Specimen.read
- description: read + search (SMART v2 granular style) access to the Specimen FHIR resource type for every record the authorized user may see.
  flows:
  - authorizationCode
  scope: user/Specimen.rs
slug: advancedmd-scopes
source_filename: advancedmd-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://providerapi.advancedmd.com/v1/r4/.well-known/smart-configuration (HTTP 200, saved verbatim\n  at fhir/advancedmd-smart-configuration.json) — scopes_supported enumerated live on 2026-07-27.\ndocs: https://fhir.advancedmd.com/fhir/launch-and-authorization\ndescription: SMART-on-FHIR OAuth 2.0 scope surface for the AdvancedMD certified FHIR APIs. The three OpenAPI\n  documents in openapi/ declare only a bare bearerAuth scheme and carry no oauth2 flows, so the scope\n  set is taken from the provider's published SMART discovery document and the portal authorization page\n  rather than derived from the specs.\nstandard: SMART App Launch — SMART v1 (.read) and SMART v2 granular (.rs) scope syntax, both advertised\n  via the permission-v1 and permission-v2 capabilities.\nschemes:\n- name: SMART-on-FHIR OAuth 2.0\n  issuer: https://providerapi.advancedmd.com/v1/r4\n  source: fhir/advancedmd-smart-configuration.json\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://providerapi.advancedmd.com/v1/oauth2/authorize\n    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token\n    pkce: S256 (code_challenge_methods_supported)\n    used_by: Patient and practitioner SMART apps against the FHIR Single API (3-legged OAuth).\n  - flow: clientCredentials\n    tokenUrl: https://providerapi.advancedmd.com/v1/oauth2/token\n    client_authentication: private_key_jwt — RS384-signed client_assertion with client_assertion_type\n      urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n    used_by: SMART Backend Services authorization for the FHIR Bulk Data API.\n  jwks_uri: https://providerapi.advancedmd.com/v1/oauth2/.well-known/jwks.json\n  introspection_endpoint: https://providerapi.advancedmd.com/v1/oauth2/introspect\n  revocation_endpoint: https://providerapi.advancedmd.com/v1/oauth2/revoke\n  management_endpoint: https://providerapi.advancedmd.com/v1/oauth2/manage\nnotes:\n- 'The portal documents\
  \ a default requested scope set of: openid fhirUser offline_access online_access\n  patient/*.read.'\n- The FHIR Launch and Authorization page states that user-level scopes are advertised but \"not yet supported\"\n  in practice, and that the scope set will be extended with FHIR v6 clinical-data scopes; the discovery\n  document nonetheless enumerates the full user/* set, so both are recorded here.\n- Two-legged OAuth for general system-to-system access is explicitly NOT supported; system/*.read exists\n  only for the Bulk Data backend-services flow.\n- 'With a user/*.read token the access token still carries a fixed patient context: a request without\n  an explicit patient parameter is answered for the launch patient only.'\n- The Bulk token request additionally requires username, password and officekey form parameters alongside\n  the standard client_credentials parameters.\nscope_groups:\n  patient: 58\n  user: 58\n  system: 6\n  identity_and_launch: 6\nscopes:\n- scope: fhirUser\n\
  \  description: Returns the FHIR resource (Patient/… or Practitioner/…) representing the authorized user.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: launch\n  description: EHR launch context — the app is launched from within AdvancedMD and inherits its context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: launch/patient\n  description: Standalone launch requesting a patient context be selected during authorization.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: offline_access\n  description: Issues a refresh token usable while the user is offline.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: online_access\n  description: Issues a refresh token usable only while the user remains online.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: openid\n  description: OpenID Connect authentication; returns an id_token identifying the authorized user.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/*.read\n  description: read + search (SMART v1 style) access to all supported FHIR resource types for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/*.rs\n  description: read + search (SMART v2 granular style) access to all supported FHIR resource types for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/AllergyIntolerance.read\n  description: read + search (SMART v1 style) access to the AllergyIntolerance FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/AllergyIntolerance.rs\n\
  \  description: read + search (SMART v2 granular style) access to the AllergyIntolerance FHIR resource\n    type for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/CarePlan.read\n  description: read + search (SMART v1 style) access to the CarePlan FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/CarePlan.rs\n  description: read + search (SMART v2 granular style) access to the CarePlan FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/CareTeam.read\n  description: read + search (SMART v1 style) access to the CareTeam FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: patient/CareTeam.rs\n  description: read + search (SMART v2 granular style) access to the CareTeam FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Condition.read\n  description: read + search (SMART v1 style) access to the Condition FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Condition.rs\n  description: read + search (SMART v2 granular style) access to the Condition FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Consent.read\n  description: read + search (SMART v1 style) access to the Consent FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: patient/Consent.rs\n  description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Coverage.read\n  description: read + search (SMART v1 style) access to the Coverage FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Coverage.rs\n  description: read + search (SMART v2 granular style) access to the Coverage FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Device.read\n  description: read + search (SMART v1 style) access to the Device FHIR resource type for the single patient\n    in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: patient/Device.rs\n  description: read + search (SMART v2 granular style) access to the Device FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/DiagnosticReport.read\n  description: read + search (SMART v1 style) access to the DiagnosticReport FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/DiagnosticReport.rs\n  description: read + search (SMART v2 granular style) access to the DiagnosticReport FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/DocumentReference.read\n  description: read + search (SMART v1 style) access to the DocumentReference FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/DocumentReference.rs\n  description: read + search (SMART v2 granular style) access to the DocumentReference FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Encounter.read\n  description: read + search (SMART v1 style) access to the Encounter FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Encounter.rs\n  description: read + search (SMART v2 granular style) access to the Encounter FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Endpoint.read\n  description: read + search (SMART v1 style) access to the Endpoint FHIR resource type for the single\n    patient in\
  \ context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Endpoint.rs\n  description: read + search (SMART v2 granular style) access to the Endpoint FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/ExplanationOfBenefit.read\n  description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/ExplanationOfBenefit.rs\n  description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource\n    type for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Goal.read\n  description: read + search (SMART v1 style) access\
  \ to the Goal FHIR resource type for the single patient\n    in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Goal.rs\n  description: read + search (SMART v2 granular style) access to the Goal FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Immunization.read\n  description: read + search (SMART v1 style) access to the Immunization FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Immunization.rs\n  description: read + search (SMART v2 granular style) access to the Immunization FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Location.read\n  description: read + search\
  \ (SMART v1 style) access to the Location FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Location.rs\n  description: read + search (SMART v2 granular style) access to the Location FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Medication.read\n  description: read + search (SMART v1 style) access to the Medication FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Medication.rs\n  description: read + search (SMART v2 granular style) access to the Medication FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/MedicationRequest.read\n\
  \  description: read + search (SMART v1 style) access to the MedicationRequest FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/MedicationRequest.rs\n  description: read + search (SMART v2 granular style) access to the MedicationRequest FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/MedicationDispense.read\n  description: read + search (SMART v1 style) access to the MedicationDispense FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/MedicationDispense.rs\n  description: read + search (SMART v2 granular style) access to the MedicationDispense FHIR resource\n    type for the single patient in context.\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Observation.read\n  description: read + search (SMART v1 style) access to the Observation FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Observation.rs\n  description: read + search (SMART v2 granular style) access to the Observation FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Organization.read\n  description: read + search (SMART v1 style) access to the Organization FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Organization.rs\n  description: read + search (SMART v2 granular style) access to the Organization FHIR resource type for\n    the single patient\
  \ in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Patient.read\n  description: read + search (SMART v1 style) access to the Patient FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Patient.rs\n  description: read + search (SMART v2 granular style) access to the Patient FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Practitioner.read\n  description: read + search (SMART v1 style) access to the Practitioner FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Practitioner.rs\n  description: read + search (SMART v2 granular style) access to the Practitioner FHIR resource\
  \ type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/PractitionerRole.read\n  description: read + search (SMART v1 style) access to the PractitionerRole FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/PractitionerRole.rs\n  description: read + search (SMART v2 granular style) access to the PractitionerRole FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Procedure.read\n  description: read + search (SMART v1 style) access to the Procedure FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Procedure.rs\n  description: read + search (SMART\
  \ v2 granular style) access to the Procedure FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Provenance.read\n  description: read + search (SMART v1 style) access to the Provenance FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Provenance.rs\n  description: read + search (SMART v2 granular style) access to the Provenance FHIR resource type for\n    the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/ServiceRequest.read\n  description: read + search (SMART v1 style) access to the ServiceRequest FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/ServiceRequest.rs\n\
  \  description: read + search (SMART v2 granular style) access to the ServiceRequest FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/RelatedPerson.read\n  description: read + search (SMART v1 style) access to the RelatedPerson FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/RelatedPerson.rs\n  description: read + search (SMART v2 granular style) access to the RelatedPerson FHIR resource type\n    for the single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: patient/Specimen.read\n  description: read + search (SMART v1 style) access to the Specimen FHIR resource type for the single\n    patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: patient/Specimen.rs\n  description: read + search (SMART v2 granular style) access to the Specimen FHIR resource type for the\n    single patient in context.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/*.read\n  description: read + search (SMART v1 style) access to all supported FHIR resource types for the whole\n    system (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/*.rs\n  description: read + search (SMART v2 granular style) access to all supported FHIR resource types for\n    the whole system (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/Consent.read\n  description: read + search (SMART v1 style) access to the Consent FHIR resource type for the whole system\n    (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/Consent.rs\n  description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for the\n    whole system (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/ExplanationOfBenefit.read\n  description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for\n    the whole system (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: system/ExplanationOfBenefit.rs\n  description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource\n    type for the whole system (backend services / Bulk Data).\n  flows:\n  - clientCredentials\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/*.read\n  description: read + search (SMART v1 style) access\
  \ to all supported FHIR resource types for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/*.rs\n  description: read + search (SMART v2 granular style) access to all supported FHIR resource types for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/AllergyIntolerance.read\n  description: read + search (SMART v1 style) access to the AllergyIntolerance FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/AllergyIntolerance.rs\n  description: read + search (SMART v2 granular style) access to the AllergyIntolerance FHIR resource\n    type for every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: user/CarePlan.read\n  description: read + search (SMART v1 style) access to the CarePlan FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/CarePlan.rs\n  description: read + search (SMART v2 granular style) access to the CarePlan FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/CareTeam.read\n  description: read + search (SMART v1 style) access to the CareTeam FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/CareTeam.rs\n  description: read + search (SMART v2 granular style) access to the CareTeam FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - fhir/advancedmd-smart-configuration.json\n- scope: user/Condition.read\n  description: read + search (SMART v1 style) access to the Condition FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Condition.rs\n  description: read + search (SMART v2 granular style) access to the Condition FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Consent.read\n  description: read + search (SMART v1 style) access to the Consent FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Consent.rs\n  description: read + search (SMART v2 granular style) access to the Consent FHIR resource type for every\n    record the authorized user\
  \ may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Coverage.read\n  description: read + search (SMART v1 style) access to the Coverage FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Coverage.rs\n  description: read + search (SMART v2 granular style) access to the Coverage FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Device.read\n  description: read + search (SMART v1 style) access to the Device FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Device.rs\n  description: read + search (SMART v2 granular style) access to the Device FHIR resource\
  \ type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/DiagnosticReport.read\n  description: read + search (SMART v1 style) access to the DiagnosticReport FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/DiagnosticReport.rs\n  description: read + search (SMART v2 granular style) access to the DiagnosticReport FHIR resource type\n    for every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/DocumentReference.read\n  description: read + search (SMART v1 style) access to the DocumentReference FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/DocumentReference.rs\n\
  \  description: read + search (SMART v2 granular style) access to the DocumentReference FHIR resource type\n    for every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Encounter.read\n  description: read + search (SMART v1 style) access to the Encounter FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Encounter.rs\n  description: read + search (SMART v2 granular style) access to the Encounter FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Endpoint.read\n  description: read + search (SMART v1 style) access to the Endpoint FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n\
  - scope: user/Endpoint.rs\n  description: read + search (SMART v2 granular style) access to the Endpoint FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/ExplanationOfBenefit.read\n  description: read + search (SMART v1 style) access to the ExplanationOfBenefit FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/ExplanationOfBenefit.rs\n  description: read + search (SMART v2 granular style) access to the ExplanationOfBenefit FHIR resource\n    type for every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Goal.read\n  description: read + search (SMART v1 style) access to the Goal FHIR resource type for every record the\n    authorized user may see.\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Goal.rs\n  description: read + search (SMART v2 granular style) access to the Goal FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Immunization.read\n  description: read + search (SMART v1 style) access to the Immunization FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Immunization.rs\n  description: read + search (SMART v2 granular style) access to the Immunization FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Location.read\n  description: read + search (SMART v1 style) access to the Location FHIR resource\
  \ type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Location.rs\n  description: read + search (SMART v2 granular style) access to the Location FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Medication.read\n  description: read + search (SMART v1 style) access to the Medication FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Medication.rs\n  description: read + search (SMART v2 granular style) access to the Medication FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/MedicationRequest.read\n  description:\
  \ read + search (SMART v1 style) access to the MedicationRequest FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/MedicationRequest.rs\n  description: read + search (SMART v2 granular style) access to the MedicationRequest FHIR resource type\n    for every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/MedicationDispense.read\n  description: read + search (SMART v1 style) access to the MedicationDispense FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/MedicationDispense.rs\n  description: read + search (SMART v2 granular style) access to the MedicationDispense FHIR resource\n    type for every record the authorized user may see.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Observation.read\n  description: read + search (SMART v1 style) access to the Observation FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Observation.rs\n  description: read + search (SMART v2 granular style) access to the Observation FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Organization.read\n  description: read + search (SMART v1 style) access to the Organization FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Organization.rs\n  description: read + search (SMART v2 granular style) access to the Organization\
  \ FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Patient.read\n  description: read + search (SMART v1 style) access to the Patient FHIR resource type for every record\n    the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Patient.rs\n  description: read + search (SMART v2 granular style) access to the Patient FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Practitioner.read\n  description: read + search (SMART v1 style) access to the Practitioner FHIR resource type for every\n    record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/Practitioner.rs\n  description:\
  \ read + search (SMART v2 granular style) access to the Practitioner FHIR resource type for\n    every record the authorized user may see.\n  flows:\n  - authorizationCode\n  sources:\n  - fhir/advancedmd-smart-configuration.json\n- scope: user/PractitionerRole.read\n  description: read + search (SMART v1 style) access to the PractitionerRole FHIR resource type for every\n    record the authorized user\n\n# --- truncated at 32 KB (34 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/scopes/advancedmd-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancedmd/refs/heads/main/scopes/advancedmd-scopes.yml
summary_line: 128 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- United States
- EHR
- EMR
- Practice Management
- Medical Billing
- FHIR
- HL7
- SMART on FHIR
- US Core
- Interoperability
- Revenue Cycle Management
- Scheduling
token_urls:
- https://providerapi.advancedmd.com/v1/oauth2/token
---
