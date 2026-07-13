---
api_specs:
- filename: orion-fhir-openapi.yml
  format: yaml
  label: Orion Health FHIR API
  slug: orion-health-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-fhir-openapi.yml
- filename: orion-population-health-openapi.yml
  format: yaml
  label: Orion Health Population Health API
  slug: orion-health-population-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-population-health-openapi.yml
- filename: orion-hie-openapi.yml
  format: yaml
  label: Orion Health HIE API
  slug: orion-health-hie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-hie-openapi.yml
- filename: orion-rhapsody-openapi.yml
  format: yaml
  label: Orion Health Rhapsody Integration API
  slug: orion-health-rhapsody-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/openapi/orion-rhapsody-openapi.yml
authorization_urls:
- https://auth.orionhealth.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Orion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Orion Health publishes 24 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Orion Health API on a user''s behalf.


  Tokens are issued from https://auth.orionhealth.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Orion Health
provider_slug: orion
schemes:
- description: OAuth 2.0 authorization using SMART on FHIR
  flows:
  - authorizationUrl: https://auth.orionhealth.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  source: openapi/orion-fhir-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  source: openapi/orion-hie-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  source: openapi/orion-population-health-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.orionhealth.com/oauth2/token
  name: oauth2
  source: openapi/orion-rhapsody-openapi.yml
scope_count: 24
scope_names:
- fhirUser
- hie:audit-read
- hie:consent-read
- hie:consent-write
- hie:document-read
- hie:document-write
- hie:notification-manage
- hie:notification-read
- hie:patient-query
- hie:provider-read
- launch
- openid
- patient/*.read
- patient/*.write
- patient/Condition.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
- population-health:admin
- population-health:read
- population-health:write
- rhapsody:admin
- rhapsody:read
- rhapsody:write
scopes:
- description: FHIR user identity
  flows:
  - authorizationCode
  scope: fhirUser
- description: Read audit logs
  flows:
  - clientCredentials
  scope: hie:audit-read
- description: Read consent directives
  flows:
  - clientCredentials
  scope: hie:consent-read
- description: Manage consent directives
  flows:
  - clientCredentials
  scope: hie:consent-write
- description: Retrieve documents
  flows:
  - clientCredentials
  scope: hie:document-read
- description: Submit documents
  flows:
  - clientCredentials
  scope: hie:document-write
- description: Manage notification subscriptions
  flows:
  - clientCredentials
  scope: hie:notification-manage
- description: Read notifications
  flows:
  - clientCredentials
  scope: hie:notification-read
- description: Query patient identity
  flows:
  - clientCredentials
  scope: hie:patient-query
- description: Query provider directory
  flows:
  - clientCredentials
  scope: hie:provider-read
- description: Launch context
  flows:
  - authorizationCode
  scope: launch
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: Read access to all patient data
  flows:
  - authorizationCode
  scope: patient/*.read
- description: Write access to all patient data
  flows:
  - authorizationCode
  scope: patient/*.write
- description: Read access to Condition resources
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read access to MedicationRequest resources
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read access to Observation resources
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read access to Patient resources
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: Administrative access
  flows:
  - clientCredentials
  scope: population-health:admin
- description: Read population health data
  flows:
  - clientCredentials
  scope: population-health:read
- description: Write population health data
  flows:
  - clientCredentials
  scope: population-health:write
- description: Administrative access
  flows:
  - clientCredentials
  scope: rhapsody:admin
- description: Read access to Rhapsody engine
  flows:
  - clientCredentials
  scope: rhapsody:read
- description: Write access to Rhapsody engine
  flows:
  - clientCredentials
  scope: rhapsody:write
slug: orion-scopes
source_filename: orion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orion-fhir-openapi.yml, openapi/orion-hie-openapi.yml, openapi/orion-population-health-openapi.yml,\n  openapi/orion-rhapsody-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/orion-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.orionhealth.com/oauth2/authorize\n    tokenUrl: https://auth.orionhealth.com/oauth2/token\n  description: OAuth 2.0 authorization using SMART on FHIR\n- name: oauth2\n  source: openapi/orion-hie-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.orionhealth.com/oauth2/token\n- name: oauth2\n  source: openapi/orion-population-health-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.orionhealth.com/oauth2/token\n- name: oauth2\n  source: openapi/orion-rhapsody-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.orionhealth.com/oauth2/token\nscopes:\n- scope: fhirUser\n\
  \  description: FHIR user identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: hie:audit-read\n  description: Read audit logs\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:consent-read\n  description: Read consent directives\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:consent-write\n  description: Manage consent directives\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:document-read\n  description: Retrieve documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:document-write\n  description: Submit documents\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:notification-manage\n  description: Manage notification subscriptions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n\
  - scope: hie:notification-read\n  description: Read notifications\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:patient-query\n  description: Query patient identity\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: hie:provider-read\n  description: Query provider directory\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-hie-openapi.yml\n- scope: launch\n  description: Launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: patient/*.read\n  description: Read access to all patient data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: patient/*.write\n  description: Write access to all patient data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n\
  - scope: patient/Condition.read\n  description: Read access to Condition resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read access to MedicationRequest resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: patient/Observation.read\n  description: Read access to Observation resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: patient/Patient.read\n  description: Read access to Patient resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/orion-fhir-openapi.yml\n- scope: population-health:admin\n  description: Administrative access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-population-health-openapi.yml\n- scope: population-health:read\n  description: Read population health data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-population-health-openapi.yml\n\
  - scope: population-health:write\n  description: Write population health data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-population-health-openapi.yml\n- scope: rhapsody:admin\n  description: Administrative access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-rhapsody-openapi.yml\n- scope: rhapsody:read\n  description: Read access to Rhapsody engine\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-rhapsody-openapi.yml\n- scope: rhapsody:write\n  description: Write access to Rhapsody engine\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/orion-rhapsody-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orion/refs/heads/main/scopes/orion-scopes.yml
summary_line: 24 scopes · authorizationCode/clientCredentials
tags:
- EHR
- FHIR
- Health IT
- Healthcare
- HIE
- HL7
- Integration
- Interoperability
- Population Health
token_urls:
- https://auth.orionhealth.com/oauth2/token
---
