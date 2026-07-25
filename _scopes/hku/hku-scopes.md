---
api_specs:
- filename: hku-altmetric-api-openapi.yml
  format: yaml
  label: University of Hong Kong altmetric API
  slug: hku-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-altmetric-api-openapi.yml
- filename: hku-articles-api-openapi.yml
  format: yaml
  label: University of Hong Kong articles API
  slug: hku-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-articles-api-openapi.yml
- filename: hku-authors-api-openapi.yml
  format: yaml
  label: University of Hong Kong authors API
  slug: hku-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-authors-api-openapi.yml
- filename: hku-collections-api-openapi.yml
  format: yaml
  label: University of Hong Kong collections API
  slug: hku-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-collections-api-openapi.yml
- filename: hku-institutions-api-openapi.yml
  format: yaml
  label: University of Hong Kong institutions API
  slug: hku-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-institutions-api-openapi.yml
- filename: hku-oauth-api-openapi.yml
  format: yaml
  label: University of Hong Kong oauth API
  slug: hku-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-oauth-api-openapi.yml
- filename: hku-other-api-openapi.yml
  format: yaml
  label: University of Hong Kong other API
  slug: hku-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-other-api-openapi.yml
- filename: hku-profiles-api-openapi.yml
  format: yaml
  label: University of Hong Kong profiles API
  slug: hku-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-profiles-api-openapi.yml
- filename: hku-projects-api-openapi.yml
  format: yaml
  label: University of Hong Kong projects API
  slug: hku-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-projects-api-openapi.yml
- filename: hku-symplectic-api-openapi.yml
  format: yaml
  label: University of Hong Kong symplectic API
  slug: hku-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Hku Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Hong Kong publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Hong Kong API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Hong Kong
provider_slug: hku
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/hku-datahub.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: hku-scopes
source_filename: hku-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hku-datahub.yaml\nschemes:\n- name: OAuth2\n  source: openapi/hku-datahub.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/hku-datahub.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/scopes/hku-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Hong Kong
token_urls:
- https://api.figshare.com/v2/token
---
