---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Culture Amp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Culture Amp publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Culture Amp API on a user''s behalf.


  Tokens are issued from /oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Culture Amp
provider_slug: culture-amp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: /oauth2/token
  name: Oauth2
  source: openapi/culture-amp-public-api-openapi.yml
scope_count: 4
scope_names:
- employee-demographics-read
- employees-read
- performance-evaluations-read
- surveys-read
scopes:
- description: Grants access to employee demographics
  flows:
  - clientCredentials
  scope: employee-demographics-read
- description: Grants read access to employees resources
  flows:
  - clientCredentials
  scope: employees-read
- description: Grants access to employee performance evaluations
  flows:
  - clientCredentials
  scope: performance-evaluations-read
- description: ''
  flows: []
  scope: surveys-read
slug: culture-amp-scopes
source_filename: culture-amp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/culture-amp-public-api-openapi.yml\nschemes:\n- name: Oauth2\n  source: openapi/culture-amp-public-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth2/token\nscopes:\n- scope: employee-demographics-read\n  description: Grants access to employee demographics\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/culture-amp-public-api-openapi.yml\n- scope: employees-read\n  description: Grants read access to employees resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/culture-amp-public-api-openapi.yml\n- scope: performance-evaluations-read\n  description: Grants access to employee performance evaluations\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/culture-amp-public-api-openapi.yml\n- scope: surveys-read\n  sources:\n  - openapi/culture-amp-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/scopes/culture-amp-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- HR
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Human Resources
token_urls:
- /oauth2/token
---
