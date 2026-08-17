---
api_specs:
- filename: meditech-allergy-api-openapi.yml
  format: yaml
  label: meditech Allergy API
  slug: meditech-allergy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-allergy-api-openapi.yml
- filename: meditech-capability-api-openapi.yml
  format: yaml
  label: meditech Capability API
  slug: meditech-capability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-capability-api-openapi.yml
- filename: meditech-condition-api-openapi.yml
  format: yaml
  label: meditech Condition API
  slug: meditech-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-condition-api-openapi.yml
- filename: meditech-diagnostic-api-openapi.yml
  format: yaml
  label: meditech Diagnostic API
  slug: meditech-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-diagnostic-api-openapi.yml
- filename: meditech-encounter-api-openapi.yml
  format: yaml
  label: meditech Encounter API
  slug: meditech-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-encounter-api-openapi.yml
- filename: meditech-medication-api-openapi.yml
  format: yaml
  label: meditech Medication API
  slug: meditech-medication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-medication-api-openapi.yml
- filename: meditech-observation-api-openapi.yml
  format: yaml
  label: meditech Observation API
  slug: meditech-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-observation-api-openapi.yml
- filename: meditech-patient-api-openapi.yml
  format: yaml
  label: meditech Patient API
  slug: meditech-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-patient-api-openapi.yml
authorization_urls:
- https://greenfield-prod-apis.meditech.com/oauth/authorize
description: ''
docs: https://greenfield.meditech.com/explorer/scope
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Meditech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MEDITECH uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://greenfield-prod-apis.meditech.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MEDITECH
provider_slug: meditech
schemes:
- description: SMART on FHIR OAuth 2.0 authorization -- Greenfield Workspace sandbox (live, first-party)
  flows:
  - authorizationUrl: https://greenfield-prod-apis.meditech.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://greenfield-prod-apis.meditech.com/oauth/token
  name: SMART_OAuth2
  source: well-known/meditech-greenfield-smart-configuration.json
