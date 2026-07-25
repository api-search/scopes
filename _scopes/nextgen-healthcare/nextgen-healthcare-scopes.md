---
api_specs:
- filename: nextgen-office-fhir-r4-openapi.yaml
  format: yaml
  label: NextGen Office FHIR R4 API
  slug: nextgen-office-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/openapi/nextgen-office-fhir-r4-openapi.yaml
- filename: nextgen-office-bulk-fhir-r4-openapi.yml
  format: yaml
  label: NextGen Office Bulk FHIR R4 API
  slug: nextgen-office-bulk-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/openapi/nextgen-office-bulk-fhir-r4-openapi.yml
authorization_urls:
- https://fhir.nextgen.com/nge/prod/patient-oauth/authorize
- https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/auth
description: SMART-on-FHIR OAuth2 scopes for the NextGen FHIR APIs. Enriched from the live published smart-configuration documents (scopes_supported) for both NextGen Enterprise (patient OAuth) and NextGen Office (Keycloak). NextGen Office advertises the full SMART v2 granular US Core scope set (patient/, user/, system/ prefixes with .r/.s/.rs/.read verbs, plus category-filtered Observation/Condition scopes); the representative families are listed here rather than the full ~350-scope enumeration.
docs:
- https://fhir.nextgen.com/nge/prod/fhir-api-r4/fhir/r4/.well-known/smart-configuration
- https://fhir.meditouchehr.com/api/fhir/r4/.well-known/smart-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Nextgen Healthcare Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'NextGen Healthcare publishes 12 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the NextGen Healthcare API on a user''s behalf.


  Tokens are issued from https://fhir.nextgen.com/nge/prod/patient-oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: NextGen Healthcare
provider_slug: nextgen-healthcare
schemes:
- flows:
  - authorizationUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/authorize
    flow: authorizationCode
    tokenUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/token
  - flow: clientCredentials
    tokenUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/token
  name: SMART-on-FHIR (NextGen Enterprise patient OAuth)
  source: fhir/nextgen-enterprise-r4-smart-configuration.json
- flows:
  - authorizationUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token
  - flow: clientCredentials
    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token
  name: SMART-on-FHIR (NextGen Office, Keycloak realm nextgen)
  source: fhir/nextgen-office-r4-smart-configuration.json
