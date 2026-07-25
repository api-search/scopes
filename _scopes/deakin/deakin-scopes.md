---
api_specs:
- filename: deakin-altmetric-api-openapi.yml
  format: yaml
  label: Deakin University altmetric API
  slug: deakin-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-altmetric-api-openapi.yml
- filename: deakin-articles-api-openapi.yml
  format: yaml
  label: Deakin University articles API
  slug: deakin-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-articles-api-openapi.yml
- filename: deakin-authors-api-openapi.yml
  format: yaml
  label: Deakin University authors API
  slug: deakin-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-authors-api-openapi.yml
- filename: deakin-collections-api-openapi.yml
  format: yaml
  label: Deakin University collections API
  slug: deakin-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-collections-api-openapi.yml
- filename: deakin-institutions-api-openapi.yml
  format: yaml
  label: Deakin University institutions API
  slug: deakin-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-institutions-api-openapi.yml
- filename: deakin-oauth-api-openapi.yml
  format: yaml
  label: Deakin University oauth API
  slug: deakin-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-oauth-api-openapi.yml
- filename: deakin-other-api-openapi.yml
  format: yaml
  label: Deakin University other API
  slug: deakin-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-other-api-openapi.yml
- filename: deakin-profiles-api-openapi.yml
  format: yaml
  label: Deakin University profiles API
  slug: deakin-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-profiles-api-openapi.yml
- filename: deakin-projects-api-openapi.yml
  format: yaml
  label: Deakin University projects API
  slug: deakin-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-projects-api-openapi.yml
- filename: deakin-symplectic-api-openapi.yml
  format: yaml
  label: Deakin University symplectic API
  slug: deakin-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/openapi/deakin-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Deakin Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Deakin University publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deakin University API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deakin University
provider_slug: deakin
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/deakin-figshare-api.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: deakin-scopes
source_filename: deakin-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deakin-figshare-api.yaml\nschemes:\n- name: OAuth2\n  source: openapi/deakin-figshare-api.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/deakin-figshare-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deakin/refs/heads/main/scopes/deakin-scopes.yml
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
