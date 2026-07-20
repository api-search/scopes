---
api_specs:
- filename: cosmo-tech-organization-openapi-original.yaml
  format: yaml
  label: Cosmo Tech Cloud Platform API
  slug: cosmo-tech-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmo-tech/refs/heads/main/openapi/cosmo-tech-organization-openapi-original.yaml
authorization_urls:
- https://example.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cosmo Tech Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cosmo Tech uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://example.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cosmo Tech
provider_slug: cosmo-tech
schemes:
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-dataset-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-meta-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-organization-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-run-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-runner-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-solution-openapi-original.yaml
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  source: openapi/cosmo-tech-workspace-openapi-original.yaml
scope_count: 0
scope_names: []
scopes: []
slug: cosmo-tech-scopes
source_filename: cosmo-tech-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cosmo-tech-dataset-openapi-original.yaml, openapi/cosmo-tech-meta-openapi-original.yaml,\n  openapi/cosmo-tech-organization-openapi-original.yaml, openapi/cosmo-tech-run-openapi-original.yaml,\n  openapi/cosmo-tech-runner-openapi-original.yaml, openapi/cosmo-tech-solution-openapi-original.yaml,\n  openapi/cosmo-tech-workspace-openapi-original.yaml\nschemes:\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-dataset-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-meta-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-organization-openapi-original.yaml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-run-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-runner-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-solution-openapi-original.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\n- name: oAuth2AuthCode\n  source: openapi/cosmo-tech-workspace-openapi-original.yaml\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n  description: OAuth2 authentication\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmo-tech/refs/heads/main/scopes/cosmo-tech-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Simulation
- Digital Twin
- Artificial Intelligence
- Supply Chain
- Predictive Analytics
- Industrial
token_urls:
- https://example.com/token
---
