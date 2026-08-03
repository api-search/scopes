---
api_specs:
- filename: visier-administration-apis-openapi.yaml
  format: yaml
  label: Visier Administration APIs
  slug: administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-administration-apis-openapi.yaml
- filename: visier-analytic-model-apis-openapi.yaml
  format: yaml
  label: Visier Analytic Model APIs
  slug: analytic-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-analytic-model-apis-openapi.yaml
- filename: visier-authentication-apis-openapi.yaml
  format: yaml
  label: Visier Authentication APIs
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-authentication-apis-openapi.yaml
- filename: visier-data-in-apis-openapi.yaml
  format: yaml
  label: Visier Data In APIs
  slug: data-in
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-in-apis-openapi.yaml
- filename: visier-data-out-apis-openapi.yaml
  format: yaml
  label: Visier Data Out APIs
  slug: data-out
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-out-apis-openapi.yaml
- filename: visier-webhooks-openapi.yaml
  format: yaml
  label: Visier Webhooks APIs
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-webhooks-openapi.yaml
- filename: visier-planning-openapi.yaml
  format: yaml
  label: Visier Planning Public APIs
  slug: planning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-planning-openapi.yaml
- filename: visier-compensation-benchmarks-openapi.yaml
  format: yaml
  label: Visier Compensation Benchmarks API
  slug: compensation-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-compensation-benchmarks-openapi.yaml
- filename: visier-skills-intelligence-engine-openapi.yaml
  format: yaml
  label: Visier Skills Intelligence Engine API
  slug: skills-intelligence-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-skills-intelligence-engine-openapi.yaml
authorization_urls:
- /v1/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- password
kind: oauth-scopes
layout: scope
method: derived
name: Visier Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Visier publishes 2 OAuth 2.0 scopes via the authorizationCode and password flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Visier API on a user''s behalf.


  Tokens are issued from /v1/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Visier
provider_slug: visier
schemes:
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-administration-apis-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-analytic-model-apis-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-authentication-apis-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-data-in-apis-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-data-out-apis-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-planning-openapi.yaml
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  source: openapi/visier-webhooks-openapi.yaml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Grants read access
  flows:
  - authorizationCode
  - password
  scope: read
- description: Grants write access
  flows:
  - authorizationCode
  - password
  scope: write
slug: visier-scopes
source_filename: visier-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/visier-administration-apis-openapi.yaml, openapi/visier-analytic-model-apis-openapi.yaml,\n  openapi/visier-authentication-apis-openapi.yaml, openapi/visier-data-in-apis-openapi.yaml,\n  openapi/visier-data-out-apis-openapi.yaml, openapi/visier-planning-openapi.yaml, openapi/visier-webhooks-openapi.yaml\nschemes:\n- name: OAuth2Auth\n  source: openapi/visier-administration-apis-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-analytic-model-apis-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-authentication-apis-openapi.yaml\n  flows:\n  -\
  \ flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-data-in-apis-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-data-out-apis-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-planning-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n- name: OAuth2Auth\n  source: openapi/visier-webhooks-openapi.yaml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\nscopes:\n- scope: read\n  description: Grants read access\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n  - openapi/visier-webhooks-openapi.yaml\n- scope: write\n  description: Grants write access\n  flows:\n  - authorizationCode\n  - password\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n\
  \  - openapi/visier-webhooks-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/scopes/visier-scopes.yml
summary_line: 2 scopes · authorizationCode/password
tags:
- Company
- People Analytics
- Workforce Analytics
- Human Resources
- HR Technology
- Workforce Planning
- Analytics
- Business Intelligence
- Compensation
- Skills
- Artificial Intelligence
- Model Context Protocol
token_urls:
- /v1/auth/oauth2/token
---
