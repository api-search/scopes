---
api_specs:
- filename: chop-fhir-r4-openapi.yml
  format: yaml
  label: CHOP FHIR R4 API
  slug: chop-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/openapi/chop-fhir-r4-openapi.yml
authorization_urls:
- https://epicnsproxy.chop.edu/fhir/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Childrens Hospital Of Philadelphia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Children''s Hospital of Philadelphia publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Children''s Hospital of Philadelphia API on a user''s behalf.


  Tokens are issued from https://epicnsproxy.chop.edu/fhir/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Children's Hospital of Philadelphia
provider_slug: childrens-hospital-of-philadelphia
schemes:
- flows:
  - authorizationUrl: https://epicnsproxy.chop.edu/fhir/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token
  name: smartOnFhir
  source: openapi/chop-fhir-r4-openapi.yml
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
slug: childrens-hospital-of-philadelphia-scopes
source_filename: childrens-hospital-of-philadelphia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chop-fhir-r4-openapi.yml\nschemes:\n- name: smartOnFhir\n  source: openapi/chop-fhir-r4-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://epicnsproxy.chop.edu/fhir/oauth2/authorize\n    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://epicnsproxy.chop.edu/fhir/oauth2/token\nscopes:\n- scope: fhirUser\n  description: Current FHIR user identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n- scope: launch\n  description: SMART app launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n- scope: offline_access\n  description: Refresh token issuance\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n- scope: openid\n  description: OpenID Connect\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n\
  - scope: profile\n  description: User profile claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n- scope: system/*.read\n  description: System-level read of all resources (Bulk Data)\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/chop-fhir-r4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/childrens-hospital-of-philadelphia/refs/heads/main/scopes/childrens-hospital-of-philadelphia-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Healthcare
- Pediatrics
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Research Data
- Open Data
token_urls:
- https://epicnsproxy.chop.edu/fhir/oauth2/token
---
