---
api_specs:
- filename: acord-ngds-openapi.yml
  format: yaml
  label: ACORD Next-Generation Digital Standards (NGDS) API
  slug: acord-ngds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/openapi/acord-ngds-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Acord Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ACORD publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ACORD API on a user''s behalf.


  Tokens are issued from https://auth.insurer-internal.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ACORD
provider_slug: acord
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.insurer-internal.example.com/oauth/token
  name: oauth2
  source: openapi/acord-ngds-openapi.yml
scope_count: 4
scope_names:
- read:claims
- read:policies
- write:claims
- write:policies
scopes:
- description: Read claim data
  flows:
  - clientCredentials
  scope: read:claims
- description: Read policy data
  flows:
  - clientCredentials
  scope: read:policies
- description: Submit and update claims
  flows:
  - clientCredentials
  scope: write:claims
- description: Create and modify policies
  flows:
  - clientCredentials
  scope: write:policies
slug: acord-scopes
source_filename: acord-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acord-ngds-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/acord-ngds-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.insurer-internal.example.com/oauth/token\nscopes:\n- scope: read:claims\n  description: Read claim data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/acord-ngds-openapi.yml\n- scope: read:policies\n  description: Read policy data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/acord-ngds-openapi.yml\n- scope: write:claims\n  description: Submit and update claims\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/acord-ngds-openapi.yml\n- scope: write:policies\n  description: Create and modify policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/acord-ngds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/scopes/acord-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
token_urls:
- https://auth.insurer-internal.example.com/oauth/token
---