scope_count: 0
scope_names: []
scopes: []
slug: meditech-scopes
source_filename: meditech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://greenfield-prod-apis.meditech.com/.well-known/smart-configuration\ndocs: https://greenfield.meditech.com/explorer/scope\nx-provenance:\n  reviewed: '2026-08-14'\n  origin: first-party-probed\n  upgrade_note: 'This file previously carried only 5 scopes derived from an API Evangelist model of US\n    Core FHIR R4 (method: derived). It is now upgraded to the REAL, complete scope list MEDITECH''s own\n    Greenfield sandbox authorization server advertises, read live from its SMART-on-FHIR discovery document\n    on 2026-08-06/2026-08-14 (greenfield-prod-apis.meditech.com/.well-known/smart-configuration) after\n    API Evangelist was issued sandbox credentials on 2026-07-27. This is MEDITECH''s own server telling\n    us what it supports, not an inference from documentation. The Explorer''s human-readable scope reference\n    page (docs: above) could not be fetched -- it is a robots-disallowed, client-rendered Angular SPA\n\
  \    -- so this discovery document is the strongest available substitute for it, and arguably stronger\n    since it is the literal contract rather than prose describing one.'\n  caveat: 'scopes_supported on a discovery document is a statement of what the AUTHORIZATION SERVER will\n    grant if asked, not of what a given client is entitled to receive, and not all 581 scopes are meant\n    for third-party app developers. Roughly 173 begin with infr-/iops-/mis-/unv- prefixes that read as\n    MEDITECH-internal administrative and infrastructure scopes (e.g. infr-tls-config/*, iops-admin) --\n    grouped separately below rather than discarded, since we cannot confirm from outside MEDITECH which\n    of them a developer could ever be granted. The confirmed grant_reality documented in authentication/meditech-greenfield-oauth.yml\n    applies here too: client_credentials is ADVERTISED but was NOT enabled for the sandbox client actually\n    tested.'\ntotal_advertised: 581\nschemes:\n- name: SMART_OAuth2\n\
  \  source: well-known/meditech-greenfield-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://greenfield-prod-apis.meditech.com/oauth/authorize\n    tokenUrl: https://greenfield-prod-apis.meditech.com/oauth/token\n  description: SMART on FHIR OAuth 2.0 authorization -- Greenfield Workspace sandbox (live, first-party)\noidc_scopes:\n  description: Standard OpenID Connect scopes advertised alongside SMART launch context.\n  scopes:\n  - openid\n  - profile\n  - email\n  - phone\n  - address\n  - fhirUser\n  - online_access\n  - offline_access\nlaunch_context_scopes:\n  description: SMART launch-context scopes advertised by the sandbox authorization server.\n  scopes:\n  - launch\n  - launch/encounter\n  - launch/location\n  - launch/patient\npatient_read_scopes:\n  description: US Core / Argonaut resource-level patient/*.read scopes (38 advertised) -- the scopes a\n    patient-facing app actually needs.\n  count: 38\n  scopes:\n  - patient/*.read\n\
  \  - patient/AllergyIntolerance.read\n  - patient/Appointment.read\n  - patient/ArgoScheduling.read\n  - patient/Binary.read\n  - patient/CarePlan.read\n  - patient/CareTeam.read\n  - patient/Communication.read\n  - patient/Condition.read\n  - patient/Coverage.read\n  - patient/Device.read\n  - patient/DiagnosticReport.read\n  - patient/DocumentReference.read\n  - patient/Encounter.read\n  - patient/Goal.read\n  - patient/Group.read\n  - patient/Immunization.read\n  - patient/Location.read\n  - patient/Media.read\n  - patient/Medication.read\n  - patient/MedicationAdministration.read\n  - patient/MedicationDispense.read\n  - patient/MedicationOrder.read\n  - patient/MedicationRequest.read\n  - patient/MedicationStatement.read\n  - patient/Observation.read\n  - patient/Organization.read\n  - patient/Patient.read\n  - patient/Practitioner.read\n  - patient/PractitionerRole.read\n  - patient/Procedure.read\n  - patient/Provenance.read\n  - patient/QuestionnaireResponse.read\n  - patient/RelatedPerson.read\n\
  \  - patient/ServiceRequest.read\n  - patient/Specimen.read\n  - patient/Task.read\n  - patient/ValueSet.read\npatient_other_scopes:\n  description: Non-.read patient/* scopes advertised -- includes write-capable and combined-permission\n    forms (e.g. patient/Communication.write, patient/QuestionnaireResponse.crus) matching the two writable\n    resources confirmed live in conformance/meditech-greenfield-conformance.yml (Communication, QuestionnaireResponse),\n    plus legacy Argonaut-shorthand scopes MEDITECH still advertises (e.g. patient/Condition.rs) that this\n    repo has not independently confirmed grant.\n  count: 41\n  scopes:\n  - patient/AllergyIntolerance.rs\n  - patient/ArgoScheduling.*\n  - patient/Binary.r\n  - patient/CarePlan.rs\n  - patient/CareTeam.rs\n  - patient/Communication.crs\n  - patient/Communication.write\n  - patient/Condition.crs\n  - patient/Coverage.rs\n  - patient/Device.rs\n  - patient/DiagnosticReport.rs\n  - patient/DocumentReference.crus\n  - patient/DocumentReference.write\n\
  \  - patient/Encounter.rs\n  - patient/Goal.rs\n  - patient/Group.crus\n  - patient/Immunization.rs\n  - patient/Location.rs\n  - patient/Media.r\n  - patient/Medication.rs\n  - patient/MedicationAdministration.rs\n  - patient/MedicationDispense.rs\n  - patient/MedicationRequest.rs\n  - patient/MedicationStatement.rs\n  - patient/Observation.crus\n  - patient/Observation.write\n  - patient/Organization.rs\n  - patient/Patient.crus\n  - patient/Person.rs\n  - patient/Practitioner.rs\n  - patient/PractitionerRole.rs\n  - patient/Procedure.rs\n  - patient/Provenance.rs\n  - patient/QuestionnaireResponse.crus\n  - patient/QuestionnaireResponse.write\n  - patient/RelatedPerson.rs\n  - patient/ServiceRequest.rs\n  - patient/Specimen.rs\n  - patient/Task.rs\n  - patient/Task.write\n  - patient/ValueSet.r\nuser_read_scopes:\n  description: Practitioner-context user/*.read scopes (38 advertised).\n  count: 38\n  scopes:\n  - user/AllergyIntolerance.read\n  - user/Appointment.read\n  - user/Binary.read\n\
  \  - user/CarePlan.read\n  - user/CareTeam.read\n  - user/Communication.read\n  - user/Condition.read\n  - user/Coverage.read\n  - user/Device.read\n  - user/DiagnosticReport.read\n  - user/DocumentReference.read\n  - user/Encounter.read\n  - user/Goal.read\n  - user/Group.read\n  - user/Immunization.read\n  - user/Location.read\n  - user/Media.read\n  - user/Medication.read\n  - user/MedicationAdministration.read\n  - user/MedicationDispense.read\n  - user/MedicationOrder.read\n  - user/MedicationRequest.read\n  - user/MedicationStatement.read\n  - user/Observation.read\n  - user/Organization.read\n  - user/Patient.read\n  - user/Practitioner.read\n  - user/PractitionerRole.read\n  - user/Procedure.read\n  - user/Provenance.read\n  - user/QuestionnaireResponse.read\n  - user/RelatedPerson.read\n  - user/ServiceRequest.read\n  - user/Specimen.read\n  - user/Task.read\n  - user/ValueSet.read\n  - user/metadata.read\n  - user/wellknown.read\nsystem_scopes:\n  description: 'system/* scopes\
  \ (75 advertised) for backend/client_credentials access. CAUTION: authentication/meditech-greenfield-oauth.yml\n    documents that client_credentials was tested and returned HTTP 400 unauthorized_client for the issued\n    sandbox client -- these scopes are advertised, not confirmed grantable in the complimentary sandbox\n    tier.'\n  count: 75\n  scopes:\n  - system/AllergyIntolerance.rs\n  - system/Binary.r\n  - system/CarePlan.rs\n  - system/CareTeam.rs\n  - system/Communication.crs\n  - system/Condition.crs\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|care-experience-preference\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|cognitive-status\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|disability-status\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|functional-status\n\
  \  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  - system/Condition.crs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|treatment-intervention-preference\n  - system/Condition.crs?category=http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  - system/Condition.crs?category=http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n  - system/Coverage.rs\n  - system/Device.rs\n  - system/DiagnosticReport.rs\n  - system/DiagnosticReport.rs?category=http://loinc.org|LP29684-5\n  - system/DiagnosticReport.rs?category=http://loinc.org|LP29708-2\n  - system/DiagnosticReport.rs?category=http://loinc.org|LP7839-6\n  - system/DiagnosticReport.rs?category=http://terminology.hl7.org/CodeSystem/v2-0074|LAB\n  - system/DocumentReference.crus\n  - system/DocumentReference.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-documentreference-category|clinical-note\n  - system/Encounter.rs\n\
  \  - system/Goal.rs\n  - system/Group.crus\n  - system/Immunization.rs\n  - system/Location.rs\n  - system/Media.r\n  - system/Medication.rs\n  - system/MedicationAdministration.rs\n  - system/MedicationDispense.rs\n  - system/MedicationRequest.rs\n  - system/MedicationStatement.rs\n  - system/Observation.crus\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|care-experience-preference\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|cognitive-status\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|disability-status\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|functional-status\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  - system/Observation.crus?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|treatment-intervention-preference\n  -\
  \ system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|activity\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|imaging\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|procedure\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|survey\n  - system/Observation.crus?category=http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n  - system/Organization.rs\n  - system/Patient.crus\n  - system/Person.rs\n  - system/Practitioner.rs\n  - system/PractitionerRole.rs\n  - system/Procedure.rs\n  - system/Provenance.rs\n  - system/QuestionnaireResponse.crus\n  - system/RelatedPerson.rs\n\
  \  - system/ServiceRequest.rs\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|care-experience-preference\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|cognitive-status\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|disability-status\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|functional-status\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|sdoh\n  - system/ServiceRequest.rs?category=http://hl7.org/fhir/us/core/CodeSystem/us-core-category|treatment-intervention-preference\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|108252007\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|363679005\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|386053000\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|387713003\n\
  \  - system/ServiceRequest.rs?category=http://snomed.info/sct|409063005\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|409073007\n  - system/ServiceRequest.rs?category=http://snomed.info/sct|410606002\n  - system/Specimen.rs\n  - system/Task.rs\n  - system/ValueSet.r\ninternal_administrative_scopes_count: 377\ninternal_administrative_scopes_note: The remainder are infr-*/iops-*/mis-*/unv-* prefixed scopes that\n  read as MEDITECH-internal infrastructure/administration surface, not third-party app scopes. Full raw\n  list preserved verbatim in well-known/meditech-greenfield-smart-configuration.json (scopes_supported)\n  rather than duplicated here.\nlegacy_model_scopes:\n  note: The 5 scopes below are what this repo previously derived from an API Evangelist model of US Core\n    FHIR R4 (openapi/*-openapi.yml), kept for traceability. They are a strict subset of the confirmed\n    live list above.\n  scopes:\n  - scope: fhirUser\n    description: FHIR user claim\n  - scope:\
  \ launch\n    description: EHR launch context\n  - scope: openid\n    description: OpenID Connect identity\n  - scope: patient/*.read\n    description: Read access to all patient-owned resources\n  - scope: user/*.read\n    description: Practitioner read access to all resources\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/scopes/meditech-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- EHR
- Healthcare
- FHIR
- HL7
- Interoperability
token_urls:
- https://greenfield-prod-apis.meditech.com/oauth/token
---
