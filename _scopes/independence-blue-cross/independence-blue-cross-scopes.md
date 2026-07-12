---
authorization_urls:
- https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Independence Blue Cross Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Independence Blue Cross publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Independence Blue Cross API on a user''s behalf.


  Tokens are issued from https://eapics.ibx.com/oauth2/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Independence Blue Cross
provider_slug: independence-blue-cross
schemes:
- flows:
  - authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://eapics.ibx.com/oauth2/v2/token
  name: smart_on_fhir
  source: openapi/independence-blue-cross-patient-openapi.yml
scope_count: 4
scope_names:
- launch/patient
- offline_access
- openid
- patient/*.read
scopes:
- description: Patient context launch
  flows:
  - authorizationCode
  scope: launch/patient
- description: Long-lived refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
- description: Read all patient-scoped FHIR resources
  flows:
  - authorizationCode
  scope: patient/*.read
slug: independence-blue-cross-scopes
source_filename: independence-blue-cross-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/independence-blue-cross-patient-openapi.yml\nschemes:\n- name: smart_on_fhir\n  source: openapi/independence-blue-cross-patient-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n    tokenUrl: https://eapics.ibx.com/oauth2/v2/token\nscopes:\n- scope: launch/patient\n  description: Patient context launch\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/independence-blue-cross-patient-openapi.yml\n- scope: offline_access\n  description: Long-lived refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/independence-blue-cross-patient-openapi.yml\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/independence-blue-cross-patient-openapi.yml\n- scope: patient/*.read\n  description: Read all patient-scoped FHIR resources\n  flows:\n  - authorizationCode\n\
  \  sources:\n  - openapi/independence-blue-cross-patient-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/scopes/independence-blue-cross-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Healthcare
- Health Insurance
- Blue Cross Blue Shield
- Managed Care
- Medicare
- Medicare Advantage
- Medicaid
- CHIP
- Commercial
- Dental
- Vision
- Behavioral Health
- Pharmacy Benefits
- Interoperability
- FHIR
- SMART On FHIR
- CMS
- Patient Access
- Provider Directory
- Drug Formulary
- Transparency In Coverage
token_urls:
- https://eapics.ibx.com/oauth2/v2/token
---
