---
authorization_urls: []
description: 'SMART on FHIR OAuth 2.0 scopes for the Veradigm FHIR R4 API. Derived directly from the live SMART App Launch discovery document served by a Veradigm Connect sandbox tenant (CP00101), fetched unauthenticated on 2026-08-14 (HTTP 200, application/json, 238 scopes). This is a real, Veradigm-published document, not a spec-derived guess: `issuer` is https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization and the raw scopes list is saved verbatim at well-known/allscripts-smart-configuration.json. No OpenAPI/Swagger document exists for this API (see conformance/allscripts-conformance.yml), so this is the strongest available evidence of the real permission surface.'
docs: https://developer.veradigm.com/Fhir/SMARTonFHIR
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Allscripts Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Allscripts uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allscripts
provider_slug: allscripts
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: allscripts-scopes
source_filename: allscripts-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://fhir.fhirpoint.open.allscripts.com/fhirroute/fhir/CP00101/.well-known/smart-configuration\ndocs: https://developer.veradigm.com/Fhir/SMARTonFHIR\ndescription: >-\n  SMART on FHIR OAuth 2.0 scopes for the Veradigm FHIR R4 API. Derived directly from the live\n  SMART App Launch discovery document served by a Veradigm Connect sandbox tenant (CP00101),\n  fetched unauthenticated on 2026-08-14 (HTTP 200, application/json, 238 scopes). This is a real,\n  Veradigm-published document, not a spec-derived guess: `issuer` is\n  https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization and the raw scopes list is\n  saved verbatim at well-known/allscripts-smart-configuration.json. No OpenAPI/Swagger document\n  exists for this API (see conformance/allscripts-conformance.yml), so this is the strongest\n  available evidence of the real permission surface.\nscope_count: 238\nraw_source_file: well-known/allscripts-smart-configuration.json\n\
  \nscheme:\n  standard: SMART App Launch 2.0 / HL7 FHIR scope syntax\n  contexts:\n  - patient   # data scoped to the patient in the launch context\n  - user      # data the launching user (provider) can access\n  - system    # backend/system caller, no launch context (bulk data, server-to-server)\n  suffixes:\n    \"*\": full CRUDS access to the resource type\n    read: read-only, single-resource GET\n    rs: read + search-type (the dominant grant across resources)\n    \"rs?category=...\": category-filtered read+search, used to scope Condition/Observation to a\n      specific US Core category (e.g. laboratory, vital-signs, sdoh, problem-list-item)\n\nresource_scopes:\n  count: 34\n  resources:\n  - \"*\"\n  - AllergyIntolerance\n  - Binary\n  - CarePlan\n  - CareTeam\n  - Condition\n  - Coverage\n  - Device\n  - DiagnosticOrder\n  - DiagnosticReport\n  - DocumentReference\n  - Encounter\n  - Goal\n  - Group\n  - Immunization\n  - Location\n  - Medication\n  - MedicationAdministration\n\
  \  - MedicationDispense\n  - MedicationOrder\n  - MedicationRequest\n  - MedicationStatement\n  - Observation\n  - Organization\n  - Patient\n  - Practitioner\n  - PractitionerRole\n  - Procedure\n  - Provenance\n  - Questionnaire\n  - QuestionnaireResponse\n  - RelatedPerson\n  - ServiceRequest\n  - Specimen\n  note: >-\n    DiagnosticOrder and MedicationOrder appear in scopes_supported as legacy DSTU2-era resource\n    names alongside their R4 successors (ServiceRequest, MedicationRequest) — both scope families\n    are still advertised even though the CapabilityStatement (R4) only declares the current\n    resource types. Veradigm stopped supporting DSTU2 on 2026-06-01 (see lifecycle/).\n\ncategory_filtered_scopes:\n- resource: Condition\n  categories:\n  - http://hl7.org/fhir/us/core/CodeSystem/condition-category|health-concern\n  - http://terminology.hl7.org/CodeSystem/condition-category|encounter-diagnosis\n  - http://terminology.hl7.org/CodeSystem/condition-category|problem-list-item\n\
  - resource: Observation\n  categories:\n  - http://terminology.hl7.org/CodeSystem/observation-category|laboratory\n  - http://terminology.hl7.org/CodeSystem/observation-category|social-history\n  - http://terminology.hl7.org/CodeSystem/observation-category|survey\n  - http://terminology.hl7.org/CodeSystem/observation-category|vital-signs\n- resource: Condition\n  category_system: http://hl7.org/fhir/us/core/CodeSystem/us-core-category\n  code: sdoh\n\nlaunch_and_identity_scopes:\n- launch\n- launch/patient\n- openid\n- fhirUser\n- profile\n- offline_access\n- online_access\n- fhir\n\noauth_endpoints:\n  authorization_endpoint: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/authorize\n  token_endpoint: https://fhir.fhirpoint.open.allscripts.com/fhirroute/authorizationV2/CP00101/connect/token\n  jwks_uri: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization/.well-known/openid-configuration/jwks\n  issuer: https://fhirecho.fhirpoint.open.allscripts.com/pro/authorization\n\
  \  note: >-\n    These are the sandbox tenant CP00101's endpoints. Each production client organization gets its\n    own tenant-specific authorize/token URLs, resolved via the Veradigm Endpoint Directory\n    (https://developer.veradigm.com/Fhir/EndpointDirectory) rather than one fixed host.\n\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n\ncapabilities_supported:\n- launch-ehr\n- launch-standalone\n- client-public\n- client-confidential-symmetric\n- client-confidential-asymmetric\n- context-ehr-patient\n- context-ehr-encounter\n- context-standalone-patient\n- context-standalone-encounter\n- context-passthrough-banner\n- context-passthrough-style\n- context-banner\n- context-style\n- sso-openid-connect\n- permission-offline\n- permission-patient\n- permission-user\n- authorize-post\n- permission-v1\n- permission-v2\n\ncross_links:\n  authentication: authentication/allscripts-authentication.yml\n  conformance: conformance/allscripts-conformance.yml\n\
  \  conventions: conventions/allscripts-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts/refs/heads/main/scopes/allscripts-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Healthcare IT
- EHR
- FHIR
- Clinical Data
- Practice Management
- HL7
token_urls: []
---
