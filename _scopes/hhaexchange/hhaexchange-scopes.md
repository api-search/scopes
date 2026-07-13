---
api_specs:
- filename: hhaexchange-fhir-openapi.yml
  format: yaml
  label: HHAeXchange EVV API
  slug: hhaexchange-evv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/openapi/hhaexchange-fhir-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Hhaexchange Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HHAeXchange publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the HHAeXchange API on a user''s behalf.


  Tokens are issued from https://api.hhaexchange.com/v1/fhir/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HHAeXchange
provider_slug: hhaexchange
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.hhaexchange.com/v1/fhir/auth/token
  name: bearerAuth
  source: openapi/hhaexchange-fhir-openapi.yml
scope_count: 1
scope_names:
- full_access
scopes:
- description: Read and write access for Internal Provider, Onboarding, and Rate limits.
  flows:
  - clientCredentials
  scope: full_access
slug: hhaexchange-scopes
source_filename: hhaexchange-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hhaexchange-fhir-openapi.yml\nschemes:\n- name: bearerAuth\n  source: openapi/hhaexchange-fhir-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.hhaexchange.com/v1/fhir/auth/token\nscopes:\n- scope: full_access\n  description: Read and write access for Internal Provider, Onboarding, and Rate limits.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/hhaexchange-fhir-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hhaexchange/refs/heads/main/scopes/hhaexchange-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Homecare
- EVV
- Electronic Visit Verification
- Medicaid
- Scheduling
- Caregiver
- Healthcare
token_urls:
- https://api.hhaexchange.com/v1/fhir/auth/token
---
