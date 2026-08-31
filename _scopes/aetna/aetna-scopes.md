---
api_specs:
- filename: aetna-patient-access-api-openapi.yml
  format: yaml
  label: Aetna Patient Access FHIR API
  slug: aetna-patient-access-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-patient-access-api-openapi.yml
- filename: aetna-provider-directory-api-openapi.yml
  format: yaml
  label: Aetna Provider Directory FHIR API
  slug: aetna-provider-directory-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-provider-directory-api-openapi.yml
- filename: aetna-patient-access-api-openapi.yml
  format: yaml
  label: Aetna Drug Formulary FHIR API
  slug: aetna-drug-formulary-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/openapi/aetna-patient-access-api-openapi.yml
authorization_urls:
- https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize
- https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize
description: ''
docs: https://apif1.aetna.com/fhir/.well-known/smart-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Aetna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Aetna publishes 54 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Aetna API on a user''s behalf.


  Tokens are issued from https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Aetna
provider_slug: aetna
schemes:
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Allergy_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Binary_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_CarePlan_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRCareTeamRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_CareTeam_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientConditionRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Condition_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token
  name: FHIR_Patient_Coverage_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRDeviceRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Device_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientDiagnosticReportRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_DiagnosticReport_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientDocumentReferenceRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_DocumentReference_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientEncounterRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Encounter_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientEndpointRead",

    "Backend" : Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS",

    "Errorhandlingpolicy": "Transparent",

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Endpoint_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientEOBRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent",

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_EOB_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientGoalRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Goal_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Immunization_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token
  name: FHIR_Patient_MedicationKnowledge_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientMedicationRequestRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_MedicationRequest_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Medication_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token
  name: FHIR_Patient_Observation_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Organization_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Patient_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token
  name: FHIR_Patient_PractitionerRole_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Practitioner_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientProcedureRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Procedure_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Allergy_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Binary_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_CarePlan_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRCareTeamRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_CareTeam_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientConditionRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Condition_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Coverage_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRDeviceRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Device_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientDiagnosticReportRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_DiagnosticReport_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientDocumentReferenceRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_DocumentReference_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientEncounterRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Encounter_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientEndpointRead",

    "Backend" : Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS",

    "Errorhandlingpolicy": "Transparent",

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Endpoint_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token
  name: FHIR_Patient_EOB_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientGoalRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Goal_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Immunization_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Location_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientMedicationDispenseRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_MedicationDispense_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientMedicationRequestRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_MedicationRequest_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Medication_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Observation_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Organization_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Patient_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token
  name: FHIR_Patient_PractitionerRole_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - flow: authorizationCode
  name: FHIR_Patient_Practitioner_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- description: '{

    "BuildEieHeader" : "Header 3.2",

    "SecurityTemplate" : "FHIRPatientProcedureRead",

    "Backend" : "IIB",

    "Errorhandlingpolicy": "Transparent"

    "Consumer":"External",

    "Mutual Auth between Consumer and APIC" : "Not Required"

    }'
  flows:
  - flow: authorizationCode
  name: FHIR_Patient_Procedure_Read_AccessCode_Oauth
  source: openapi/aetna-patient-access-api-sandbox-openapi.yml
- flows:
  - authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token
  name: FHIR_User_AccessCode_Oauth
  source: openapi/aetna-provider-directory-api-openapi.yml
- description: "{\n \"BuildEieHeader\" : \"Header 3.2\",\n \"SecurityTemplate\" : \"FHIROpenApp\",\n \"Backend\" : \"Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\",\n \"Errorhandlingpolicy\": \"Transparent\"\n \"Consumer\":\"External\",\n \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n}"
  flows:
  - flow: clientCredentials
    tokenUrl: https://$(catalog.url)/v3/internal/auth/oauth2/app/token
  name: FHIR_Application_Oauth
  source: openapi/aetna-provider-directory-api-openapi.yml
