---
authorization_urls:
- https://sandbox-api.va.gov/oauth2/health/v1/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Department Of Veterans Affairs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Department of Veterans Affairs (VA) publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Department of Veterans Affairs (VA) API on a user''s behalf.


  Tokens are issued from https://sandbox-api.va.gov/oauth2/health/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schemes:
- flows:
  - authorizationUrl: https://sandbox-api.va.gov/oauth2/health/v1/authorization
    flow: authorizationCode
    tokenUrl: https://sandbox-api.va.gov/oauth2/health/v1/token
  name: SmartOnFhir
  source: openapi/va-clinical-health-fhir-api-openapi.yml
scope_count: 3
scope_names:
- launch/patient
- offline_access
- patient/*.read
scopes:
- description: Patient context launch
  flows:
  - authorizationCode
  scope: launch/patient
- description: Refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
- description: Read patient-scoped resources
  flows:
  - authorizationCode
  scope: patient/*.read
slug: department-of-veterans-affairs-scopes
source_filename: department-of-veterans-affairs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/va-clinical-health-fhir-api-openapi.yml\nschemes:\n- name: SmartOnFhir\n  source: openapi/va-clinical-health-fhir-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox-api.va.gov/oauth2/health/v1/authorization\n    tokenUrl: https://sandbox-api.va.gov/oauth2/health/v1/token\nscopes:\n- scope: launch/patient\n  description: Patient context launch\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-clinical-health-fhir-api-openapi.yml\n- scope: offline_access\n  description: Refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-clinical-health-fhir-api-openapi.yml\n- scope: patient/*.read\n  description: Read patient-scoped resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/va-clinical-health-fhir-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/scopes/department-of-veterans-affairs-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Federal Government
- Healthcare
- Veterans
token_urls:
- https://sandbox-api.va.gov/oauth2/health/v1/token
---
