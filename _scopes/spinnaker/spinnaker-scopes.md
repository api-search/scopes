---
api_specs:
- filename: spinnaker-applications-api-openapi.yml
  format: yaml
  label: Spinnaker Applications API
  slug: spinnaker-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-applications-api-openapi.yml
- filename: spinnaker-build-services-api-openapi.yml
  format: yaml
  label: Spinnaker Build Services API
  slug: spinnaker-build-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-build-services-api-openapi.yml
- filename: spinnaker-clusters-api-openapi.yml
  format: yaml
  label: Spinnaker Clusters API
  slug: spinnaker-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-clusters-api-openapi.yml
- filename: spinnaker-images-api-openapi.yml
  format: yaml
  label: Spinnaker Images API
  slug: spinnaker-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-images-api-openapi.yml
- filename: spinnaker-load-balancers-api-openapi.yml
  format: yaml
  label: Spinnaker Load Balancers API
  slug: spinnaker-load-balancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-load-balancers-api-openapi.yml
- filename: spinnaker-pipelines-api-openapi.yml
  format: yaml
  label: Spinnaker Pipelines API
  slug: spinnaker-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-pipelines-api-openapi.yml
- filename: spinnaker-projects-api-openapi.yml
  format: yaml
  label: Spinnaker Projects API
  slug: spinnaker-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-projects-api-openapi.yml
- filename: spinnaker-search-api-openapi.yml
  format: yaml
  label: Spinnaker Search API
  slug: spinnaker-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-search-api-openapi.yml
- filename: spinnaker-tasks-api-openapi.yml
  format: yaml
  label: Spinnaker Tasks API
  slug: spinnaker-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-tasks-api-openapi.yml
authorization_urls:
- https://accounts.example.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Spinnaker Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spinnaker publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spinnaker API on a user''s behalf.


  Tokens are issued from https://accounts.example.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spinnaker
provider_slug: spinnaker
schemes:
- description: OAuth 2.0 authentication for Spinnaker Gate
  flows:
  - authorizationUrl: https://accounts.example.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://accounts.example.com/oauth/token
  name: oauth2
  source: openapi/spinnaker-gate-openapi.yml
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: User email access
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect scope
  flows:
  - authorizationCode
  scope: openid
- description: User profile access
  flows:
  - authorizationCode
  scope: profile
slug: spinnaker-scopes
source_filename: spinnaker-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spinnaker-gate-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/spinnaker-gate-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.example.com/oauth/authorize\n    tokenUrl: https://accounts.example.com/oauth/token\n  description: OAuth 2.0 authentication for Spinnaker Gate\nscopes:\n- scope: email\n  description: User email access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spinnaker-gate-openapi.yml\n- scope: openid\n  description: OpenID Connect scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spinnaker-gate-openapi.yml\n- scope: profile\n  description: User profile access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spinnaker-gate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/scopes/spinnaker-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Continuous Delivery
- Containers
- DevOps
- Multi-Cloud
- Pipelines
token_urls:
- https://accounts.example.com/oauth/token
---
