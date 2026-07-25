---
api_specs:
- filename: uon-altmetric-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia altmetric API
  slug: uon-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-altmetric-api-openapi.yml
- filename: uon-articles-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia articles API
  slug: uon-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-articles-api-openapi.yml
- filename: uon-authors-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia authors API
  slug: uon-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-authors-api-openapi.yml
- filename: uon-collections-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia collections API
  slug: uon-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-collections-api-openapi.yml
- filename: uon-institutions-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia institutions API
  slug: uon-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-institutions-api-openapi.yml
- filename: uon-oauth-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia oauth API
  slug: uon-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-oauth-api-openapi.yml
- filename: uon-other-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia other API
  slug: uon-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-other-api-openapi.yml
- filename: uon-profiles-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia profiles API
  slug: uon-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-profiles-api-openapi.yml
- filename: uon-projects-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia projects API
  slug: uon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-projects-api-openapi.yml
- filename: uon-symplectic-api-openapi.yml
  format: yaml
  label: University of Newcastle Australia symplectic API
  slug: uon-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/openapi/uon-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Uon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Newcastle Australia publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Newcastle Australia API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Newcastle Australia
provider_slug: uon
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/uon-open-research-figshare.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: uon-scopes
source_filename: uon-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uon-open-research-figshare.yaml\nschemes:\n- name: OAuth2\n  source: openapi/uon-open-research-figshare.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/uon-open-research-figshare.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uon/refs/heads/main/scopes/uon-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Research
- Open Access
- Repository
- OAI-PMH
- Australia
token_urls:
- https://api.figshare.com/v2/token
---
