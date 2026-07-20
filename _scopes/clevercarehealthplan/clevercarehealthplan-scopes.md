---
api_specs:
- filename: clevercarehealthplan-fhir-openapi.yml
  format: yaml
  label: Clever Care Health Plan FHIR R4 API
  slug: clever-care-health-plan-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/openapi/clevercarehealthplan-fhir-openapi.yml
authorization_urls:
- https://fhir-portal.clevercarehealthplan.com/oauth2/authorize
description: ''
docs: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Clevercarehealthplan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Clever Care Health Plan publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clever Care Health Plan API on a user''s behalf.


  Tokens are issued from https://fhir-portal.clevercarehealthplan.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clever Care Health Plan
provider_slug: clevercarehealthplan
schemes:
- description: SMART-on-FHIR OAuth 2.0 (PKCE S256), OpenID Connect enabled.
  flows:
  - authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token
  name: smartOnFhir
  source: openapi/clevercarehealthplan-fhir-openapi.yml
scope_count: 4
scope_names:
- launch/patient
- openid
- patient/*.cruds
- user/*.cruds
scopes:
- description: Launch in patient context
  flows:
  - authorizationCode
  scope: launch/patient
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  - clientCredentials
  scope: openid
- description: Patient-scoped access to permitted resources
  flows:
  - authorizationCode
  scope: patient/*.cruds
- description: User-scoped access to permitted resources
  flows:
  - authorizationCode
  - clientCredentials
  scope: user/*.cruds
slug: clevercarehealthplan-scopes
source_filename: clevercarehealthplan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/clevercarehealthplan-fhir-openapi.yml\ndocs: https://fhir.clevercarehealthplan.com/r4/.well-known/smart-configuration\nnotes: >-\n  Scopes confirmed verbatim from the server SMART-on-FHIR discovery document\n  (scopes_supported). SMART v2 wildcard scopes; patient/user CRUDS. Patient\n  Access resources (Patient, ExplanationOfBenefit, Coverage) require patient/*\n  or user/* scope; Provider Directory and Drug Formulary resources are public.\nschemes:\n- name: smartOnFhir\n  source: openapi/clevercarehealthplan-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/authorize\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://fhir-portal.clevercarehealthplan.com/oauth2/token\n  description: SMART-on-FHIR OAuth 2.0 (PKCE S256), OpenID Connect enabled.\nscopes:\n- scope: launch/patient\n\
  \  description: Launch in patient context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clevercarehealthplan-fhir-openapi.yml\n- scope: openid\n  description: OpenID Connect authentication\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/clevercarehealthplan-fhir-openapi.yml\n- scope: patient/*.cruds\n  description: Patient-scoped access to permitted resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clevercarehealthplan-fhir-openapi.yml\n- scope: user/*.cruds\n  description: User-scoped access to permitted resources\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/clevercarehealthplan-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevercarehealthplan/refs/heads/main/scopes/clevercarehealthplan-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Patient Access
- Provider Directory
- Drug Formulary
token_urls:
- https://fhir-portal.clevercarehealthplan.com/oauth2/token
---
