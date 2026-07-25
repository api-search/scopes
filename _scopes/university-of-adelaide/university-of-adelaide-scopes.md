---
api_specs:
- filename: university-of-adelaide-altmetric-api-openapi.yml
  format: yaml
  label: University of Adelaide altmetric API
  slug: university-of-adelaide-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-altmetric-api-openapi.yml
- filename: university-of-adelaide-articles-api-openapi.yml
  format: yaml
  label: University of Adelaide articles API
  slug: university-of-adelaide-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-articles-api-openapi.yml
- filename: university-of-adelaide-authors-api-openapi.yml
  format: yaml
  label: University of Adelaide authors API
  slug: university-of-adelaide-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-authors-api-openapi.yml
- filename: university-of-adelaide-collections-api-openapi.yml
  format: yaml
  label: University of Adelaide collections API
  slug: university-of-adelaide-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-collections-api-openapi.yml
- filename: university-of-adelaide-institutions-api-openapi.yml
  format: yaml
  label: University of Adelaide institutions API
  slug: university-of-adelaide-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-institutions-api-openapi.yml
- filename: university-of-adelaide-oauth-api-openapi.yml
  format: yaml
  label: University of Adelaide oauth API
  slug: university-of-adelaide-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-oauth-api-openapi.yml
- filename: university-of-adelaide-other-api-openapi.yml
  format: yaml
  label: University of Adelaide other API
  slug: university-of-adelaide-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-other-api-openapi.yml
- filename: university-of-adelaide-profiles-api-openapi.yml
  format: yaml
  label: University of Adelaide profiles API
  slug: university-of-adelaide-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-profiles-api-openapi.yml
- filename: university-of-adelaide-projects-api-openapi.yml
  format: yaml
  label: University of Adelaide projects API
  slug: university-of-adelaide-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-projects-api-openapi.yml
- filename: university-of-adelaide-symplectic-api-openapi.yml
  format: yaml
  label: University of Adelaide symplectic API
  slug: university-of-adelaide-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/openapi/university-of-adelaide-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: University Of Adelaide Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Adelaide publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Adelaide API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Adelaide
provider_slug: university-of-adelaide
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/university-of-adelaide-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: university-of-adelaide-scopes
source_filename: university-of-adelaide-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-adelaide-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/university-of-adelaide-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/university-of-adelaide-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-adelaide/refs/heads/main/scopes/university-of-adelaide-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Institutional Repository
- Open Data
- Australia
token_urls:
- https://api.figshare.com/v2/token
---
