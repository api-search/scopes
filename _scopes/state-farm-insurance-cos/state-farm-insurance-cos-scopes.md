---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: State Farm Insurance Cos Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'State Farm Insurance Companies publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the State Farm Insurance Companies API on a user''s behalf.


  Tokens are issued from https://api.statefarm.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: State Farm Insurance Companies
provider_slug: state-farm-insurance-cos
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.statefarm.com/oauth/token
  name: OAuth2
  source: openapi/state-farm-insurance-cos-renters-openapi.yml
scope_count: 3
scope_names:
- renters:policy:read
- renters:policy:write
- renters:quote
scopes:
- description: Read renters insurance policy details
  flows:
  - clientCredentials
  scope: renters:policy:read
- description: Bind and manage renters insurance policies
  flows:
  - clientCredentials
  scope: renters:policy:write
- description: Create and retrieve renters insurance quotes
  flows:
  - clientCredentials
  scope: renters:quote
slug: state-farm-insurance-cos-scopes
source_filename: state-farm-insurance-cos-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/state-farm-insurance-cos-renters-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/state-farm-insurance-cos-renters-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.statefarm.com/oauth/token\nscopes:\n- scope: renters:policy:read\n  description: Read renters insurance policy details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-farm-insurance-cos-renters-openapi.yml\n- scope: renters:policy:write\n  description: Bind and manage renters insurance policies\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-farm-insurance-cos-renters-openapi.yml\n- scope: renters:quote\n  description: Create and retrieve renters insurance quotes\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/state-farm-insurance-cos-renters-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-farm-insurance-cos/refs/heads/main/scopes/state-farm-insurance-cos-scopes.yml
summary_line: 3 scopes · clientCredentials
tags: []
token_urls:
- https://api.statefarm.com/oauth/token
---
