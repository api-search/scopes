---
api_specs:
- filename: meditech-fhir-openapi.yml
  format: yaml
  label: Meditech Expanse FHIR API
  slug: meditech-expanse-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/openapi/meditech-fhir-openapi.yml
authorization_urls:
- https://yourhospital.meditech.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Meditech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'meditech publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the meditech API on a user''s behalf.


  Tokens are issued from https://yourhospital.meditech.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: meditech
provider_slug: meditech
schemes:
- description: SMART on FHIR OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://yourhospital.meditech.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://yourhospital.meditech.com/oauth/token
  name: SMART_OAuth2
  source: openapi/meditech-fhir-openapi.yml
scope_count: 5
scope_names:
- fhirUser
- launch
- openid
- patient/*.read
- user/*.read
scopes:
- description: FHIR user claim
  flows:
  - authorizationCode
  scope: fhirUser
- description: EHR launch context
  flows:
  - authorizationCode
  scope: launch
- description: OpenID Connect identity
  flows:
  - authorizationCode
  scope: openid
- description: Read access to all patient-owned resources
  flows:
  - authorizationCode
  scope: patient/*.read
- description: Practitioner read access to all resources
  flows:
  - authorizationCode
  scope: user/*.read
slug: meditech-scopes
source_filename: meditech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/meditech-fhir-openapi.yml\nschemes:\n- name: SMART_OAuth2\n  source: openapi/meditech-fhir-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://yourhospital.meditech.com/oauth/authorize\n    tokenUrl: https://yourhospital.meditech.com/oauth/token\n  description: SMART on FHIR OAuth 2.0 authorization\nscopes:\n- scope: fhirUser\n  description: FHIR user claim\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n- scope: launch\n  description: EHR launch context\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n- scope: openid\n  description: OpenID Connect identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n- scope: patient/*.read\n  description: Read access to all patient-owned resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n- scope: user/*.read\n\
  \  description: Practitioner read access to all resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/meditech-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meditech/refs/heads/main/scopes/meditech-scopes.yml
summary_line: 5 scopes · authorizationCode
tags: []
token_urls:
- https://yourhospital.meditech.com/oauth/token
---