scope_count: 12
scope_names:
- openid
- offline_access
- fhirUser
- launch
- launch/patient
- launch/encounter
- patient/*.*
- user/*.*
- patient/[Resource].rs
- user/[Resource].rs
- system/[Resource].rs
- patient/Observation.rs?category=laboratory
scopes:
- description: OpenID Connect authentication scope
  flows: []
  scope: openid
- description: Request a refresh_token usable while the end-user remains offline
  flows: []
  scope: offline_access
- description: Return the fhirUser claim identifying the authorized user's FHIR resource
  flows: []
  scope: fhirUser
- description: SMART EHR launch context
  flows: []
  scope: launch
- description: Request a patient-scoped access token (standalone launch)
  flows: []
  scope: launch/patient
- description: Request an encounter-scoped access token
  flows: []
  scope: launch/encounter
- description: Full access to all FHIR resources in the patient compartment (Enterprise)
  flows: []
  scope: patient/*.*
- description: Full access to all FHIR resources the user can see (Enterprise)
  flows: []
  scope: user/*.*
- description: SMART v2 granular read+search on a US Core resource in the patient compartment (Office; e.g. patient/Observation.rs)
  flows: []
  scope: patient/[Resource].rs
- description: SMART v2 granular read+search on a US Core resource for the user (Office)
  flows: []
  scope: user/[Resource].rs
- description: SMART Backend Services granular read+search on a US Core resource (Office; client_credentials)
  flows: []
  scope: system/[Resource].rs
- description: Category-filtered granular scope (Office advertises vital-signs, laboratory, social-history, survey, imaging, exam, procedure, activity, therapy, functional-status, cognitive-status, disability-status, sdoh variants)
  flows: []
  scope: patient/Observation.rs?category=laboratory
slug: nextgen-healthcare-scopes
source_filename: nextgen-healthcare-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/nextgen-office-fhir-r4-openapi.yaml\ndocs:\n- https://fhir.nextgen.com/nge/prod/fhir-api-r4/fhir/r4/.well-known/smart-configuration\n- https://fhir.meditouchehr.com/api/fhir/r4/.well-known/smart-configuration\ndescription: >-\n  SMART-on-FHIR OAuth2 scopes for the NextGen FHIR APIs. Enriched from the live published\n  smart-configuration documents (scopes_supported) for both NextGen Enterprise (patient OAuth)\n  and NextGen Office (Keycloak). NextGen Office advertises the full SMART v2 granular US Core\n  scope set (patient/, user/, system/ prefixes with .r/.s/.rs/.read verbs, plus category-filtered\n  Observation/Condition scopes); the representative families are listed here rather than the full\n  ~350-scope enumeration.\nschemes:\n- name: SMART-on-FHIR (NextGen Enterprise patient OAuth)\n  source: fhir/nextgen-enterprise-r4-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/authorize\n\
  \    tokenUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://fhir.nextgen.com/nge/prod/patient-oauth/token\n- name: SMART-on-FHIR (NextGen Office, Keycloak realm nextgen)\n  source: fhir/nextgen-office-r4-smart-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/auth\n    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token\n  - flow: clientCredentials\n    tokenUrl: https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication scope\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json, fhir/nextgen-office-r4-smart-configuration.json]\n- scope: offline_access\n  description: Request a refresh_token usable while the end-user remains offline\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json,\
  \ fhir/nextgen-office-r4-smart-configuration.json]\n- scope: fhirUser\n  description: Return the fhirUser claim identifying the authorized user's FHIR resource\n  sources: [fhir/nextgen-office-r4-smart-configuration.json]\n- scope: launch\n  description: SMART EHR launch context\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json, fhir/nextgen-office-r4-smart-configuration.json]\n- scope: launch/patient\n  description: Request a patient-scoped access token (standalone launch)\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json, fhir/nextgen-office-r4-smart-configuration.json]\n- scope: launch/encounter\n  description: Request an encounter-scoped access token\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json, fhir/nextgen-office-r4-smart-configuration.json]\n- scope: patient/*.*\n  description: Full access to all FHIR resources in the patient compartment (Enterprise)\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json]\n- scope: user/*.*\n\
  \  description: Full access to all FHIR resources the user can see (Enterprise)\n  sources: [fhir/nextgen-enterprise-r4-smart-configuration.json]\n- scope: patient/[Resource].rs\n  description: SMART v2 granular read+search on a US Core resource in the patient compartment (Office; e.g. patient/Observation.rs)\n  sources: [fhir/nextgen-office-r4-smart-configuration.json]\n- scope: user/[Resource].rs\n  description: SMART v2 granular read+search on a US Core resource for the user (Office)\n  sources: [fhir/nextgen-office-r4-smart-configuration.json]\n- scope: system/[Resource].rs\n  description: SMART Backend Services granular read+search on a US Core resource (Office; client_credentials)\n  sources: [fhir/nextgen-office-r4-smart-configuration.json]\n- scope: patient/Observation.rs?category=laboratory\n  description: Category-filtered granular scope (Office advertises vital-signs, laboratory, social-history, survey, imaging, exam, procedure, activity, therapy, functional-status, cognitive-status,\
  \ disability-status, sdoh variants)\n  sources: [fhir/nextgen-office-r4-smart-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextgen-healthcare/refs/heads/main/scopes/nextgen-healthcare-scopes.yml
summary_line: 12 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- United States
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- USCDI
- Bulk FHIR
- Patient Access
- 21st Century Cures
token_urls:
- https://fhir.nextgen.com/nge/prod/patient-oauth/token
- https://idp-prod.prod.ngo.nextgenaws.net/auth/realms/nextgen/protocol/openid-connect/token
---
