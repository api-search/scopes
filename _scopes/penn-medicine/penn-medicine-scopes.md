---
api_specs:
- filename: penn-medicine-fhir-r4-openapi.yml
  format: yaml
  label: Penn Medicine FHIR R4 API
  slug: penn-medicine-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/openapi/penn-medicine-fhir-r4-openapi.yml
authorization_urls:
- https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Penn Medicine Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Penn Medicine publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Penn Medicine API on a user''s behalf.


  Tokens are issued from https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Penn Medicine
provider_slug: penn-medicine
schemes:
- flows:
  - authorizationUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token
  name: smartOnFhir
  source: openapi/penn-medicine-fhir-r4-openapi.yml
scope_count: 6
scope_names:
- fhirUser
- launch
- offline_access
- openid
- profile
- system/*.read
scopes:
- description: Current FHIR user identity
  flows:
  - authorizationCode
  scope: fhirUser
- description: SMART app launch context
  flows:
  - authorizationCode
  scope: launch
- description: Refresh token issuance
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect
  flows:
  - authorizationCode
  scope: openid
- description: User profile claims
  flows:
  - authorizationCode
  scope: profile
- description: System-level read of all resources (Bulk Data)
  flows:
  - clientCredentials
  scope: system/*.read
slug: penn-medicine-scopes
source_filename: penn-medicine-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/penn-medicine-fhir-r4-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/penn-medicine-fhir-r4-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/authorize\n    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token\nscopes:\n- scope: fhirUser\n  description: Current FHIR user identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n- scope: launch\n  description: SMART app launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n- scope: offline_access\n  description: Refresh token issuance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n- scope: profile\n  description: User profile claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n- scope: system/*.read\n  description: System-level read of all resources (Bulk Data)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/penn-medicine-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/scopes/penn-medicine-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- Hospital
- Academic Medical Center
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Epic
token_urls:
- https://ssproxy.pennhealth.com/PRD-FHIR/oauth2/token
---
