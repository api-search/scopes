---
api_specs:
- filename: monash-altmetric-api-openapi.yml
  format: yaml
  label: Monash University altmetric API
  slug: monash-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-altmetric-api-openapi.yml
- filename: monash-articles-api-openapi.yml
  format: yaml
  label: Monash University articles API
  slug: monash-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-articles-api-openapi.yml
- filename: monash-authors-api-openapi.yml
  format: yaml
  label: Monash University authors API
  slug: monash-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-authors-api-openapi.yml
- filename: monash-collections-api-openapi.yml
  format: yaml
  label: Monash University collections API
  slug: monash-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-collections-api-openapi.yml
- filename: monash-institutions-api-openapi.yml
  format: yaml
  label: Monash University institutions API
  slug: monash-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-institutions-api-openapi.yml
- filename: monash-oauth-api-openapi.yml
  format: yaml
  label: Monash University oauth API
  slug: monash-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-oauth-api-openapi.yml
- filename: monash-other-api-openapi.yml
  format: yaml
  label: Monash University other API
  slug: monash-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-other-api-openapi.yml
- filename: monash-profiles-api-openapi.yml
  format: yaml
  label: Monash University profiles API
  slug: monash-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-profiles-api-openapi.yml
- filename: monash-projects-api-openapi.yml
  format: yaml
  label: Monash University projects API
  slug: monash-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-projects-api-openapi.yml
- filename: monash-symplectic-api-openapi.yml
  format: yaml
  label: Monash University symplectic API
  slug: monash-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/openapi/monash-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Monash Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Monash University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Monash University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Monash University
provider_slug: monash
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/monash-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: monash-scopes
source_filename: monash-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/monash-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/monash-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/monash-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monash/refs/heads/main/scopes/monash-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Australia
token_urls:
- https://api.figshare.com/v2/token
---
