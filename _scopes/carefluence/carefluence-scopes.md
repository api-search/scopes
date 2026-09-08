---
api_specs:
- filename: postman.yaml
  format: yaml
  label: Carefluence Open API R4
  slug: openapi-r4
  spec_type: Postman
  url: https://api.carefluence.com/
authorization_urls: []
description: 'The SMART on FHIR scope set advertised by the Carefluence authorization server at https://core.carefluence.com/cf.admin.core. Every clinical scope is read-only: the server advertises no .write or .* compound write scope, even though the FHIR CapabilityStatement declares create/update/patch interactions on 23 of its 24 resource types.'
docs: https://api.carefluence.com/
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Carefluence Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Carefluence publishes 51 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Carefluence API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Carefluence
provider_slug: carefluence
schemes: []
scope_count: 51
scope_names:
- address
- email
- openid
- phone
- profile
- fhirUser
- launch
- launch/patient
- offline_access
- patient/AllergyIntolerance.read
- patient/CarePlan.read
- patient/CareTeam.read
- patient/Condition.read
- patient/Device.read
- patient/DiagnosticReport.read
- patient/DocumentReference.read
- patient/Encounter.read
- patient/Goal.read
- patient/Immunization.read
- patient/Location.read
- patient/Medication.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Organization.read
- patient/Patient.read
- patient/Practitioner.read
- patient/PractitionerRole.read
- patient/Procedure.read
- patient/Provenance.read
- user/AllergyIntolerance.read
- user/CarePlan.read
- user/CareTeam.read
- user/Condition.read
- user/Device.read
- user/DiagnosticReport.read
- user/DocumentReference.read
- user/Encounter.read
- user/Goal.read
- user/Immunization.read
- user/Medication.read
- user/MedicationRequest.read
- user/Observation.read
- user/Organization.read
- user/Patient.read
- user/Practitioner.read
- user/PractitionerRole.read
- user/Procedure.read
- user/Provenance.read
- system/*.read
- user/Location.read
- patient/*.read
scopes:
- description: Access the address claim.
  flows: []
  scope: address
- description: Access the email and email_verified claims.
  flows: []
  scope: email
- description: Request an OpenID Connect ID token identifying the authorizing user.
  flows: []
  scope: openid
- description: Access the phone and phone_verified claims.
  flows: []
  scope: phone
- description: Access the standard OpenID profile claims (name, family_name, given_name, gender, birthdate, locale and related).
  flows: []
  scope: profile
- description: SMART fhirUser claim identifying the FHIR resource for the logged-in user.
  flows: []
  scope: fhirUser
- description: SMART EHR launch context.
  flows: []
  scope: launch
- description: SMART standalone launch requesting patient context selection.
  flows: []
  scope: launch/patient
- description: Issue a refresh token so the app can act without the user present.
  flows: []
  scope: offline_access
- description: Read every AllergyIntolerance resource in the in-context patient's compartment.
  flows: []
  scope: patient/AllergyIntolerance.read
- description: Read every CarePlan resource in the in-context patient's compartment.
  flows: []
  scope: patient/CarePlan.read
- description: Read every CareTeam resource in the in-context patient's compartment.
  flows: []
  scope: patient/CareTeam.read
- description: Read every Condition resource in the in-context patient's compartment.
  flows: []
  scope: patient/Condition.read
- description: Read every Device resource in the in-context patient's compartment.
  flows: []
  scope: patient/Device.read
- description: Read every DiagnosticReport resource in the in-context patient's compartment.
  flows: []
  scope: patient/DiagnosticReport.read
- description: Read every DocumentReference resource in the in-context patient's compartment.
  flows: []
  scope: patient/DocumentReference.read
- description: Read every Encounter resource in the in-context patient's compartment.
  flows: []
  scope: patient/Encounter.read
- description: Read every Goal resource in the in-context patient's compartment.
  flows: []
  scope: patient/Goal.read
- description: Read every Immunization resource in the in-context patient's compartment.
  flows: []
  scope: patient/Immunization.read
- description: Read every Location resource in the in-context patient's compartment.
  flows: []
  scope: patient/Location.read
- description: Read every Medication resource in the in-context patient's compartment.
  flows: []
  scope: patient/Medication.read
- description: Read every MedicationRequest resource in the in-context patient's compartment.
  flows: []
  scope: patient/MedicationRequest.read
- description: Read every Observation resource in the in-context patient's compartment.
  flows: []
  scope: patient/Observation.read
- description: Read every Organization resource in the in-context patient's compartment.
  flows: []
  scope: patient/Organization.read
- description: Read every Patient resource in the in-context patient's compartment.
  flows: []
  scope: patient/Patient.read
- description: Read every Practitioner resource in the in-context patient's compartment.
  flows: []
  scope: patient/Practitioner.read
- description: Read every PractitionerRole resource in the in-context patient's compartment.
  flows: []
  scope: patient/PractitionerRole.read
- description: Read every Procedure resource in the in-context patient's compartment.
  flows: []
  scope: patient/Procedure.read
- description: Read every Provenance resource in the in-context patient's compartment.
  flows: []
  scope: patient/Provenance.read
- description: Read AllergyIntolerance resources the authorizing user is permitted to see.
  flows: []
  scope: user/AllergyIntolerance.read
- description: Read CarePlan resources the authorizing user is permitted to see.
  flows: []
  scope: user/CarePlan.read
- description: Read CareTeam resources the authorizing user is permitted to see.
  flows: []
  scope: user/CareTeam.read
- description: Read Condition resources the authorizing user is permitted to see.
  flows: []
  scope: user/Condition.read
- description: Read Device resources the authorizing user is permitted to see.
  flows: []
  scope: user/Device.read
- description: Read DiagnosticReport resources the authorizing user is permitted to see.
  flows: []
  scope: user/DiagnosticReport.read
- description: Read DocumentReference resources the authorizing user is permitted to see.
  flows: []
  scope: user/DocumentReference.read
- description: Read Encounter resources the authorizing user is permitted to see.
  flows: []
  scope: user/Encounter.read
- description: Read Goal resources the authorizing user is permitted to see.
  flows: []
  scope: user/Goal.read
- description: Read Immunization resources the authorizing user is permitted to see.
  flows: []
  scope: user/Immunization.read
- description: Read Medication resources the authorizing user is permitted to see.
  flows: []
  scope: user/Medication.read
- description: Read MedicationRequest resources the authorizing user is permitted to see.
  flows: []
  scope: user/MedicationRequest.read
- description: Read Observation resources the authorizing user is permitted to see.
  flows: []
  scope: user/Observation.read
- description: Read Organization resources the authorizing user is permitted to see.
  flows: []
  scope: user/Organization.read
- description: Read Patient resources the authorizing user is permitted to see.
  flows: []
  scope: user/Patient.read
- description: Read Practitioner resources the authorizing user is permitted to see.
  flows: []
  scope: user/Practitioner.read
- description: Read PractitionerRole resources the authorizing user is permitted to see.
  flows: []
  scope: user/PractitionerRole.read
- description: Read Procedure resources the authorizing user is permitted to see.
  flows: []
  scope: user/Procedure.read
- description: Read Provenance resources the authorizing user is permitted to see.
  flows: []
  scope: user/Provenance.read
- description: Backend-services read access across all resource types the client is authorised for.
  flows: []
  scope: system/*.read
- description: Read Location resources the authorizing user is permitted to see.
  flows: []
  scope: user/Location.read
- description: Read every resource in the in-context patient's compartment.
  flows: []
  scope: patient/*.read
slug: carefluence-scopes
source_filename: carefluence-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://core.carefluence.com/cf.admin.core/.well-known/openid-configuration (HTTP 200, fetched 2026-09-02) — scopes_supported read verbatim from the live OpenID Connect discovery document\ndocs: https://api.carefluence.com/  # \"Security & Authorization Flow\" section: \"The Carefluence OpenAPI R4 authorization server uses the scopes defined for Smart on FHIR.\"\nname: Carefluence Open API R4 OAuth scopes\ndescription: >-\n  The SMART on FHIR scope set advertised by the Carefluence authorization\n  server at https://core.carefluence.com/cf.admin.core. Every clinical scope\n  is read-only: the server advertises no .write or .* compound write scope,\n  even though the FHIR CapabilityStatement declares create/update/patch\n  interactions on 23 of its 24 resource types.\nissuer: https://core.carefluence.com/cf.admin.core\nauthorization_endpoint: https://core.carefluence.com/cf.admin.core/connect/authorize\ntoken_endpoint: https://core.carefluence.com/cf.admin.core/connect/token\n\
  scope_syntax: SMART App Launch scopes v1 (<compartment>/<Resource>.<access>)\nscope_count: 51\nscopes:\n- scope: 'address'\n  category: openid-connect\n  description: \"Access the address claim.\"\n- scope: 'email'\n  category: openid-connect\n  description: \"Access the email and email_verified claims.\"\n- scope: 'openid'\n  category: openid-connect\n  description: \"Request an OpenID Connect ID token identifying the authorizing user.\"\n- scope: 'phone'\n  category: openid-connect\n  description: \"Access the phone and phone_verified claims.\"\n- scope: 'profile'\n  category: openid-connect\n  description: \"Access the standard OpenID profile claims (name, family_name, given_name, gender, birthdate, locale and related).\"\n- scope: 'fhirUser'\n  category: openid-connect\n  description: \"SMART fhirUser claim identifying the FHIR resource for the logged-in user.\"\n- scope: 'launch'\n  category: smart-launch-context\n  description: \"SMART EHR launch context.\"\n- scope: 'launch/patient'\n\
  \  category: smart-launch-context\n  description: \"SMART standalone launch requesting patient context selection.\"\n- scope: 'offline_access'\n  category: refresh\n  description: \"Issue a refresh token so the app can act without the user present.\"\n- scope: 'patient/AllergyIntolerance.read'\n  category: smart-patient\n  description: \"Read every AllergyIntolerance resource in the in-context patient's compartment.\"\n- scope: 'patient/CarePlan.read'\n  category: smart-patient\n  description: \"Read every CarePlan resource in the in-context patient's compartment.\"\n- scope: 'patient/CareTeam.read'\n  category: smart-patient\n  description: \"Read every CareTeam resource in the in-context patient's compartment.\"\n- scope: 'patient/Condition.read'\n  category: smart-patient\n  description: \"Read every Condition resource in the in-context patient's compartment.\"\n- scope: 'patient/Device.read'\n  category: smart-patient\n  description: \"Read every Device resource in the in-context patient's\
  \ compartment.\"\n- scope: 'patient/DiagnosticReport.read'\n  category: smart-patient\n  description: \"Read every DiagnosticReport resource in the in-context patient's compartment.\"\n- scope: 'patient/DocumentReference.read'\n  category: smart-patient\n  description: \"Read every DocumentReference resource in the in-context patient's compartment.\"\n- scope: 'patient/Encounter.read'\n  category: smart-patient\n  description: \"Read every Encounter resource in the in-context patient's compartment.\"\n- scope: 'patient/Goal.read'\n  category: smart-patient\n  description: \"Read every Goal resource in the in-context patient's compartment.\"\n- scope: 'patient/Immunization.read'\n  category: smart-patient\n  description: \"Read every Immunization resource in the in-context patient's compartment.\"\n- scope: 'patient/Location.read'\n  category: smart-patient\n  description: \"Read every Location resource in the in-context patient's compartment.\"\n- scope: 'patient/Medication.read'\n  category:\
  \ smart-patient\n  description: \"Read every Medication resource in the in-context patient's compartment.\"\n- scope: 'patient/MedicationRequest.read'\n  category: smart-patient\n  description: \"Read every MedicationRequest resource in the in-context patient's compartment.\"\n- scope: 'patient/Observation.read'\n  category: smart-patient\n  description: \"Read every Observation resource in the in-context patient's compartment.\"\n- scope: 'patient/Organization.read'\n  category: smart-patient\n  description: \"Read every Organization resource in the in-context patient's compartment.\"\n- scope: 'patient/Patient.read'\n  category: smart-patient\n  description: \"Read every Patient resource in the in-context patient's compartment.\"\n- scope: 'patient/Practitioner.read'\n  category: smart-patient\n  description: \"Read every Practitioner resource in the in-context patient's compartment.\"\n- scope: 'patient/PractitionerRole.read'\n  category: smart-patient\n  description: \"Read every PractitionerRole\
  \ resource in the in-context patient's compartment.\"\n- scope: 'patient/Procedure.read'\n  category: smart-patient\n  description: \"Read every Procedure resource in the in-context patient's compartment.\"\n- scope: 'patient/Provenance.read'\n  category: smart-patient\n  description: \"Read every Provenance resource in the in-context patient's compartment.\"\n- scope: 'user/AllergyIntolerance.read'\n  category: smart-user\n  description: \"Read AllergyIntolerance resources the authorizing user is permitted to see.\"\n- scope: 'user/CarePlan.read'\n  category: smart-user\n  description: \"Read CarePlan resources the authorizing user is permitted to see.\"\n- scope: 'user/CareTeam.read'\n  category: smart-user\n  description: \"Read CareTeam resources the authorizing user is permitted to see.\"\n- scope: 'user/Condition.read'\n  category: smart-user\n  description: \"Read Condition resources the authorizing user is permitted to see.\"\n- scope: 'user/Device.read'\n  category: smart-user\n\
  \  description: \"Read Device resources the authorizing user is permitted to see.\"\n- scope: 'user/DiagnosticReport.read'\n  category: smart-user\n  description: \"Read DiagnosticReport resources the authorizing user is permitted to see.\"\n- scope: 'user/DocumentReference.read'\n  category: smart-user\n  description: \"Read DocumentReference resources the authorizing user is permitted to see.\"\n- scope: 'user/Encounter.read'\n  category: smart-user\n  description: \"Read Encounter resources the authorizing user is permitted to see.\"\n- scope: 'user/Goal.read'\n  category: smart-user\n  description: \"Read Goal resources the authorizing user is permitted to see.\"\n- scope: 'user/Immunization.read'\n  category: smart-user\n  description: \"Read Immunization resources the authorizing user is permitted to see.\"\n- scope: 'user/Medication.read'\n  category: smart-user\n  description: \"Read Medication resources the authorizing user is permitted to see.\"\n- scope: 'user/MedicationRequest.read'\n\
  \  category: smart-user\n  description: \"Read MedicationRequest resources the authorizing user is permitted to see.\"\n- scope: 'user/Observation.read'\n  category: smart-user\n  description: \"Read Observation resources the authorizing user is permitted to see.\"\n- scope: 'user/Organization.read'\n  category: smart-user\n  description: \"Read Organization resources the authorizing user is permitted to see.\"\n- scope: 'user/Patient.read'\n  category: smart-user\n  description: \"Read Patient resources the authorizing user is permitted to see.\"\n- scope: 'user/Practitioner.read'\n  category: smart-user\n  description: \"Read Practitioner resources the authorizing user is permitted to see.\"\n- scope: 'user/PractitionerRole.read'\n  category: smart-user\n  description: \"Read PractitionerRole resources the authorizing user is permitted to see.\"\n- scope: 'user/Procedure.read'\n  category: smart-user\n  description: \"Read Procedure resources the authorizing user is permitted to see.\"\
  \n- scope: 'user/Provenance.read'\n  category: smart-user\n  description: \"Read Provenance resources the authorizing user is permitted to see.\"\n- scope: 'system/*.read'\n  category: smart-system\n  description: \"Backend-services read access across all resource types the client is authorised for.\"\n- scope: 'user/Location.read'\n  category: smart-user\n  description: \"Read Location resources the authorizing user is permitted to see.\"\n- scope: 'patient/*.read'\n  category: smart-patient\n  description: \"Read every resource in the in-context patient's compartment.\"\nnotes:\n- >-\n  scopes_supported in the live document lists 52 entries but contains\n  offline_access twice; 51 are distinct.\n- >-\n  patient/*.read and system/*.read wildcards are advertised alongside the\n  per-resource scopes.\n- >-\n  Location is advertised under user/ and patient/ but the CapabilityStatement\n  exposes Location as an open directory-style search; treat scope grants as\n  the authoritative access\
  \ control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carefluence/refs/heads/main/scopes/carefluence-scopes.yml
summary_line: 51 scopes
tags:
- Company
- Healthcare
- Interoperability
- FHIR
- HL7
- SMART on FHIR
- Electronic Health Records
- Clinical Data
- Health IT
- ONC Certified
- USCDI
- OAuth 2.0
- Telehealth
- Health Information Exchange
token_urls: []
---
