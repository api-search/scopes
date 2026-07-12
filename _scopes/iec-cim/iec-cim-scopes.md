---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Iec Cim Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'iec-cim publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the iec-cim API on a user''s behalf.


  Tokens are issued from https://auth.utility.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: iec-cim
provider_slug: iec-cim
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.utility.example.com/oauth/token
  name: OAuth2
  source: openapi/iec-cim-61968-distribution-openapi.yml
scope_count: 2
scope_names:
- cim.read
- cim.write
scopes:
- description: Read CIM data
  flows:
  - clientCredentials
  scope: cim.read
- description: Write CIM data
  flows:
  - clientCredentials
  scope: cim.write
slug: iec-cim-scopes
source_filename: iec-cim-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/iec-cim-61968-distribution-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/iec-cim-61968-distribution-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.utility.example.com/oauth/token\nscopes:\n- scope: cim.read\n  description: Read CIM data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/iec-cim-61968-distribution-openapi.yml\n- scope: cim.write\n  description: Write CIM data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/iec-cim-61968-distribution-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iec-cim/refs/heads/main/scopes/iec-cim-scopes.yml
summary_line: 2 scopes · clientCredentials
tags: []
token_urls:
- https://auth.utility.example.com/oauth/token
---
