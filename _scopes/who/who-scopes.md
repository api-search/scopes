---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Who Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'World Health Organization (WHO) publishes 1 OAuth 2.0 scope via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the World Health Organization (WHO) API on a user''s behalf.


  Tokens are issued from https://icdaccessmanagement.who.int/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: World Health Organization (WHO)
provider_slug: who
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://icdaccessmanagement.who.int/connect/token
  name: oauth2
  source: openapi/who-icd-api-openapi.json
scope_count: 1
scope_names:
- icdapi_access
scopes:
- description: ''
  flows:
  - clientCredentials
  scope: icdapi_access
slug: who-scopes
source_filename: who-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/who-icd-api-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/who-icd-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://icdaccessmanagement.who.int/connect/token\nscopes:\n- scope: icdapi_access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/who-icd-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/who/refs/heads/main/scopes/who-scopes.yml
summary_line: 1 scope · clientCredentials
tags:
- Health
- Global Health
- Disease Surveillance
- Immunization
- Health Statistics
- ICD
- WHO
- United Nations
- Open Data
token_urls:
- https://icdaccessmanagement.who.int/connect/token
---
