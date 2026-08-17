---
api_specs:
- filename: moxe-health-chart-retrieval-initiate-openapi.json
  format: json
  label: Moxe Health Chart Retrieval API
  slug: moxe-health-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-chart-retrieval-initiate-openapi.json
- filename: moxe-health-claim-management-initiate-openapi.json
  format: json
  label: Moxe Health Claim Management API
  slug: moxe-health-claim-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-claim-management-initiate-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Moxe Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moxe Health publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Moxe Health API on a user''s behalf.


  Tokens are issued from https://${environment}-api.moxehealth.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moxe Health
provider_slug: moxe-health
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token
  name: moxe_auth
  source: openapi/moxe-health-chart-retrieval-initiate-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token
  name: moxe_auth
  source: openapi/moxe-health-chart-retrieval-status-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token
  name: moxe_auth
  source: openapi/moxe-health-claim-management-initiate-openapi.json
- flows:
  - flow: clientCredentials
    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token
  name: moxe_auth
  source: openapi/moxe-health-claim-management-status-openapi.json
scope_count: 4
scope_names:
- read:claim-management-request
- read:patient-chart-request
- write:claim-management-request
- write:patient-chart-request
scopes:
- description: ''
  flows: []
  scope: read:claim-management-request
- description: get information on existing transactions
  flows:
  - clientCredentials
  scope: read:patient-chart-request
- description: ''
  flows: []
  scope: write:claim-management-request
- description: create patient chart transactions
  flows:
  - clientCredentials
  scope: write:patient-chart-request
slug: moxe-health-scopes
source_filename: moxe-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/moxe-health-chart-retrieval-initiate-openapi.json, openapi/moxe-health-chart-retrieval-status-openapi.json,\n  openapi/moxe-health-claim-management-initiate-openapi.json, openapi/moxe-health-claim-management-status-openapi.json\nschemes:\n- name: moxe_auth\n  source: openapi/moxe-health-chart-retrieval-initiate-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token\n- name: moxe_auth\n  source: openapi/moxe-health-chart-retrieval-status-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token\n- name: moxe_auth\n  source: openapi/moxe-health-claim-management-initiate-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token\n- name: moxe_auth\n  source: openapi/moxe-health-claim-management-status-openapi.json\n  flows:\n  - flow:\
  \ clientCredentials\n    tokenUrl: https://${environment}-api.moxehealth.com/oauth/token\nscopes:\n- scope: read:claim-management-request\n  sources:\n  - openapi/moxe-health-claim-management-status-openapi.json\n- scope: read:patient-chart-request\n  description: get information on existing transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moxe-health-chart-retrieval-initiate-openapi.json\n  - openapi/moxe-health-chart-retrieval-status-openapi.json\n  - openapi/moxe-health-claim-management-initiate-openapi.json\n  - openapi/moxe-health-claim-management-status-openapi.json\n- scope: write:claim-management-request\n  sources:\n  - openapi/moxe-health-claim-management-initiate-openapi.json\n- scope: write:patient-chart-request\n  description: create patient chart transactions\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moxe-health-chart-retrieval-initiate-openapi.json\n  - openapi/moxe-health-chart-retrieval-status-openapi.json\n  - openapi/moxe-health-claim-management-initiate-openapi.json\n\
  \  - openapi/moxe-health-claim-management-status-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/scopes/moxe-health-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Healthcare
- United States
- Interoperability
- Clinical Data
- Payer
- Provider
- EHR
- Health Data Exchange
- Claims
- Risk Adjustment
token_urls:
- https://${environment}-api.moxehealth.com/oauth/token
---
