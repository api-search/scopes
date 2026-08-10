---
api_specs:
- filename: bezero-carbon-projects-api-openapi.yml
  format: yaml
  label: BeZero Carbon Projects API
  slug: bezero-carbon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-projects-api-openapi.yml
- filename: bezero-carbon-ratings-api-openapi.yml
  format: yaml
  label: BeZero Carbon Ratings API
  slug: bezero-carbon-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-ratings-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bezero Carbon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BeZero Carbon publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BeZero Carbon API on a user''s behalf.


  Tokens are issued from https://login.bezerocarbonmarkets.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BeZero Carbon
provider_slug: bezero-carbon
schemes:
- description: This API uses OAuth 2 with Client Credentials
  flows:
  - flow: clientCredentials
    tokenUrl: https://login.bezerocarbonmarkets.com/oauth2/token
  name: OAuth2
  source: openapi/bezero-carbon-ratings-openapi.yml
scope_count: 4
scope_names:
- bcm/v3.projects:list
- bcm/v3.ratings:details
- bcm/v3.ratings:list
- bcm/v3.ratings:riskFactors
scopes:
- description: list projects
  flows:
  - clientCredentials
  scope: bcm/v3.projects:list
- description: read rating details
  flows:
  - clientCredentials
  scope: bcm/v3.ratings:details
- description: list ratings
  flows:
  - clientCredentials
  scope: bcm/v3.ratings:list
- description: read rating risk factors
  flows:
  - clientCredentials
  scope: bcm/v3.ratings:riskFactors
slug: bezero-carbon-scopes
source_filename: bezero-carbon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: derived\nsource: openapi/bezero-carbon-ratings-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/bezero-carbon-ratings-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.bezerocarbonmarkets.com/oauth2/token\n  description: This API uses OAuth 2 with Client Credentials\nscopes:\n- scope: bcm/v3.projects:list\n  description: list projects\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bezero-carbon-ratings-openapi.yml\n- scope: bcm/v3.ratings:details\n  description: read rating details\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bezero-carbon-ratings-openapi.yml\n- scope: bcm/v3.ratings:list\n  description: list ratings\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bezero-carbon-ratings-openapi.yml\n- scope: bcm/v3.ratings:riskFactors\n  description: read rating risk factors\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/bezero-carbon-ratings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/scopes/bezero-carbon-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- Company
- Carbon Ratings
- Carbon Markets
- Climate
- Sustainability
- ESG
- Ratings
- Reference Data
- Market Intelligence
- Risk Analysis
token_urls:
- https://login.bezerocarbonmarkets.com/oauth2/token
---
