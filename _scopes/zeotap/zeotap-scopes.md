---
api_specs:
- filename: zeotap-openapi.yml
  format: yaml
  label: Zeotap Profile API
  slug: zeotap-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zeotap/openapi/zeotap-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Zeotap Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zeotap publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zeotap API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zeotap
provider_slug: zeotap
schemes: []
scope_count: 3
scope_names:
- profile.read
- profile.write
- profile.delete
scopes:
- description: Read user profile data
  flows: []
  scope: profile.read
- description: Write or update user profile data
  flows: []
  scope: profile.write
- description: Delete user profile data
  flows: []
  scope: profile.delete
slug: zeotap-scopes
source_filename: zeotap-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.zeotap.com/profile-api/profileapi.md\nscopes:\n  - name: profile.read\n    description: Read user profile data\n  - name: profile.write\n    description: Write or update user profile data\n  - name: profile.delete\n    description: Delete user profile data\n"
source_yaml_url: https://artifacts.apis.io/zeotap/scopes/zeotap-scopes.yml
summary_line: 3 scopes
tags:
- Company
- Artificial Intelligence
- Customer Data Platform
- Data Integration
- Identity Resolution
token_bound: false
token_urls: []
---
