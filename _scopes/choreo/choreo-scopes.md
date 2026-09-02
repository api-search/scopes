---
api_specs:
- filename: choreo-alerts-api-openapi.yml
  format: yaml
  label: Choreo Alerts API
  slug: choreo-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-alerts-api-openapi.yml
- filename: choreo-apis-api-openapi.yml
  format: yaml
  label: Choreo Apis API
  slug: choreo-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-apis-api-openapi.yml
- filename: choreo-application-keys-api-openapi.yml
  format: yaml
  label: Choreo Application Keys API
  slug: choreo-application-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-application-keys-api-openapi.yml
- filename: choreo-applications-api-openapi.yml
  format: yaml
  label: Choreo Applications API
  slug: choreo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-applications-api-openapi.yml
- filename: choreo-builds-api-openapi.yml
  format: yaml
  label: Choreo Builds API
  slug: choreo-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-builds-api-openapi.yml
- filename: choreo-business-plans-api-openapi.yml
  format: yaml
  label: Choreo Business Plans API
  slug: choreo-business-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-business-plans-api-openapi.yml
- filename: choreo-components-api-openapi.yml
  format: yaml
  label: Choreo Components API
  slug: choreo-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-components-api-openapi.yml
- filename: choreo-deployments-api-openapi.yml
  format: yaml
  label: Choreo Deployments API
  slug: choreo-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-deployments-api-openapi.yml
- filename: choreo-environments-api-openapi.yml
  format: yaml
  label: Choreo Environments API
  slug: choreo-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-environments-api-openapi.yml
- filename: choreo-errors-api-openapi.yml
  format: yaml
  label: Choreo Errors API
  slug: choreo-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-errors-api-openapi.yml
- filename: choreo-latency-api-openapi.yml
  format: yaml
  label: Choreo Latency API
  slug: choreo-latency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-latency-api-openapi.yml
- filename: choreo-logs-api-openapi.yml
  format: yaml
  label: Choreo Logs API
  slug: choreo-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-logs-api-openapi.yml
- filename: choreo-organizations-api-openapi.yml
  format: yaml
  label: Choreo Organizations API
  slug: choreo-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-organizations-api-openapi.yml
- filename: choreo-projects-api-openapi.yml
  format: yaml
  label: Choreo Projects API
  slug: choreo-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-projects-api-openapi.yml
- filename: choreo-subscriptions-api-openapi.yml
  format: yaml
  label: Choreo Subscriptions API
  slug: choreo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-subscriptions-api-openapi.yml
- filename: choreo-usage-api-openapi.yml
  format: yaml
  label: Choreo Usage API
  slug: choreo-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/choreo/refs/heads/main/openapi/choreo-usage-api-openapi.yml
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
- Ai Apps
- API Management
- CI/CD
- Cloud-Native
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
- Pro-Code-API-Composition
- Unified
- WSO2
- Workflows
token_urls:
- https://console.choreo.dev/oauth2/token
- https://devportal.choreo.dev/oauth2/token
---
