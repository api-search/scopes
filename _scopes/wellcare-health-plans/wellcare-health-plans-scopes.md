---
api_specs:
- filename: wellcare-health-plans-condition-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Condition API
  slug: wellcare-health-plans-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-condition-api-openapi.yml
- filename: wellcare-health-plans-coverage-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Coverage API
  slug: wellcare-health-plans-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-coverage-api-openapi.yml
- filename: wellcare-health-plans-encounter-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Encounter API
  slug: wellcare-health-plans-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-encounter-api-openapi.yml
- filename: wellcare-health-plans-explanation-of-benefits-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Explanation of Benefits API
  slug: wellcare-health-plans-explanation-of-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-explanation-of-benefits-api-openapi.yml
- filename: wellcare-health-plans-immunization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Immunization API
  slug: wellcare-health-plans-immunization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-immunization-api-openapi.yml
- filename: wellcare-health-plans-insurance-plan-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Insurance Plan API
  slug: wellcare-health-plans-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-insurance-plan-api-openapi.yml
- filename: wellcare-health-plans-location-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Location API
  slug: wellcare-health-plans-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-location-api-openapi.yml
- filename: wellcare-health-plans-medication-request-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Medication Request API
  slug: wellcare-health-plans-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-medication-request-api-openapi.yml
- filename: wellcare-health-plans-observation-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Observation API
  slug: wellcare-health-plans-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-observation-api-openapi.yml
- filename: wellcare-health-plans-organization-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Organization API
  slug: wellcare-health-plans-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-organization-api-openapi.yml
- filename: wellcare-health-plans-patient-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Patient API
  slug: wellcare-health-plans-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-patient-api-openapi.yml
- filename: wellcare-health-plans-practitioner-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner API
  slug: wellcare-health-plans-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-api-openapi.yml
- filename: wellcare-health-plans-practitioner-role-api-openapi.yml
  format: yaml
  label: wellcare-health-plans Practitioner Role API
  slug: wellcare-health-plans-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/openapi/wellcare-health-plans-practitioner-role-api-openapi.yml
authorization_urls:
- https://partners.centene.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Wellcare Health Plans Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'WellCare Health Plans publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the WellCare Health Plans API on a user''s behalf.


  Tokens are issued from https://partners.centene.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: WellCare Health Plans
provider_slug: wellcare-health-plans
schemes:
- description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.
  flows:
  - authorizationUrl: https://partners.centene.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://partners.centene.com/oauth2/token
  name: smartOnFhir
  source: openapi/wellcare-fhir-patient-access-api-openapi.yml
scope_count: 8
scope_names:
- patient/Condition.read
- patient/Coverage.read
- patient/Encounter.read
- patient/ExplanationOfBenefit.read
- patient/Immunization.read
- patient/MedicationRequest.read
- patient/Observation.read
- patient/Patient.read
scopes:
- description: Read diagnosed conditions
  flows:
  - authorizationCode
  scope: patient/Condition.read
- description: Read coverage and enrollment data
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: Read care encounters
  flows:
  - authorizationCode
  scope: patient/Encounter.read
- description: Read claims and EOB data
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: Read immunization records
  flows:
  - authorizationCode
  scope: patient/Immunization.read
- description: Read medication requests
  flows:
  - authorizationCode
  scope: patient/MedicationRequest.read
- description: Read observations and lab results
  flows:
  - authorizationCode
  scope: patient/Observation.read
- description: Read patient demographic data
  flows:
  - authorizationCode
  scope: patient/Patient.read
slug: wellcare-health-plans-scopes
source_filename: wellcare-health-plans-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wellcare-fhir-patient-access-api-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/wellcare-fhir-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://partners.centene.com/oauth2/authorize\n    tokenUrl: https://partners.centene.com/oauth2/token\n  description: SMART on FHIR OAuth 2.0 authorization for patient-facing apps.\nscopes:\n- scope: patient/Condition.read\n  description: Read diagnosed conditions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Coverage.read\n  description: Read coverage and enrollment data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Encounter.read\n  description: Read care encounters\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n\
  - scope: patient/ExplanationOfBenefit.read\n  description: Read claims and EOB data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Immunization.read\n  description: Read immunization records\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/MedicationRequest.read\n  description: Read medication requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Observation.read\n  description: Read observations and lab results\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n- scope: patient/Patient.read\n  description: Read patient demographic data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/wellcare-fhir-patient-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellcare-health-plans/refs/heads/main/scopes/wellcare-health-plans-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Fortune 500
token_urls:
- https://partners.centene.com/oauth2/token
---
