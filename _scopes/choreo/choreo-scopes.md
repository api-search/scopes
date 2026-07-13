---
api_specs:
- filename: choreo-api-management-openapi.yml
  format: yaml
  label: Choreo API Management API
  slug: api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-api-management-openapi.yml
- filename: choreo-developer-portal-openapi.yml
  format: yaml
  label: Choreo Developer Portal API
  slug: developer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-developer-portal-openapi.yml
- filename: choreo-insights-openapi.yml
  format: yaml
  label: Choreo Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-insights-openapi.yml
authorization_urls:
- https://console.choreo.dev/oauth2/authorize
- https://devportal.choreo.dev/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Choreo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Choreo publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Choreo API on a user''s behalf.


  Tokens are issued from https://console.choreo.dev/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Choreo
provider_slug: choreo
schemes:
- flows:
  - authorizationUrl: https://console.choreo.dev/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://console.choreo.dev/oauth2/token
  name: oauth2
  source: openapi/choreo-api-management-openapi.yml
- flows:
  - authorizationUrl: https://devportal.choreo.dev/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://devportal.choreo.dev/oauth2/token
  name: oauth2
  source: openapi/choreo-developer-portal-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access
  flows:
  - authorizationCode
  scope: read
- description: Write access
  flows:
  - authorizationCode
  scope: write
slug: choreo-scopes
source_filename: choreo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/choreo-api-management-openapi.yml, openapi/choreo-developer-portal-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/choreo-api-management-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://console.choreo.dev/oauth2/authorize\n    tokenUrl: https://console.choreo.dev/oauth2/token\n- name: oauth2\n  source: openapi/choreo-developer-portal-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://devportal.choreo.dev/oauth2/authorize\n    tokenUrl: https://devportal.choreo.dev/oauth2/token\nscopes:\n- scope: read\n  description: Read access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/choreo-api-management-openapi.yml\n  - openapi/choreo-developer-portal-openapi.yml\n- scope: write\n  description: Write access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/choreo-api-management-openapi.yml\n  - openapi/choreo-developer-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/scopes/choreo-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- AI Apps
- API Management
- CI/CD
- Cloud Native
- DevOps
- Developer Portal
- FinOps
- IDE
- Internal Developer Platform
- Kubernetes
- Lifecycle
- Observability
- Orchestration
- Platform Engineering
- Pro-Code API Composition
- Unified
- WSO2
- Workflows
token_urls:
- https://console.choreo.dev/oauth2/token
- https://devportal.choreo.dev/oauth2/token
---
