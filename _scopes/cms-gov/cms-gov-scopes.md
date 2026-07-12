---
authorization_urls:
- https://api.bluebutton.cms.gov/v2/o/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cms Gov Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CMS — Centers for Medicare & Medicaid Services publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CMS — Centers for Medicare & Medicaid Services API on a user''s behalf.


  Tokens are issued from https://api.bluebutton.cms.gov/v2/o/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CMS — Centers for Medicare & Medicaid Services
provider_slug: cms-gov
schemes:
- flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/
    flow: authorizationCode
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/
  name: OAuth2
  source: openapi/cms-gov-blue-button-2-openapi.yml
scope_count: 5
scope_names:
- patient/Coverage.read
- patient/ExplanationOfBenefit.read
- patient/Patient.read
- profile
- read
scopes:
- description: Read Coverage resources
  flows:
  - authorizationCode
  scope: patient/Coverage.read
- description: Read ExplanationOfBenefit resources
  flows:
  - authorizationCode
  scope: patient/ExplanationOfBenefit.read
- description: Read Patient resource
  flows:
  - authorizationCode
  scope: patient/Patient.read
- description: OpenID profile claims
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows: []
  scope: read
slug: cms-gov-scopes
source_filename: cms-gov-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cms-gov-blue-button-2-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/cms-gov-blue-button-2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/\nscopes:\n- scope: patient/Coverage.read\n  description: Read Coverage resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n- scope: patient/ExplanationOfBenefit.read\n  description: Read ExplanationOfBenefit resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n- scope: patient/Patient.read\n  description: Read Patient resource\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n- scope: profile\n  description: OpenID profile claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n\
  - scope: read\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/scopes/cms-gov-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Healthcare
- Medicare
- Medicaid
- FHIR
- Bulk Data
- Open Data
- Government
- Federal
- Claims
- Insurance
- ACA
- Marketplace
- Quality
token_urls:
- https://api.bluebutton.cms.gov/v2/o/token/
---