scope_count: 54
scope_names:
- NonPII
- Public
- patient/*.*
- patient/*.read
- patient/Allergy.*
- patient/Allergy.read
- patient/Binary.*
- patient/Binary.read
- patient/CarePlan.*
- patient/CarePlan.read
- patient/CareTeam.*
- patient/CareTeam.read
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
- patient/Endpoint.*
- patient/Endpoint.read
- patient/ExplanationOfBenefit.*
- patient/ExplanationOfBenefit.read
- patient/Goal.*
- patient/Goal.read
- patient/Immunization.*
- patient/Immunization.read
- patient/Location.*
- patient/Location.read
- patient/Medication.*
- patient/Medication.read
- patient/MedicationDispense.*
- patient/MedicationDispense.read
- patient/MedicationKnowledge.*
- patient/MedicationKnowledge.read
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
- patient/PractitionerRole.*
- patient/PractitionerRole.read
- patient/Procedure.*
- patient/Procedure.read
scopes:
- description: NonPII
  flows:
  - clientCredentials
  scope: NonPII
- description: Public
  flows:
  - clientCredentials
  scope: Public
- description: patient/*.*
  flows:
  - authorizationCode
  scope: patient/*.*
- description: patient/*.read
  flows:
  - authorizationCode
  scope: patient/*.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Allergy.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Allergy.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Binary.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Binary.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/CarePlan.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/CarePlan.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/CareTeam.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/CareTeam.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Condition.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Coverage.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Device.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Device.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/DiagnosticReport.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/DocumentReference.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/DocumentReference.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Encounter.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Endpoint.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Endpoint.read
- description: patient/ExplanationOfBenefit.*
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.*
- description: patient/ExplanationOfBenefit.read
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Goal.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Goal.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Immunization.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Location.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Location.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Medication.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Medication.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/MedicationDispense.read
- description: patient/MedicationKnowledge.*
  flows:
  - authorizationCode
  scope: patient/MedicationKnowledge.*
- description: patient/MedicationKnowledge.read
  flows:
  - authorizationCode
  scope: patient/MedicationKnowledge.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Observation.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Organization.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Organization.read
- description: patient/Patient.*
  flows:
  - authorizationCode
  scope: patient/Patient.*
- description: patient/Patient.read
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Practitioner.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Practitioner.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/PractitionerRole.read
- description: ''
  flows:
  - authorizationCode
  scope: patient/Procedure.*
- description: ''
  flows:
  - authorizationCode
  scope: patient/Procedure.read
slug: aetna-scopes
source_filename: aetna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: openapi/aetna-patient-access-api-openapi.yml, openapi/aetna-provider-directory-api-openapi.yml (derived\n  baseline), upgraded from https://apif1.aetna.com/fhir/.well-known/smart-configuration (HTTP 200, live 2026-08-30),\n  https://apif1.aetna.com/fhir/v2/patientaccess/metadata, and https://developerportal.aetna.com/managedcontent/pdfs/Token_Generation_Process-Patient_Access_APIs-Production.pdf\nschemes:\n- name: FHIR_Patient_Allergy_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Binary_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_CarePlan_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_CareTeam_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRCareTeamRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Condition_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientConditionRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Coverage_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize\n\
  \    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token\n- name: FHIR_Patient_Device_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRDeviceRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_DiagnosticReport_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientDiagnosticReportRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\
  \n\n    }'\n- name: FHIR_Patient_DocumentReference_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientDocumentReferenceRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Encounter_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientEncounterRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Endpoint_Read_AccessCode_Oauth\n\
  \  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientEndpointRead\",\n\n    \"Backend\" : Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\",\n\n    \"Errorhandlingpolicy\": \"Transparent\",\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_EOB_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientEOBRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\",\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Required\"\n\n    }'\n- name: FHIR_Patient_Goal_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientGoalRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Immunization_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_MedicationKnowledge_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize\n    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token\n- name: FHIR_Patient_MedicationRequest_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description:\
  \ '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientMedicationRequestRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Medication_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Observation_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize\n    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token\n- name: FHIR_Patient_Organization_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Patient_Read_AccessCode_Oauth\n \
  \ source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_PractitionerRole_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize\n    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token\n- name: FHIR_Patient_Practitioner_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Procedure_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientProcedureRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between\
  \ Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Allergy_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Binary_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_CarePlan_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_CareTeam_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRCareTeamRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Condition_Read_AccessCode_Oauth\n\
  \  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientConditionRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Coverage_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Device_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRDeviceRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\"\
  \ : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_DiagnosticReport_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientDiagnosticReportRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_DocumentReference_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientDocumentReferenceRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n\
  - name: FHIR_Patient_Encounter_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientEncounterRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Endpoint_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientEndpointRead\",\n\n    \"Backend\" : Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\",\n\n    \"Errorhandlingpolicy\": \"Transparent\",\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_EOB_Read_AccessCode_Oauth\n\
  \  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize\n    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token\n- name: FHIR_Patient_Goal_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientGoalRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_Immunization_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Location_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n\
  \  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_MedicationDispense_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientMedicationDispenseRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_Patient_MedicationRequest_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientMedicationRequestRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\
  \n\n    }'\n- name: FHIR_Patient_Medication_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Observation_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Organization_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Patient_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_PractitionerRole_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://devpih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/authorize\n    tokenUrl: https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token\n- name:\
  \ FHIR_Patient_Practitioner_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n- name: FHIR_Patient_Procedure_Read_AccessCode_Oauth\n  source: openapi/aetna-patient-access-api-sandbox-openapi.yml\n  flows:\n  - flow: authorizationCode\n  description: '{\n\n    \"BuildEieHeader\" : \"Header 3.2\",\n\n    \"SecurityTemplate\" : \"FHIRPatientProcedureRead\",\n\n    \"Backend\" : \"IIB\",\n\n    \"Errorhandlingpolicy\": \"Transparent\"\n\n    \"Consumer\":\"External\",\n\n    \"Mutual Auth between Consumer and APIC\" : \"Not Required\"\n\n    }'\n- name: FHIR_User_AccessCode_Oauth\n  source: openapi/aetna-provider-directory-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/authorize\n    tokenUrl: https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token\n- name: FHIR_Application_Oauth\n  source: openapi/aetna-provider-directory-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://$(catalog.url)/v3/internal/auth/oauth2/app/token\n  description: \"{\\n \\\"BuildEieHeader\\\" : \\\"Header 3.2\\\",\\n \\\"SecurityTemplate\\\" : \\\"FHIROpenApp\\\",\\n \\\"Backend\\\"\\\n    \\ : \\\"Non-IIB, FHIRServer APIGEE APIs, requires Mutual TLS\\\",\\n \\\"Errorhandlingpolicy\\\": \\\"Transparent\\\"\\\n    \\n \\\"Consumer\\\":\\\"External\\\",\\n \\\"Mutual Auth between Consumer and APIC\\\" : \\\"Not Required\\\"\\n}\"\nscopes:\n- scope: NonPII\n  description: NonPII\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aetna-provider-directory-api-openapi.yml\n- scope: Public\n  description: Public\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/aetna-provider-directory-api-openapi.yml\n- scope: patient/*.*\n  description: patient/*.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n  - openapi/aetna-provider-directory-api-openapi.yml\n\
  - scope: patient/*.read\n  description: patient/*.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n  - openapi/aetna-provider-directory-api-openapi.yml\n- scope: patient/Allergy.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Allergy.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Binary.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Binary.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope:\
  \ patient/CarePlan.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/CarePlan.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/CareTeam.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/CareTeam.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Condition.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Condition.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Coverage.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Coverage.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Device.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Device.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/DiagnosticReport.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/DiagnosticReport.read\n\
  \  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/DocumentReference.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/DocumentReference.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Encounter.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Encounter.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Endpoint.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Endpoint.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/ExplanationOfBenefit.*\n  description: patient/ExplanationOfBenefit.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/ExplanationOfBenefit.read\n  description: patient/ExplanationOfBenefit.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Goal.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Goal.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Immunization.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Immunization.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Location.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Location.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Medication.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Medication.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/MedicationDispense.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/MedicationDispense.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/MedicationKnowledge.*\n  description: patient/MedicationKnowledge.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n- scope: patient/MedicationKnowledge.read\n  description: patient/MedicationKnowledge.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n- scope: patient/MedicationRequest.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/MedicationRequest.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Observation.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Observation.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Organization.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Organization.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Patient.*\n  description: patient/Patient.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n\
  \  - openapi/aetna-provider-directory-api-openapi.yml\n- scope: patient/Patient.read\n  description: patient/Patient.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n  - openapi/aetna-provider-directory-api-openapi.yml\n- scope: patient/Practitioner.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Practitioner.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/PractitionerRole.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/PractitionerRole.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n\
  \  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Procedure.*\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\n- scope: patient/Procedure.read\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aetna-patient-access-api-openapi.yml\n  - openapi/aetna-patient-access-api-sandbox-openapi.yml\ndocs: https://apif1.aetna.com/fhir/.well-known/smart-configuration\nprofile: SMART App Launch 1.0.0 scope syntax\nauthorization_server:\n  production:\n    authorization_endpoint: https://apif1.aetna.com/fhir/prod/v1/fhirserver_auth/oauth2/authorize\n    token_endpoint: https://apif1.aetna.com/fhir/prod/v1/fhirserver_auth/oauth2/token\n  sandbox:\n    authorization_endpoint: https://vteapif1.aetna.com/fhirdemo/v1/fhirserver_auth/oauth2/authorize\n    token_endpoint: https://vteapif1.aetna.com/fhirdemo/v1/fhirserver_auth/oauth2/token\n  note: The tokenUrl in every published\
  \ Swagger is the un-substituted IBM API Connect template https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token\n    - not a usable URL. The real endpoints are the ones above, read live from the smart-configuration documents.\n    Aetna's own token-generation PDF and both CapabilityStatements name /fhir/v1/fhirserver_auth/... without\n    the \"prod\" segment; both forms are recorded because Aetna publishes both.\nadvertised_scopes:\n  source: https://apif1.aetna.com/fhir/.well-known/smart-configuration scopes_supported\n  scopes:\n  - openid\n  - fhirUser\n  - profile\n  - launch/patient\n  - patient/*.read\ncapabilities:\n  source: smart-configuration capabilities + Patient Access CapabilityStatement security extensions\n  values:\n  - client-public\n  - client-confidential-symmetric\n  - sso-openid-connect\n  - launch-standalone\n  - context-standalone-patient\n  - permission-patient\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_basic\nscope_families:\n- family: patient/{Resource}.read\n  count: 27\n  description: Per-resource read on the patient in context. Declared per operation in the Swagger securityDefinitions.\n- family: patient/{Resource}.*\n  count: 27\n  description: Per-resource wildcard. Aetna declares these alongside .read even though the surface is read-only.\n- family: patient/*.read\n  description: Read every resource in the patient compartment. The scope Aetna's own token guide tells developers\n    to request, as \"launch/patient patient/*.read\".\n- family: patient/*.*\n  description: Wildcard on everything in the patient compartment.\n- family: Public / NonPII\n  description: Client-credentials scopes on the FHIR_Application_Oauth scheme used by the provider-directory\n    surface, which carries no member data.\ngrant_note: Aetna does not publish a scopes reference page. There is no page to link; the machine-readable\n  smart-configuration document is the closest thing and\
  \ is used as `docs`. Scope descriptions in the schemes[]\n  below are Aetna's own securityDefinitions text, which in many cases repeats the scope string verbatim rather\n  than describing it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aetna/refs/heads/main/scopes/aetna-scopes.yml
summary_line: 54 scopes · authorizationCode/clientCredentials
tags:
- Health Insurance
- Healthcare
- FHIR
- Patient Access
- Provider Directory
- Drug Formulary
- Prior Authorization
- CMS Interoperability
- SMART on FHIR
- CARIN Blue Button
- Da Vinci
- Payer
- Fortune 100
- CVS Health
token_urls:
- https://devapih1.int.aetna.com/healthcare/devpath1/v7/auth/oauth2/token
- https://$(catalog.url)/v1/internal/fhirserver_auth/oauth2/token
- https://$(catalog.url)/v3/internal/auth/oauth2/app/token
---
