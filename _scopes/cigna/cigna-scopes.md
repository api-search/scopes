---
api_specs:
- filename: cigna-bulk-data-api-openapi.yml
  format: yaml
  label: Cigna Bulk Data API
  slug: cigna-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-bulk-data-api-openapi.yml
- filename: cigna-condition-api-openapi.yml
  format: yaml
  label: Cigna Condition API
  slug: cigna-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-condition-api-openapi.yml
- filename: cigna-coverage-api-openapi.yml
  format: yaml
  label: Cigna Coverage API
  slug: cigna-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-coverage-api-openapi.yml
- filename: cigna-encounter-api-openapi.yml
  format: yaml
  label: Cigna Encounter API
  slug: cigna-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-encounter-api-openapi.yml
- filename: cigna-explanationofbenefit-api-openapi.yml
  format: yaml
  label: Cigna ExplanationOfBenefit API
  slug: cigna-explanationofbenefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-explanationofbenefit-api-openapi.yml
- filename: cigna-healthcareservice-api-openapi.yml
  format: yaml
  label: Cigna HealthcareService API
  slug: cigna-healthcareservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-healthcareservice-api-openapi.yml
- filename: cigna-insuranceplan-api-openapi.yml
  format: yaml
  label: Cigna InsurancePlan API
  slug: cigna-insuranceplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-insuranceplan-api-openapi.yml
- filename: cigna-location-api-openapi.yml
  format: yaml
  label: Cigna Location API
  slug: cigna-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-location-api-openapi.yml
- filename: cigna-medicationknowledge-api-openapi.yml
  format: yaml
  label: Cigna MedicationKnowledge API
  slug: cigna-medicationknowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationknowledge-api-openapi.yml
- filename: cigna-medicationrequest-api-openapi.yml
  format: yaml
  label: Cigna MedicationRequest API
  slug: cigna-medicationrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-medicationrequest-api-openapi.yml
- filename: cigna-observation-api-openapi.yml
  format: yaml
  label: Cigna Observation API
  slug: cigna-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-observation-api-openapi.yml
- filename: cigna-organization-api-openapi.yml
  format: yaml
  label: Cigna Organization API
  slug: cigna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-organization-api-openapi.yml
- filename: cigna-patient-api-openapi.yml
  format: yaml
  label: Cigna Patient API
  slug: cigna-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-patient-api-openapi.yml
- filename: cigna-practitioner-api-openapi.yml
  format: yaml
  label: Cigna Practitioner API
  slug: cigna-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitioner-api-openapi.yml
- filename: cigna-practitionerrole-api-openapi.yml
  format: yaml
  label: Cigna PractitionerRole API
  slug: cigna-practitionerrole-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/openapi/cigna-practitionerrole-api-openapi.yml
authorization_urls:
- https://r-hi2.cigna.com/mga/sps/oauth/oauth20/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Cigna Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cigna publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cigna API on a user''s behalf.


  Tokens are issued from https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cigna
provider_slug: cigna
schemes:
- description: SMART on FHIR authorization with patient-context launch
  flows:
  - authorizationUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/authorize
    flow: authorizationCode
    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token
  name: smartOnFhir
  source: openapi/cigna-patient-access-api-openapi.yml
- description: SMART Backend Services authorization for bulk FHIR export
  flows:
  - flow: clientCredentials
    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token
  name: bulkData
  source: openapi/cigna-provider-access-api-openapi.yml
scope_count: 6
scope_names:
- fhirUser
- launch/patient
- offline_access
- openid
- patient/*.read
- system/*.read
scopes:
- description: Receive the user resource identifier
  flows:
  - authorizationCode
  scope: fhirUser
- description: Launch in patient context
  flows:
  - authorizationCode
  scope: launch/patient
- description: Receive a refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Receive an OpenID Connect identity token
  flows:
  - authorizationCode
  scope: openid
- description: Read all patient-context FHIR resources
  flows:
  - authorizationCode
  scope: patient/*.read
- description: System-level read access to FHIR resources
  flows:
  - clientCredentials
  scope: system/*.read
slug: cigna-scopes
source_filename: cigna-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cigna-patient-access-api-openapi.yml, openapi/cigna-provider-access-api-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/cigna-patient-access-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/authorize\n    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token\n  description: SMART on FHIR authorization with patient-context launch\n- name: bulkData\n  source: openapi/cigna-provider-access-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token\n  description: SMART Backend Services authorization for bulk FHIR export\nscopes:\n- scope: fhirUser\n  description: Receive the user resource identifier\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- scope: launch/patient\n  description: Launch in patient context\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- scope: offline_access\n  description: Receive a refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- scope: openid\n  description: Receive an OpenID Connect identity token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- scope: patient/*.read\n  description: Read all patient-context FHIR resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cigna-patient-access-api-openapi.yml\n- scope: system/*.read\n  description: System-level read access to FHIR resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/cigna-provider-access-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cigna/refs/heads/main/scopes/cigna-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
- Fortune 100
token_urls:
- https://r-hi2.cigna.com/mga/sps/oauth/oauth20/token
---
