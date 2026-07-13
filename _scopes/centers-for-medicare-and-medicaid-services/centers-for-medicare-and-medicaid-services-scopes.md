---
api_specs:
- filename: centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: cms-blue-button-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
authorization_urls:
- https://api.bluebutton.cms.gov/v2/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Centers For Medicare And Medicaid Services Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Centers for Medicare and Medicaid Services publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Centers for Medicare and Medicaid Services API on a user''s behalf.


  Tokens are issued from https://api.bluebutton.cms.gov/v2/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Centers for Medicare and Medicaid Services
provider_slug: centers-for-medicare-and-medicaid-services
schemes:
- description: OAuth 2.0 authorization code flow used by Medicare beneficiaries to grant access to a third-party application.
  flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/
    flow: authorizationCode
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/
  name: oauth2
  source: openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
scope_count: 3
scope_names:
- patient/Coverage.read
- patient/ExplanationOfBenefit.read
- patient/Patient.read
scopes:
- description: Read beneficiary Coverage resources.
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: Read beneficiary claims.
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: Read beneficiary Patient resource.
  flows:
  - authorizationCode
  scope: patient/Patient.read
slug: centers-for-medicare-and-medicaid-services-scopes
source_filename: centers-for-medicare-and-medicaid-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/\n  description: OAuth 2.0 authorization code flow used by Medicare beneficiaries to grant access\n    to a third-party application.\nscopes:\n- scope: patient/Coverage.read\n  description: Read beneficiary Coverage resources.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\n- scope: patient/ExplanationOfBenefit.read\n  description: Read beneficiary claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\n\
  - scope: patient/Patient.read\n  description: Read beneficiary Patient resource.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/scopes/centers-for-medicare-and-medicaid-services-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- BCDA
- Blue Button
- CMS
- Claims
- DPC
- FHIR
- Federal Government
- Healthcare
- Interoperability
- Marketplace
- Medicaid
- Medicare
- Open Data
- Provider Data
- Socrata
token_urls:
- https://api.bluebutton.cms.gov/v2/o/token/
---
