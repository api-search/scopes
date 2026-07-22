---
api_specs:
- filename: sinai-technologies-openapi-original.yml
  format: yaml
  label: SINAI API
  slug: sinai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/openapi/sinai-technologies-openapi-original.yml
authorization_urls:
- https://auth.sinai.com/oauth2/authorize
description: ''
docs: https://docs.sinai.com/reference/accessing-the-api
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Sinai Technologies Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sinai Technologies publishes 6 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sinai Technologies API on a user''s behalf.


  Tokens are issued from https://auth.sinai.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sinai Technologies
provider_slug: sinai-technologies
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://auth.sinai.com/oauth2/token
  name: OAuth2ClientCredentialsProduction
  source: openapi/sinai-technologies-openapi-original.yml
- flows:
  - authorizationUrl: https://auth.sinai.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.sinai.com/oauth2/token
  name: OAuth2AuthCodeProduction
  source: openapi/sinai-technologies-openapi-original.yml
scope_count: 6
scope_names:
- https://api.sinai.com/organization
- https://api.sinai.com/carbon_accounting
- https://api.sinai.com/baseline_forecasts
- https://api.sinai.com/transition_plan
- https://api.sinai.com/reduction_projects
- https://api.sinai.com/decarbonization_roadmap
scopes:
- description: Organization-level data and features
  flows:
  - clientCredentials
  scope: https://api.sinai.com/organization
- description: Read/write access to carbon accounting data
  flows:
  - clientCredentials
  scope: https://api.sinai.com/carbon_accounting
- description: Read/write access to baseline forecasts data
  flows:
  - clientCredentials
  scope: https://api.sinai.com/baseline_forecasts
- description: Transition plan modeling and access
  flows:
  - clientCredentials
  scope: https://api.sinai.com/transition_plan
- description: Emissions reduction project data
  flows:
  - clientCredentials
  scope: https://api.sinai.com/reduction_projects
- description: Strategic decarbonization roadmap
  flows:
  - clientCredentials
  scope: https://api.sinai.com/decarbonization_roadmap
slug: sinai-technologies-scopes
source_filename: sinai-technologies-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sinai-technologies-openapi-original.yml\ndocs: https://docs.sinai.com/reference/accessing-the-api\nnotes: >-\n  Scopes are resource-URI style and apply to the Client Credentials flow; request\n  one or more as a space-separated `scope` parameter at the token endpoint. The\n  Authorization Code flow currently supports no scopes (access is governed by the\n  user's platform permissions). Docs enumerate an additional\n  `https://api.sinai.com/decarbonization_roadmap` scope alongside those in the\n  spec's flow map.\nschemes:\n- name: OAuth2ClientCredentialsProduction\n  source: openapi/sinai-technologies-openapi-original.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinai.com/oauth2/token\n- name: OAuth2AuthCodeProduction\n  source: openapi/sinai-technologies-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.sinai.com/oauth2/authorize\n    tokenUrl:\
  \ https://auth.sinai.com/oauth2/token\nscopes:\n- scope: https://api.sinai.com/organization\n  description: Organization-level data and features\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n- scope: https://api.sinai.com/carbon_accounting\n  description: Read/write access to carbon accounting data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n- scope: https://api.sinai.com/baseline_forecasts\n  description: Read/write access to baseline forecasts data\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n- scope: https://api.sinai.com/transition_plan\n  description: Transition plan modeling and access\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n- scope: https://api.sinai.com/reduction_projects\n  description: Emissions reduction project data\n  flows:\n  - clientCredentials\n  sources:\n\
  \  - openapi/sinai-technologies-openapi-original.yml\n- scope: https://api.sinai.com/decarbonization_roadmap\n  description: Strategic decarbonization roadmap\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/sinai-technologies-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinai-technologies/refs/heads/main/scopes/sinai-technologies-scopes.yml
summary_line: 6 scopes · clientCredentials/authorizationCode
tags:
- Company
- Carbon Management
- Carbon Accounting
- Emissions
- Sustainability
- ESG
- Decarbonization
- Climate
token_urls:
- https://auth.sinai.com/oauth2/token
---
