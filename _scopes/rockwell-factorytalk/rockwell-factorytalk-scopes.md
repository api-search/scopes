---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Rockwell Factorytalk Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'rockwell-factorytalk publishes 3 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the rockwell-factorytalk API on a user''s behalf.


  Tokens are issued from https://optix.example.com/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: rockwell-factorytalk
provider_slug: rockwell-factorytalk
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://optix.example.com/auth/token
  name: oauth2
  source: openapi/rockwell-factorytalk-optix-openapi.yml
scope_count: 3
scope_names:
- optix.admin
- optix.read
- optix.write
scopes:
- description: Manage recipes and project configuration
  flows:
  - clientCredentials
  scope: optix.admin
- description: Read tag values and alarm data
  flows:
  - clientCredentials
  scope: optix.read
- description: Write tag values
  flows:
  - clientCredentials
  scope: optix.write
slug: rockwell-factorytalk-scopes
source_filename: rockwell-factorytalk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rockwell-factorytalk-optix-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/rockwell-factorytalk-optix-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://optix.example.com/auth/token\nscopes:\n- scope: optix.admin\n  description: Manage recipes and project configuration\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/rockwell-factorytalk-optix-openapi.yml\n- scope: optix.read\n  description: Read tag values and alarm data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/rockwell-factorytalk-optix-openapi.yml\n- scope: optix.write\n  description: Write tag values\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/rockwell-factorytalk-optix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/scopes/rockwell-factorytalk-scopes.yml
summary_line: 3 scopes · clientCredentials
tags: []
token_urls:
- https://optix.example.com/auth/token
---
