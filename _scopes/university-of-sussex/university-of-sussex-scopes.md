---
api_specs:
- filename: university-of-sussex-altmetric-api-openapi.yml
  format: yaml
  label: University of Sussex altmetric API
  slug: university-of-sussex-altmetric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-altmetric-api-openapi.yml
- filename: university-of-sussex-articles-api-openapi.yml
  format: yaml
  label: University of Sussex articles API
  slug: university-of-sussex-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-articles-api-openapi.yml
- filename: university-of-sussex-authors-api-openapi.yml
  format: yaml
  label: University of Sussex authors API
  slug: university-of-sussex-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-authors-api-openapi.yml
- filename: university-of-sussex-collections-api-openapi.yml
  format: yaml
  label: University of Sussex collections API
  slug: university-of-sussex-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-collections-api-openapi.yml
- filename: university-of-sussex-institutions-api-openapi.yml
  format: yaml
  label: University of Sussex institutions API
  slug: university-of-sussex-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-institutions-api-openapi.yml
- filename: university-of-sussex-oauth-api-openapi.yml
  format: yaml
  label: University of Sussex oauth API
  slug: university-of-sussex-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-oauth-api-openapi.yml
- filename: university-of-sussex-other-api-openapi.yml
  format: yaml
  label: University of Sussex other API
  slug: university-of-sussex-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-other-api-openapi.yml
- filename: university-of-sussex-profiles-api-openapi.yml
  format: yaml
  label: University of Sussex profiles API
  slug: university-of-sussex-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-profiles-api-openapi.yml
- filename: university-of-sussex-projects-api-openapi.yml
  format: yaml
  label: University of Sussex projects API
  slug: university-of-sussex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-projects-api-openapi.yml
- filename: university-of-sussex-symplectic-api-openapi.yml
  format: yaml
  label: University of Sussex symplectic API
  slug: university-of-sussex-symplectic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/openapi/university-of-sussex-symplectic-api-openapi.yml
authorization_urls:
- https://figshare.com/account/applications/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: University Of Sussex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Sussex publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the University of Sussex API on a user''s behalf.


  Tokens are issued from https://api.figshare.com/v2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Sussex
provider_slug: university-of-sussex
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  source: openapi/university-of-sussex-figshare-repository.yaml
scope_count: 1
scope_names:
- all
scopes:
- description: Grants all access
  flows:
  - authorizationCode
  scope: all
slug: university-of-sussex-scopes
source_filename: university-of-sussex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-sussex-figshare-repository.yaml\nschemes:\n- name: OAuth2\n  source: openapi/university-of-sussex-figshare-repository.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\nscopes:\n- scope: all\n  description: Grants all access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/university-of-sussex-figshare-repository.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sussex/refs/heads/main/scopes/university-of-sussex-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- United Kingdom
token_urls:
- https://api.figshare.com/v2/token
---
