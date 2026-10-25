---
api_specs:
- filename: culture-amp-employees-api-openapi.yml
  format: yaml
  label: Culture Amp Employees API
  slug: culture-amp-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-employees-api-openapi.yml
- filename: culture-amp-performance-api-openapi.yml
  format: yaml
  label: Culture Amp Performance API
  slug: culture-amp-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-performance-api-openapi.yml
- filename: culture-amp-surveys-api-openapi.yml
  format: yaml
  label: Culture Amp Surveys API
  slug: culture-amp-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-surveys-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.api.cultureamp.com/docs/customer-guide-authorization-scopes
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Culture Amp Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Culture Amp publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Culture Amp API on a user''s behalf.


  Tokens are issued from https://api.cultureamp.com/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Culture Amp
provider_slug: culture-amp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.cultureamp.com/v1/oauth2/token
  name: Oauth2
  sources:
  - openapi/culture-amp-employees-api-openapi.yml
  - openapi/culture-amp-performance-api-openapi.yml
  - openapi/culture-amp-surveys-api-openapi.yml
scope_count: 4
scope_names:
- employees-read
- employee-demographics-read
- performance-evaluations-read
- surveys-read
scopes:
- description: Provides access to basic employee data
  flows:
  - clientCredentials
  scope: employees-read
- description: Provides access to employee demographic data
  flows:
  - clientCredentials
  scope: employee-demographics-read
- description: Provides access to performance evaluation data
  flows:
  - clientCredentials
  scope: performance-evaluations-read
- description: Provides access to engagement survey data
  flows:
  - clientCredentials
  scope: surveys-read
slug: culture-amp-scopes
source_filename: culture-amp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://docs.api.cultureamp.com/docs/customer-guide-authorization-scopes\ndocs: https://docs.api.cultureamp.com/docs/customer-guide-authorization-scopes\nschemes:\n- name: Oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cultureamp.com/v1/oauth2/token\n  sources:\n  - openapi/culture-amp-employees-api-openapi.yml\n  - openapi/culture-amp-performance-api-openapi.yml\n  - openapi/culture-amp-surveys-api-openapi.yml\nscope_format: target-entity:<entity id>:<comma separated list of permissions>\ntarget_entities:\n- id: 8ed17dce-9eca-4383-a9e1-54f82c362b6d\n  description: The entity id to use when calling the production API\n- id: 79040b4d-3e2b-4480-a061-2e230eeb83b2\n  description: The entity id to use when calling the sandbox API\nscopes:\n- scope: employees-read\n  description: Provides access to basic employee data\n  flows:\n  - clientCredentials\n- scope: employee-demographics-read\n  description: Provides\
  \ access to employee demographic data\n  flows:\n  - clientCredentials\n- scope: performance-evaluations-read\n  description: Provides access to performance evaluation data\n  flows:\n  - clientCredentials\n- scope: surveys-read\n  description: Provides access to engagement survey data\n  flows:\n  - clientCredentials\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/scopes/culture-amp-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Human Resources
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Australia
token_bound: false
token_urls:
- https://api.cultureamp.com/v1/oauth2/token
---
