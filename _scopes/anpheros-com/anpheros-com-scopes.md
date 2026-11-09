---
api_specs:
- filename: anpheros-com-access-requests-api-openapi.yml
  format: yaml
  label: anpheros-com Access requests API
  slug: anpheros-com-access-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-access-requests-api-openapi.yml
- filename: anpheros-com-admin-api-openapi.yml
  format: yaml
  label: anpheros-com Admin API
  slug: anpheros-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-admin-api-openapi.yml
- filename: anpheros-com-anpheros-search-api-openapi.yml
  format: yaml
  label: anpheros-com Anpheros Search API
  slug: anpheros-com-anpheros-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-anpheros-search-api-openapi.yml
- filename: anpheros-com-fhir-r4-api-openapi.yml
  format: yaml
  label: anpheros-com FHIR R4 API
  slug: anpheros-com-fhir-r4-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-fhir-r4-api-openapi.yml
- filename: anpheros-com-icd-10-to-icd-11-api-openapi.yml
  format: yaml
  label: anpheros-com ICD-10 to ICD-11 API
  slug: anpheros-com-icd-10-to-icd-11-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-icd-10-to-icd-11-api-openapi.yml
- filename: anpheros-com-oauth-api-openapi.yml
  format: yaml
  label: anpheros-com OAuth API
  slug: anpheros-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-oauth-api-openapi.yml
- filename: anpheros-com-patient-me-api-openapi.yml
  format: yaml
  label: anpheros-com Patient (me) API
  slug: anpheros-com-patient-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-patient-me-api-openapi.yml
- filename: anpheros-com-rest-v1-api-openapi.yml
  format: yaml
  label: anpheros-com REST v1 API
  slug: anpheros-com-rest-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-rest-v1-api-openapi.yml
- filename: anpheros-com-smart-health-links-api-openapi.yml
  format: yaml
  label: anpheros-com SMART Health Links API
  slug: anpheros-com-smart-health-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-smart-health-links-api-openapi.yml
- filename: anpheros-com-webhooks-api-openapi.yml
  format: yaml
  label: anpheros-com Webhooks API
  slug: anpheros-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anpheros-com/openapi/anpheros-com-webhooks-api-openapi.yml
authorization_urls:
- https://platform.anpheros.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Anpheros Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'anpheros-com publishes 11 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the anpheros-com API on a user''s behalf.


  Tokens are issued from https://platform.anpheros.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: anpheros-com
provider_slug: anpheros-com
schemes:
- description: SMART on FHIR v2 scopes; authorization code with PKCE for a person's record, client_credentials for a project.
  flows:
  - authorizationUrl: https://platform.anpheros.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://platform.anpheros.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://platform.anpheros.com/oauth/token
  name: oauth2
  source: openapi/anpheros-com-openapi.json
scope_count: 11
scope_names:
- anpheros/patterns
- fhirUser
- offline_access
- openid
- patient/*.rs
- patient/AllergyIntolerance.rs
- patient/Condition.rs
- patient/DocumentReference.rs
- patient/MedicationStatement.rs
- patient/Observation.rs
- patient/Observation.rs?category=laboratory
scopes:
- description: Pattern analysis on production records (separate patient consent)
  flows:
  - authorizationCode
  scope: anpheros/patterns
- description: Identity of the person
  flows:
  - authorizationCode
  scope: fhirUser
- description: Refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Read the whole record
  flows:
  - authorizationCode
  scope: patient/*.rs
- description: Read allergies
  flows:
  - authorizationCode
  scope: patient/AllergyIntolerance.rs
- description: Read conditions
  flows:
  - authorizationCode
  scope: patient/Condition.rs
- description: Read documents
  flows:
  - authorizationCode
  scope: patient/DocumentReference.rs
- description: Read medications
  flows:
  - authorizationCode
  scope: patient/MedicationStatement.rs
- description: Read measurements and lab results
  flows:
  - authorizationCode
  scope: patient/Observation.rs
- description: Read lab results only
  flows:
  - authorizationCode
  scope: patient/Observation.rs?category=laboratory
slug: anpheros-com-scopes
source_filename: anpheros-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/anpheros-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/anpheros-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.anpheros.com/oauth/authorize\n    tokenUrl: https://platform.anpheros.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://platform.anpheros.com/oauth/token\n  description: SMART on FHIR v2 scopes; authorization code with PKCE for a person's record,\n    client_credentials for a project.\nscopes:\n- scope: anpheros/patterns\n  description: Pattern analysis on production records (separate patient consent)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: fhirUser\n  description: Identity of the person\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: offline_access\n  description: Refresh token\n  flows:\n  - authorizationCode\n  sources:\n  -\
  \ openapi/anpheros-com-openapi.json\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/*.rs\n  description: Read the whole record\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/AllergyIntolerance.rs\n  description: Read allergies\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/Condition.rs\n  description: Read conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/DocumentReference.rs\n  description: Read documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/MedicationStatement.rs\n  description: Read medications\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/Observation.rs\n  description: Read measurements and lab\
  \ results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n- scope: patient/Observation.rs?category=laboratory\n  description: Read lab results only\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/anpheros-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/anpheros-com/scopes/anpheros-com-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials
tags:
- Health
- Digital Health
- FHIR
- Medical Records
token_bound: false
token_urls:
- https://platform.anpheros.com/oauth/token
---
