---
authorization_urls:
- https://api.practicefusion.com/fhir/r4/v1/{organizationId}/authorize
description: ''
docs: https://www.practicefusion.com/fhir/api-specifications/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Practice Fusion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Practice Fusion uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Practice Fusion
provider_slug: practice-fusion
schemes:
- flows:
  - authorizationUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/authorize
    flow: authorizationCode
    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
  - flow: clientCredentials
    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
  name: SMART-on-FHIR OAuth2
  source: smart-configuration
scope_count: 0
scope_names: []
scopes: []
slug: practice-fusion-scopes
source_filename: practice-fusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/.well-known/smart-configuration\ndocs: https://www.practicefusion.com/fhir/api-specifications/\nmodel: SMART on FHIR v2 (SMART App Launch 2.0.0)\nnotes: >-\n  Practice Fusion uses SMART-on-FHIR v2 scopes (the SMART configuration advertises\n  permission-v1, permission-v2, permission-patient, permission-user, and\n  permission-offline capabilities). Resource-level scopes follow the SMART v2\n  grammar `<context>/<Resource>.<cruds>` where context is patient, user, or\n  system, Resource is any of the 47 supported FHIR R4 resource types (or `*`),\n  and cruds is a subset of c-r-u-d-s. The API is predominantly read/search\n  (read + search-type on all resources), so `.rs` is the operative access.\nschemes:\n- name: SMART-on-FHIR OAuth2\n  source: smart-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/authorize\n\
  \    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token\n  - flow: clientCredentials\n    tokenUrl: https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token\nidentity_scopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an id_token.\n- scope: fhirUser\n  description: Returns the FHIR resource representing the current user.\n- scope: profile\n  description: OpenID profile claim.\n- scope: offline_access\n  description: Requests a refresh token for long-lived access (permission-offline).\n- scope: launch\n  description: EHR launch context (launch-ehr).\n- scope: launch/patient\n  description: Standalone launch scoped to a selected patient.\n- scope: launch/encounter\n  description: Standalone launch scoped to a selected encounter.\nscope_patterns:\n- pattern: patient/{Resource}.rs\n  description: Read + search a resource type in the patient compartment (v2 grammar).\n  example: patient/Observation.rs\n- pattern: user/{Resource}.rs\n\
  \  description: Read + search a resource type in the authorized user's context.\n  example: user/Condition.rs\n- pattern: system/{Resource}.rs\n  description: Backend (client_credentials) read + search access to a resource type.\n  example: system/Patient.rs\n- pattern: patient/*.rs\n  description: Read + search across all patient-compartment resources.\nsupported_resources:\n- AllergyIntolerance\n- CarePlan\n- CareTeam\n- Condition\n- Coverage\n- Device\n- DiagnosticReport\n- DocumentReference\n- Encounter\n- Goal\n- Immunization\n- Location\n- Medication\n- MedicationRequest\n- Observation\n- Organization\n- Patient\n- Practitioner\n- PractitionerRole\n- Procedure\n- Provenance\n- RelatedPerson\n- ServiceRequest\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/practice-fusion/refs/heads/main/scopes/practice-fusion-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Healthcare
- Electronic Health Records
- EHR
- FHIR
- Interoperability
- Medical
- Health IT
- SMART on FHIR
- Clinical Data
token_urls:
- https://api.practicefusion.com/fhir/r4/v1/{organizationId}/token
---
